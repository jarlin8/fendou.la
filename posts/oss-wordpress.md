---
ID: 13828
title: >
  7个有用的wordpress图片云储存方案
slug: oss-wordpress
post_date: 2021-04-10 22:19:03
layout: post
post_excerpt:
post_status: publish
post_tag: [ ]
category:
  - 杂谈系列
---
<!-- wp:paragraph -->

储存图片一直是我们这些小站长的难题，本地占用空间大，速度还提不起来。

<!-- /wp:paragraph -->

<!-- wp:paragraph -->

这里搜集整理了三个可用的解决方案和插件分享：

<!-- /wp:paragraph -->

<!-- wp:list {"textColor":"white","gradient":"vivid-cyan-blue-to-vivid-purple"} -->

<ul class="has-white-color has-vivid-cyan-blue-to-vivid-purple-gradient-background has-text-color has-background">
  <li>
    阿里云OSS
  </li>
  <li>
    腾讯云COS
  </li>
  <li>
    远程上传到Github使用Jsdelivr CDN加速
  </li>
</ul>

<!-- /wp:list -->

<!-- wp:paragraph -->

阿里云是我自己在使用的，一起开了CDN,后来没有啥访问量，很鸡肋，就关掉了。

<!-- /wp:paragraph -->

<!-- wp:heading -->

## 阿里云OSS {#阿里云oss}

<!-- /wp:heading -->

<!-- wp:heading {"level":3} -->

### Aliyun** OSS ** {#aliyun-oss}

<!-- /wp:heading -->

<!-- wp:paragraph -->

作者： <a href="https://yii.im/" target="_blank" rel="nofollow noopener" data-schema-attribute="">Ivan Chou</a>在wordpress后台插件库可以直接搜索到，目前使用正常，好像快两年没有更新了。推荐使用wordpress插件页面安装的3.2.7版本，新版3.30在wordpress5.7里面出现故障，提示致命错误。

<!-- /wp:paragraph -->

<!-- wp:paragraph -->

github仓库地址：<a href="https://github.com/yiichou/aliyun-oss-support" target="_blank" rel="noopener" data-schema-attribute="">https://github.com/yiichou/aliyun-oss-support</a>

<!-- /wp:paragraph -->

<!-- wp:heading {"level":4} -->

#### 插件特点 {#插件特点}

<!-- /wp:heading -->

<!-- wp:list {"ordered":true,"backgroundColor":"vivid-cyan-blue","textColor":"white"} -->

<ol class="has-white-color has-vivid-cyan-blue-background-color has-text-color has-background">
  <li>
    支持 Aliyun OSS 的图片服务（根据参数获得不同尺寸的图片）
  </li>
  <li>
    自定义文件在 Bucket 上的存储位置
  </li>
  <li>
    支持 Https 站点
  </li>
  <li>
    支持阿里云内网和 VPC 网络
  </li>
  <li>
    全格式附件支持，不仅仅是图片
  </li>
  <li>
    支持 WordPress 4.4+ 新功能 srcset，在不同分辨率设备上加载不同大小图片
  </li>
  <li>
    支持 WordPress 5.0+ 默认古藤堡编辑器Gutenburg
  </li>
  <li>
    支持阿里云url鉴权，实现高级别防盗链功能，支持阿里云CDN的A、B、C所有方式鉴权，推荐A方式
  </li>
  <li>
    支持在 WordPress 后台编辑图片
  </li>
  <li>
    支持预设图片样式，图片保护，自定义分割符
  </li>
  <li>
    中英文双语支持，方便使用英文为默认语言的同学
  </li>
  <li>
    支持在其他插件/主题中通过系统钩子调用插件功能
  </li>
  <li>
    代码遵循 PSR-4 规则编写
  </li>
</ol>

<!-- /wp:list -->

<!-- wp:heading {"level":3} -->

### Aliyun-oss-wordpress {#aliyun-oss-wordpress}

<!-- /wp:heading -->

<!-- wp:paragraph -->

该插件将 WordPress 站点图片等多媒体文件直接上传到阿里云对象存储 OSS 中，一键将静态资源托管到阿里云

<!-- /wp:paragraph -->

<!-- wp:paragraph -->

github仓库地址：<a href="https://github.com/sy-records/aliyun-oss-wordpress" target="_blank" rel="nofollow noopener" data-schema-attribute="">https://github.com/sy-records/aliyun-oss-wordpress</a>

<!-- /wp:paragraph -->

<!-- wp:heading {"level":4} -->

#### 插件特点 {#插件特点}

<!-- /wp:heading -->

<!-- wp:paragraph {"backgroundColor":"vivid-cyan-blue","textColor":"white"} -->

<p class="has-white-color has-vivid-cyan-blue-background-color has-text-color has-background">
  1. 可配置是否上传缩略图和是否保留本地备份<br />2. 本地删除可同步删除阿里云对象存储 OSS 中的文件<br />3. 支持阿里云对象存储 OSS 绑定的用户域名<br />4. 支持替换数据库中旧的资源链接地址<br />5. 支持阿里云对象存储 OSS 完整地域使用<br />6. 支持同步历史附件到阿里云对象存储 OSS<br />7. 支持使用阿里云内网传输
</p>

<!-- /wp:paragraph -->

<!-- wp:heading -->

## 腾讯云COS云存储插件 {#腾讯云cos云存储插件}

<!-- /wp:heading -->

<!-- wp:paragraph -->

该插件将 WordPress 站点图片等多媒体文件直接上传到腾讯云对象存储 COS 中，该插件依赖腾讯云对象存储 COS。

<!-- /wp:paragraph -->

<!-- wp:paragraph -->

**Github 下载节点：**<a href="https://github.com/sy-records/wordpress-qcloud-cos/releases/latest" target="_blank" rel="noopener" data-schema-attribute="">https://github.com/sy-records/wordpress-qcloud-cos/releases/latest</a>

<!-- /wp:paragraph -->

<!-- wp:paragraph -->

**Github 项目地址：**<a href="https://github.com/sy-records/wordpress-qcloud-cos" target="_blank" rel="noopener" data-schema-attribute="">https://github.com/sy-records/wordpress-qcloud-cos</a>

<!-- /wp:paragraph -->

<!-- wp:heading {"level":4} -->

#### 插件特点 {#插件特点}

<!-- /wp:heading -->

<!-- wp:list {"ordered":true,"backgroundColor":"vivid-cyan-blue","textColor":"white"} -->

<ol class="has-white-color has-vivid-cyan-blue-background-color has-text-color has-background">
  <li>
    可配置是否上传缩略图和是否保留本地备份
  </li>
  <li>
    本地删除可同步删除腾讯云对象存储 COS 中的文件
  </li>
  <li>
    支持腾讯云 COS 存储桶绑定自定义域名
  </li>
  <li>
    支持替换数据库中旧的资源链接地址
  </li>
  <li>
    支持北京、上海、广州、香港、法兰克福等完整地域使用
  </li>
  <li>
    支持同步历史附件到 COS
  </li>
  <li>
    支持验证桶名是否填写正确
  </li>
  <li>
    更多功能正在路上…
  </li>
</ol>

<!-- /wp:list -->

<!-- wp:heading -->

## Github 作为免费图床 {#github-作为免费图床}

<!-- /wp:heading -->

<!-- wp:paragraph -->

Github 项目地址: <a class="wp-editor-md-post-content-link" title="https://github.com/niqingyang/wp-github-gos" href="https://github.com/niqingyang/wp-github-gos" target="_blank" rel="nofollow noopener" data-schema-attribute="">https://github.com/niqingyang/wp-github-gos</a>

<!-- /wp:paragraph -->

<!-- wp:heading {"level":4} -->

#### 插件特色 {#插件特色}

<!-- /wp:heading -->

<!-- wp:list {"backgroundColor":"vivid-cyan-blue","textColor":"white"} -->

<ul class="has-white-color has-vivid-cyan-blue-background-color has-text-color has-background">
  <li>
    使用 GitHub 仓库存储 WordPress 站点图片等多媒体文件
  </li>
  <li>
    可配置是否上传缩略图和是否保留本地备份
  </li>
  <li>
    本地删除可同步删除腾讯云上面的文件
  </li>
  <li>
    支持替换数据库中旧的资源链接地址
  </li>
  <li>
    支持在图片链接地址后面自定义拼接图片<code>宽度</code>、<code>高度</code>、<code>大小</code>三个参数
  </li>
  <li>
    建议使用 jsdelivr 免费加速 github 下的图片，速度还是很可以的
  </li>
</ul>

<!-- /wp:list -->

<!-- wp:heading {"level":4} -->

#### 插件缺点 {#插件缺点}

<!-- /wp:heading -->

<!-- wp:list -->

*   使用 Github API 同步图片等附件的时候速度相较于国内的免费图床比较慢
*   未来不知道会不会被屏蔽

<!-- /wp:list -->

<!-- wp:paragraph -->

感谢以上作者的辛勤付出，有需求的小伙伴自取。

<!-- /wp:paragraph -->

<!-- wp:heading -->

## 华为云OBS {#华为云obs}

<!-- /wp:heading -->

<!-- wp:paragraph -->

<a href="https://github.com/sy-records/huaweicloud-obs-wordpress" target="_blank" rel="noopener">GitHub</a>，<a href="https://wordpress.org/plugins/obs-huaweicloud" target="_blank" rel="noopener">WordPress Plugins</a>

<!-- /wp:paragraph -->

<!-- wp:heading -->

## 七牛云KODO {#七牛云kodo}

<!-- /wp:heading -->

<!-- wp:paragraph -->

<a href="https://github.com/sy-records/qiniu-kodo-wordpress" target="_blank" rel="noopener">GitHub</a>，<a href="https://wordpress.org/plugins/kodo-qiniu" target="_blank" rel="noopener">WordPress Plugins</a>

<!-- /wp:paragraph -->

<!-- wp:heading -->

## 又拍云USS {#又拍云uss}

<!-- /wp:heading -->

<!-- wp:paragraph -->

<a href="https://github.com/sy-records/upyun-uss-wordpress" target="_blank" rel="noopener">GitHub</a>，<a href="https://wordpress.org/plugins/uss-upyun" target="_blank" rel="noopener">WordPress Plugins</a>

<!-- /wp:paragraph -->