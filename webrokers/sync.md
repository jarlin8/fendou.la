---
title: 产品页面相关配置syncBlock
post_status: 
skip_file: yes
comment_status: closed
custom_fields:
  rank_math_title: 不同步
  _review_post_pros_text: |
    无
  _review_post_cons_text: |
    无
post_excerpt: 简码备忘
---
<details><summary>wordpress多站点无法新建站点</summary>

<li>和报错需要清理cookies一样的原因</li>
<li>wp-config.php里面<code>define( 'SUBDOMAIN_INSTALL', false );//子域名安装</code></li>
<li>新建子站点是用<code>define( 'SUBDOMAIN_INSTALL', true);//子域名安装</code> 完成以后，改成<code>false</code></li>
</details>

<details><summary>站点升级和相关版本问题</summary>

<p>wordpress：5.9.9
woocommerce：7.5.1
出现问题的地方：主题选项里面>><strong>Product layout >>compact style</strong></p>
<p>如何出现没有用过的字段 导致无法保存。先导出配置 然后进行修改，后面再次恢复即可。</p>
<p>出现部分字段无法显示时，需要返回默认布局后，对产品进行保存就好了。</p>
<p></p>
</details>

优点：`_review_post_pros_text`

缺点：`_review_post_cons_text`

<details><summary>图片展示使用位置</summary>

<img src="https://prod-files-secure.s3.us-west-2.amazonaws.com/39ed1227-6d7d-4570-be36-9ccd4a2c4241/f51d3d83-55d4-4bdf-9604-f37ec77ab556/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45HZZMZUHI%2F20240503%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20240503T165513Z&X-Amz-Expires=3600&X-Amz-Signature=c15d5c267069025b8fa320751b45987544eb0243aae54bc23a15610ebf552624&X-Amz-SignedHeaders=host&x-id=GetObject" alt="Image">
</details>

SEO标题：`rank_math_title`

`TMGM测评 %currentyear% 开户必看 %sep% %sitename%`

SEO关键字：`rank_math_focus_keyword`

一句话总结：`_review_post_summary_text`

<details><summary>图片展示使用位置</summary>

<img src="https://prod-files-secure.s3.us-west-2.amazonaws.com/39ed1227-6d7d-4570-be36-9ccd4a2c4241/4b96a922-296c-4f4e-8630-d1c870cbce01/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45HZZMZUHI%2F20240503%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20240503T165513Z&X-Amz-Expires=3600&X-Amz-Signature=2b194514136d69c811a4cb295ee55fce3b37e09a0f998ef8e8a662b690444b44&X-Amz-SignedHeaders=host&x-id=GetObject" alt="Image">
</details>

平台亮点 用于SEO展示 **摘要**：`post_excerpt`  等价于 `rank_math_description`

<details><summary>图片展示使用位置</summary>

<img src="https://prod-files-secure.s3.us-west-2.amazonaws.com/39ed1227-6d7d-4570-be36-9ccd4a2c4241/1ee11f63-b60a-4dfe-a7a7-d58ff23b5d88/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45HZZMZUHI%2F20240503%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20240503T165513Z&X-Amz-Expires=3600&X-Amz-Signature=628c2cc0f5c21d68433e84a72f21285db4cdb511a7e47ee1662b606af862c62e&X-Amz-SignedHeaders=host&x-id=GetObject" alt="Image">
<img src="https://prod-files-secure.s3.us-west-2.amazonaws.com/39ed1227-6d7d-4570-be36-9ccd4a2c4241/ad4118b5-78d8-4fbe-801e-3b29b5d99c01/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45HZZMZUHI%2F20240503%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20240503T165513Z&X-Amz-Expires=3600&X-Amz-Signature=cddf784e589123a6cd7745b8f982b05b96cd3da908ba294e64c66099cb0dd593&X-Amz-SignedHeaders=host&x-id=GetObject" alt="Image">
<img src="https://prod-files-secure.s3.us-west-2.amazonaws.com/39ed1227-6d7d-4570-be36-9ccd4a2c4241/a38cf7c9-a79c-4b64-9e94-13589fe0758b/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45HZZMZUHI%2F20240503%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20240503T165513Z&X-Amz-Expires=3600&X-Amz-Signature=c0d50278db355392e63df1bbe45cb20acb6256bf8afd54390099332e652bcf8f&X-Amz-SignedHeaders=host&x-id=GetObject" alt="Image">
<img src="https://prod-files-secure.s3.us-west-2.amazonaws.com/39ed1227-6d7d-4570-be36-9ccd4a2c4241/7da6fc1e-d2ac-42ae-8c75-cb5749aa18f6/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45HZZMZUHI%2F20240503%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20240503T165513Z&X-Amz-Expires=3600&X-Amz-Signature=b9ea04302f2397bb0caae70d6fd9d8e3b4cab21a15227d526d1603a8f5d35d53&X-Amz-SignedHeaders=host&x-id=GetObject" alt="Image">
<img src="https://prod-files-secure.s3.us-west-2.amazonaws.com/39ed1227-6d7d-4570-be36-9ccd4a2c4241/7e97f40a-eaee-47f5-b2f9-475f96808fa7/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45HZZMZUHI%2F20240503%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20240503T165513Z&X-Amz-Expires=3600&X-Amz-Signature=ae307f632ae57c08183936cb057b375c2a12d30fd3ae45e07fa4ddcd054b7b95&X-Amz-SignedHeaders=host&x-id=GetObject" alt="Image">
</details>

head：`_review_heading`

<details><summary>图片展示使用位置</summary>

<img src="https://prod-files-secure.s3.us-west-2.amazonaws.com/39ed1227-6d7d-4570-be36-9ccd4a2c4241/3a4650ad-9887-415c-889a-edd51fa54f27/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45HZZMZUHI%2F20240503%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20240503T165514Z&X-Amz-Expires=3600&X-Amz-Signature=667f09880dc03764056fba1a34342ace95a9d5d9df5239d110dcfb6ac1cd4f21&X-Amz-SignedHeaders=host&x-id=GetObject" alt="Image">
</details>

`rehub_woodeals_short`	field to store custom code areas near Short content section. It supports also shortcodes



## 简码使用

### 经纪商详细展示

<details><summary>常用经纪商ID列表</summary>

<pre><code class="php">嘉盛 ===> 20641  [wpsm_woobox id="20641" title="嘉盛"]
易信easymarkets ===> 11542  [wpsm_woobox id="11542" title="易信easymarkets"]
ATFX外汇 ===> 10424  [wpsm_woobox id="10424" title="ATFX"]
XM ===> 10406  [wpsm_woobox id="10406" title="XM"]
TMGM ===> 29622  [wpsm_woobox id="29622" title="TMGM"]
HYCM ===> 10447  [wpsm_woobox id="10447" title="HYCM"]
fpmarkets澳福外汇 ===> 20639  [wpsm_woobox id="20639" title="fpmarkets澳福外汇"]</code></pre>
</details>

`[wpsm_woobox id="10406" title="XM"]` **不需要加引号**

![Image](https://prod-files-secure.s3.us-west-2.amazonaws.com/39ed1227-6d7d-4570-be36-9ccd4a2c4241/4f898f9d-0fa7-4e43-acd3-ac6bc7be575a/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45HZZMZUHI%2F20240503%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20240503T165512Z&X-Amz-Expires=3600&X-Amz-Signature=f831eabd96d36e8dc642b427283a5c5880a1e801c1024dfe0c144490865ccf19&X-Amz-SignedHeaders=host&x-id=GetObject)

### 单个推荐
`[wpsm_top postid="20641,10424,11542,10447,10406,28706" title="平台推荐列表"]`

[wpsm_top postid="10424" title="ATFX CTA"]

![Image](https://prod-files-secure.s3.us-west-2.amazonaws.com/39ed1227-6d7d-4570-be36-9ccd4a2c4241/5ac620dc-51a8-48b6-b55d-91f47299193c/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45HZZMZUHI%2F20240503%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20240503T165512Z&X-Amz-Expires=3600&X-Amz-Signature=b315fa70206063e3803249a332d4f6e32972a2dca212fb081ae661cc3c225cba&X-Amz-SignedHeaders=host&x-id=GetObject)

详情对比

`[wpsm_woocharts ids="20641,10406,10424" disable="brand,stock,userrate,review"]`

![Image](https://prod-files-secure.s3.us-west-2.amazonaws.com/39ed1227-6d7d-4570-be36-9ccd4a2c4241/bf3ba45f-b9f3-4295-8aef-b4a495fd25f4/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45HZZMZUHI%2F20240503%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20240503T165512Z&X-Amz-Expires=3600&X-Amz-Signature=6b9d8ec4fa927966ab77f61ab1eb997dc1073d1fdfa644ccfa10eb3b5e7623f2&X-Amz-SignedHeaders=host&x-id=GetObject)

![Image](https://prod-files-secure.s3.us-west-2.amazonaws.com/39ed1227-6d7d-4570-be36-9ccd4a2c4241/30bc56ef-f383-4b48-9768-2ebc9e436ec0/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45HZZMZUHI%2F20240503%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20240503T165512Z&X-Amz-Expires=3600&X-Amz-Signature=b772d52d99276107c91255ef047ade780ddcecc974a8fda96bb356650b9bb6eb&X-Amz-SignedHeaders=host&x-id=GetObject)

## sync同步模块

### PROs CONs对照表

| <img src="https://cdn.ifttt.fun/gh/jarlin8/OSS@main/icons/customize/pros.svg" height="auto" width="37.3%"> | <img src="https://cdn.ifttt.fun/gh/jarlin8/OSS@main/icons/customize/cons.svg" height="auto" width="28.8%"> |
| :--- | :--- |
| 优点 | 缺点 |

![Image](https://prod-files-secure.s3.us-west-2.amazonaws.com/39ed1227-6d7d-4570-be36-9ccd4a2c4241/8742b755-dfb5-4004-9a5f-d6e561664bd8/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45HZZMZUHI%2F20240503%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20240503T165512Z&X-Amz-Expires=3600&X-Amz-Signature=ff4ed63f63a480441ab2d32917853d3e8beaa9a00fb1093bf2b75751dea6995e&X-Amz-SignedHeaders=host&x-id=GetObject)

| <img src="https://cdn.ifttt.fun/gh/jarlin8/OSS@main/icons/customize/pros1.svg" height="auto"> | <img src="https://cdn.ifttt.fun/gh/jarlin8/OSS@main/icons/customize/cons1.svg" height="auto"> |
| :--- | :--- |
| 优点 | 缺点 |

![Image](https://prod-files-secure.s3.us-west-2.amazonaws.com/39ed1227-6d7d-4570-be36-9ccd4a2c4241/806358f8-c9c4-4e17-bb35-c6c76a5397a5/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45HZZMZUHI%2F20240503%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20240503T165512Z&X-Amz-Expires=3600&X-Amz-Signature=d86323a42cb68daecc26866e7358acce1a7bd3684c7d87a7fa38898d9830a9a0&X-Amz-SignedHeaders=host&x-id=GetObject)

| <img src="https://cdn.ifttt.fun/gh/jarlin8/OSS@main/icons/customize/pros2.svg" height="auto"> | <img src="https://cdn.ifttt.fun/gh/jarlin8/OSS@main/icons/customize/cons2.svg" height="auto"> |
| :--- | :--- |
| 优点 | 缺点 |

![Image](https://prod-files-secure.s3.us-west-2.amazonaws.com/39ed1227-6d7d-4570-be36-9ccd4a2c4241/a9245ec9-70dd-4005-b534-0d54315fc5f3/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45HZZMZUHI%2F20240503%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20240503T165512Z&X-Amz-Expires=3600&X-Amz-Signature=10f3f275b868cdc2f740960475c66e3016e001081c74a4f66f8aefec4068369c&X-Amz-SignedHeaders=host&x-id=GetObject)

| <img src="https://cdn.ifttt.fun/gh/jarlin8/OSS@main/icons/customize/pros3.svg" height="auto"> | <img src="https://cdn.ifttt.fun/gh/jarlin8/OSS@main/icons/customize/cons3.svg" height="auto"> |
| :--- | :--- |
| 优点 | 缺点 |

![Image](https://prod-files-secure.s3.us-west-2.amazonaws.com/39ed1227-6d7d-4570-be36-9ccd4a2c4241/e1e580a2-2e5c-4780-9ff4-19c318fc2284/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45HZZMZUHI%2F20240503%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20240503T165512Z&X-Amz-Expires=3600&X-Amz-Signature=d4a712b04b26ec61dffe16bfbb9db4a1e4bc0b3cafb7e676c5cf44904871263d&X-Amz-SignedHeaders=host&x-id=GetObject)