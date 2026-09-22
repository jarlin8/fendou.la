---
title: "奋斗博客主题和功能设定修改记录"
post_status: "publish"
post_password: "1"
skip_file: "no"
post_date: "2023-12-29T04:10:00.000Z"
taxonomy:
  category:
        - log
  post_tag:
        - 代码
post_excerpt: ""
---
## Git-it-write插件支持post_password字段

文件：`/www/wwwroot/fendou.la/wp-content/plugins/git-it-write/includes/publisher.php`（备份：publisher.php.bak），共 3 处：

1. 第 142 行：读取 YAML 头部的 post_password

1. 第 173 行：无 front matter 时默认空值

1. 第 207 行：post_password 加入 wp_insert_post 的文章数据数组

作用：让插件把 YAML 顶层的 `post_password: "密码"` 写入 wp_posts 表字段，启用密码保护。语法检查已通过。

**要注意什么**

1. **插件更新会覆盖修改**，更新后需按上面 3 处重改

1. YAML 中密码必须放**顶层**，放 custom_fields 无效（会存成没用的 meta）

1. Notion 数据库需添加 Text 类型属性 `post_password`，留空则不加密

## 说说添加Nginx层面的加密

给站点 [fendou.la](http://fendou.la/) 的说说页面（WordPress 自定义文章类型，非真实目录）添加访问密码。

**关键结论（重点）**

宝塔面板的『目录密码保护』功能只适用于真实存在的文件夹，说说不是目录，所以面板保存时报错（生成的配置缺分号导致 nginx -t 失败）。最终改用 nginx 按 URL 路径保护实现。

**具体修改（共 3 处）**

1. **新增保护配置**

`文件：/www/server/panel/vhost/nginx/dir_auth/www.fendou.la/shuoshuo.conf`

内容：location 匹配所有 /shuoshuo 开头的请求，要求 Basic 认证，认证后交给 WordPress 处理。此文件被站点主配置 www.fendou.la.conf 中的 dir_auth include 自动加载。

* **新增密码文件**

```plain text
文件：/www/server/passwd/shuo.pass
属主：www:www（重点：nginx worker 以 www 运行，属主不对会 500）
权限：640
```

当前凭据：用户名 **，密码 `1****1`（文件内为加密哈希，非明文）。改密码命令：`printf '1:%s\n' "$(openssl passwd -apr1 新密码)" > /www/server/passwd/shuo.pass`，改完即生效，无需重载 nginx。

* **清理伪静态文件中的残留规则**

`文件：/www/server/panel/vhost/rewrite/www.fendou.la.conf`

删除了其中一段旧的手写 /shuo 保护规则（它引用已删除的 shuo.conf 当密码文件，导致旧路径弹框且认证后 500）。现只保留 WordPress 默认伪静态和 wp-admin 重定向。

**维护要点**

* 改路径：编辑 shuoshuo.conf 里的 location 正则，然后 `nginx -t && nginx -s reload`；

* 改用户名/密码：见上方命令，即时生效；

* 取消保护：删除 shuoshuo.conf 后 reload nginx；

* 验证命令：`curl -o /dev/null -w '%{http_code}\n' -u 1:123321 <https://fendou.la/shuoshuo`（未认证应> 401，带密码应 200）；