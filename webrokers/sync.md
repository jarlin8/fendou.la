---
title: ""
post_status: ""
skip_file: "yes"
post_date: "2024-01-14T01:22:00.000Z"
taxonomy:
  category:

  post_tag:

post_excerpt: "简码备忘"
---
<details><summary>wordpress多站点无法新建站点</summary>

* 和报错需要清理cookies一样的原因

* wp-config.php里面`define( 'SUBDOMAIN_INSTALL', false );//子域名安装`

* 新建子站点是用`define( 'SUBDOMAIN_INSTALL', true);//子域名安装` 完成以后，改成`false`
</details>

<details><summary>站点升级和相关版本问题</summary>

wordpress：5.9.9
woocommerce：7.5.1
出现问题的地方：主题选项里面>>**Product layout >>compact style**

如何出现没有用过的字段 导致无法保存。先导出配置 然后进行修改，后面再次恢复即可。

出现部分字段无法显示时，需要返回默认布局后，对产品进行保存就好了。
</details>

优点：**`_review_post_pros_text`**

缺点：**`_review_post_cons_text`**

<details><summary>图片展示使用位置</summary>

![image](https://cdn.jsdmirror.com/gh/jarlin8/fendou.la@main/webrokers/images/2fd5702f6c9b2c13b81b2fba248fbfc1.png)
</details>

SEO标题：`rank_math_title`

`TMGM测评 %currentyear% 开户必看 %sep% %sitename%`

SEO关键字：`rank_math_focus_keyword`

一句话总结：`_review_post_summary_text`

<details><summary>图片展示使用位置</summary>

![image](https://cdn.jsdmirror.com/gh/jarlin8/fendou.la@main/webrokers/images/2823c5e6c9f5460081e8cef5a96b622a.png)
</details>

平台亮点 用于SEO展示 **摘要**：`post_excerpt`  等价于 `rank_math_description`

<details><summary>图片展示使用位置</summary>

![image](https://cdn.jsdmirror.com/gh/jarlin8/fendou.la@main/webrokers/images/29cd85662f0f070994e195139654e687.png)

![image](https://cdn.jsdmirror.com/gh/jarlin8/fendou.la@main/webrokers/images/e10f774759e2ba4e27f5b6f523cf1bf9.png)

![image](https://cdn.jsdmirror.com/gh/jarlin8/fendou.la@main/webrokers/images/7494054dafd4e614b0f8093b2f10621b.png)

![image](https://cdn.jsdmirror.com/gh/jarlin8/fendou.la@main/webrokers/images/b37f8a654db05f11236b72144c5efac3.png)

![image](https://cdn.jsdmirror.com/gh/jarlin8/fendou.la@main/webrokers/images/40352ffc42467c4aa2a5a2333467998f.png)
</details>

head：**`_review_heading`**

<details><summary>图片展示使用位置</summary>

![image](https://cdn.jsdmirror.com/gh/jarlin8/fendou.la@main/webrokers/images/acd00662b1d912864730cb36d51616fe.png)
</details>

`rehub_woodeals_short`	field to store custom code areas near Short content section. It supports also shortcodes

## 简码使用

### 经纪商详细展示

<details><summary>常用经纪商ID列表</summary>

```php
嘉盛 ===> 20641  [wpsm_woobox id="20641" title="嘉盛"]
易信easymarkets ===> 11542  [wpsm_woobox id="11542" title="易信easymarkets"]
ATFX外汇 ===> 10424  [wpsm_woobox id="10424" title="ATFX"]
XM ===> 10406  [wpsm_woobox id="10406" title="XM"]
TMGM ===> 29622  [wpsm_woobox id="29622" title="TMGM"]
HYCM ===> 10447  [wpsm_woobox id="10447" title="HYCM"]
fpmarkets澳福外汇 ===> 20639  [wpsm_woobox id="20639" title="fpmarkets澳福外汇"]
```
</details>

`[wpsm_woobox id="10406" title="XM"]` <span style="color:orange_background">**不需要加引号**</span>

![image](https://cdn.jsdmirror.com/gh/jarlin8/fendou.la@main/webrokers/images/83f8ffbf6c84d397ad4f61c09547996b.png)

### 单个推荐
`[wpsm_top postid="20641,10424,11542,10447,10406,28706" title="平台推荐列表"]`

[wpsm_top postid="10424" title="ATFX CTA"]

![image](https://cdn.jsdmirror.com/gh/jarlin8/fendou.la@main/webrokers/images/5b5f3fb2827cc4b0d42301d58366c5f0.png)

详情对比

`[wpsm_woocharts ids="20641,10406,10424" disable="brand,stock,userrate,review"]`

![image](https://cdn.jsdmirror.com/gh/jarlin8/fendou.la@main/webrokers/images/70ed738aafb3e30c16f84536439ef0b0.png)

![image](https://cdn.jsdmirror.com/gh/jarlin8/fendou.la@main/webrokers/images/12fe288e7bd450b310b1887e03f7cfae.png)

## sync同步模块

### PROs CONs对照表

| <img src="https://cdn.ifttt.fun/gh/jarlin8/OSS@main/icons/customize/pros.svg" height="auto" width="37.3%"> | <img src="https://cdn.ifttt.fun/gh/jarlin8/OSS@main/icons/customize/cons.svg" height="auto" width="28.8%"> |
| :--- | :--- |
| 优点 | 缺点 |

![image](https://cdn.jsdmirror.com/gh/jarlin8/fendou.la@main/webrokers/images/ec8143bf40cfa651f347e7827856884b.png)

| <img src="https://cdn.ifttt.fun/gh/jarlin8/OSS@main/icons/customize/pros1.svg" height="auto"> | <img src="https://cdn.ifttt.fun/gh/jarlin8/OSS@main/icons/customize/cons1.svg" height="auto"> |
| :--- | :--- |
| 优点 | 缺点 |

![image](https://cdn.jsdmirror.com/gh/jarlin8/fendou.la@main/webrokers/images/79513a5ea753c39444560a4461b14aba.png)

| <img src="https://cdn.ifttt.fun/gh/jarlin8/OSS@main/icons/customize/pros2.svg" height="auto"> | <img src="https://cdn.ifttt.fun/gh/jarlin8/OSS@main/icons/customize/cons2.svg" height="auto"> |
| :--- | :--- |
| 优点 | 缺点 |

![image](https://cdn.jsdmirror.com/gh/jarlin8/fendou.la@main/webrokers/images/ed432e5a7dcaa30a1e7aad2b439055a0.png)

| <img src="https://cdn.ifttt.fun/gh/jarlin8/OSS@main/icons/customize/pros3.svg" height="auto"> | <img src="https://cdn.ifttt.fun/gh/jarlin8/OSS@main/icons/customize/cons3.svg" height="auto"> |
| :--- | :--- |
| 优点 | 缺点 |

![image](https://cdn.jsdmirror.com/gh/jarlin8/fendou.la@main/webrokers/images/2fe8013647023e7daae985b420c749b8.png)