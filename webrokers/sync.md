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

<img src="https://prod-files-secure.s3.us-west-2.amazonaws.com/39ed1227-6d7d-4570-be36-9ccd4a2c4241/f51d3d83-55d4-4bdf-9604-f37ec77ab556/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45HZZMZUHI%2F20240910%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20240910T045517Z&X-Amz-Expires=3600&X-Amz-Signature=9bb5b9b6cf472285c083f347e78b3a0485a4f5815a67993776cb871d509288cf&X-Amz-SignedHeaders=host&x-id=GetObject" alt="Image">
</details>

SEO标题：`rank_math_title`

`TMGM测评 %currentyear% 开户必看 %sep% %sitename%`

SEO关键字：`rank_math_focus_keyword`

一句话总结：`_review_post_summary_text`

<details><summary>图片展示使用位置</summary>

<img src="https://prod-files-secure.s3.us-west-2.amazonaws.com/39ed1227-6d7d-4570-be36-9ccd4a2c4241/4b96a922-296c-4f4e-8630-d1c870cbce01/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45HZZMZUHI%2F20240910%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20240910T045517Z&X-Amz-Expires=3600&X-Amz-Signature=a75987928a9c70b7981be816c30473fc6f5edb81a49597d498befe45f2c59be0&X-Amz-SignedHeaders=host&x-id=GetObject" alt="Image">
</details>

平台亮点 用于SEO展示 **摘要**：`post_excerpt`  等价于 `rank_math_description`

<details><summary>图片展示使用位置</summary>

<img src="https://prod-files-secure.s3.us-west-2.amazonaws.com/39ed1227-6d7d-4570-be36-9ccd4a2c4241/1ee11f63-b60a-4dfe-a7a7-d58ff23b5d88/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45HZZMZUHI%2F20240910%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20240910T045518Z&X-Amz-Expires=3600&X-Amz-Signature=470e5e6676059704a9292fb20a695a102816c964bd0f7693e37d3c45c946a8f7&X-Amz-SignedHeaders=host&x-id=GetObject" alt="Image">
<img src="https://prod-files-secure.s3.us-west-2.amazonaws.com/39ed1227-6d7d-4570-be36-9ccd4a2c4241/ad4118b5-78d8-4fbe-801e-3b29b5d99c01/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45HZZMZUHI%2F20240910%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20240910T045518Z&X-Amz-Expires=3600&X-Amz-Signature=8d7610c29cd98a14d2100addb2bd927adcb86ab5568e8bc9b26dd54aed907005&X-Amz-SignedHeaders=host&x-id=GetObject" alt="Image">
<img src="https://prod-files-secure.s3.us-west-2.amazonaws.com/39ed1227-6d7d-4570-be36-9ccd4a2c4241/a38cf7c9-a79c-4b64-9e94-13589fe0758b/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45HZZMZUHI%2F20240910%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20240910T045518Z&X-Amz-Expires=3600&X-Amz-Signature=593b7ffbc6c54aaa45eff36f9d6cb8e98c87165b9524bc20f7047686822185dc&X-Amz-SignedHeaders=host&x-id=GetObject" alt="Image">
<img src="https://prod-files-secure.s3.us-west-2.amazonaws.com/39ed1227-6d7d-4570-be36-9ccd4a2c4241/7da6fc1e-d2ac-42ae-8c75-cb5749aa18f6/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45HZZMZUHI%2F20240910%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20240910T045518Z&X-Amz-Expires=3600&X-Amz-Signature=0c2133cf37dc8267c17771057afc9c5ffbf59a85cf8f97ce2dc7d9fcffbe5ad6&X-Amz-SignedHeaders=host&x-id=GetObject" alt="Image">
<img src="https://prod-files-secure.s3.us-west-2.amazonaws.com/39ed1227-6d7d-4570-be36-9ccd4a2c4241/7e97f40a-eaee-47f5-b2f9-475f96808fa7/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45HZZMZUHI%2F20240910%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20240910T045518Z&X-Amz-Expires=3600&X-Amz-Signature=f1dd11cbe97927a95e2ea833f19bfe72e14cd5dbc626064c471f2b7927fe9e46&X-Amz-SignedHeaders=host&x-id=GetObject" alt="Image">
</details>

head：`_review_heading`

<details><summary>图片展示使用位置</summary>

<img src="https://prod-files-secure.s3.us-west-2.amazonaws.com/39ed1227-6d7d-4570-be36-9ccd4a2c4241/3a4650ad-9887-415c-889a-edd51fa54f27/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45HZZMZUHI%2F20240910%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20240910T045518Z&X-Amz-Expires=3600&X-Amz-Signature=4db21fc8e133100b7d46ca96f118013a9fadb6c86f1bb2341a6321fdcc23ef3a&X-Amz-SignedHeaders=host&x-id=GetObject" alt="Image">
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

![Image](https://prod-files-secure.s3.us-west-2.amazonaws.com/39ed1227-6d7d-4570-be36-9ccd4a2c4241/4f898f9d-0fa7-4e43-acd3-ac6bc7be575a/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45HZZMZUHI%2F20240910%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20240910T045516Z&X-Amz-Expires=3600&X-Amz-Signature=e3cca58e76f57dc6fa5672af6b61730470237eedf7b581dcb817248e17d5291c&X-Amz-SignedHeaders=host&x-id=GetObject)

### 单个推荐
`[wpsm_top postid="20641,10424,11542,10447,10406,28706" title="平台推荐列表"]`

[wpsm_top postid="10424" title="ATFX CTA"]

![Image](https://prod-files-secure.s3.us-west-2.amazonaws.com/39ed1227-6d7d-4570-be36-9ccd4a2c4241/5ac620dc-51a8-48b6-b55d-91f47299193c/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45HZZMZUHI%2F20240910%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20240910T045516Z&X-Amz-Expires=3600&X-Amz-Signature=99a589996a9dc018a891e5d58c8cf25ab79027a61ff84ab40f05ce7ab1b6e3dc&X-Amz-SignedHeaders=host&x-id=GetObject)

详情对比

`[wpsm_woocharts ids="20641,10406,10424" disable="brand,stock,userrate,review"]`

![Image](https://prod-files-secure.s3.us-west-2.amazonaws.com/39ed1227-6d7d-4570-be36-9ccd4a2c4241/bf3ba45f-b9f3-4295-8aef-b4a495fd25f4/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45HZZMZUHI%2F20240910%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20240910T045516Z&X-Amz-Expires=3600&X-Amz-Signature=c4b5272406d66313bf00c336ea8f17b4c439e1c5901907608fe956ecfe6471a1&X-Amz-SignedHeaders=host&x-id=GetObject)

![Image](https://prod-files-secure.s3.us-west-2.amazonaws.com/39ed1227-6d7d-4570-be36-9ccd4a2c4241/30bc56ef-f383-4b48-9768-2ebc9e436ec0/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45HZZMZUHI%2F20240910%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20240910T045516Z&X-Amz-Expires=3600&X-Amz-Signature=df098af8df78b7e32aa6df97d932a1e47d429648cb467ab8032a5be3e554c18b&X-Amz-SignedHeaders=host&x-id=GetObject)

## sync同步模块

### PROs CONs对照表

| <img src="https://cdn.ifttt.fun/gh/jarlin8/OSS@main/icons/customize/pros.svg" height="auto" width="37.3%"> | <img src="https://cdn.ifttt.fun/gh/jarlin8/OSS@main/icons/customize/cons.svg" height="auto" width="28.8%"> |
| :--- | :--- |
| 优点 | 缺点 |

![Image](https://prod-files-secure.s3.us-west-2.amazonaws.com/39ed1227-6d7d-4570-be36-9ccd4a2c4241/8742b755-dfb5-4004-9a5f-d6e561664bd8/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45HZZMZUHI%2F20240910%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20240910T045516Z&X-Amz-Expires=3600&X-Amz-Signature=bc3c6137be344cee08253049a4cb52a45ab39e1fbc55f9e8df46f4ad08bed134&X-Amz-SignedHeaders=host&x-id=GetObject)

| <img src="https://cdn.ifttt.fun/gh/jarlin8/OSS@main/icons/customize/pros1.svg" height="auto"> | <img src="https://cdn.ifttt.fun/gh/jarlin8/OSS@main/icons/customize/cons1.svg" height="auto"> |
| :--- | :--- |
| 优点 | 缺点 |

![Image](https://prod-files-secure.s3.us-west-2.amazonaws.com/39ed1227-6d7d-4570-be36-9ccd4a2c4241/806358f8-c9c4-4e17-bb35-c6c76a5397a5/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45HZZMZUHI%2F20240910%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20240910T045516Z&X-Amz-Expires=3600&X-Amz-Signature=3c5f3acfca5522e0197c27e828fd8227f6a6d0d942d2d618b80b5919321e1562&X-Amz-SignedHeaders=host&x-id=GetObject)

| <img src="https://cdn.ifttt.fun/gh/jarlin8/OSS@main/icons/customize/pros2.svg" height="auto"> | <img src="https://cdn.ifttt.fun/gh/jarlin8/OSS@main/icons/customize/cons2.svg" height="auto"> |
| :--- | :--- |
| 优点 | 缺点 |

![Image](https://prod-files-secure.s3.us-west-2.amazonaws.com/39ed1227-6d7d-4570-be36-9ccd4a2c4241/a9245ec9-70dd-4005-b534-0d54315fc5f3/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45HZZMZUHI%2F20240910%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20240910T045516Z&X-Amz-Expires=3600&X-Amz-Signature=e4bf08839f9f1b60b799f8137b7b87cb7ba41bcdfa2f9bd1f768fee2a463ce04&X-Amz-SignedHeaders=host&x-id=GetObject)

| <img src="https://cdn.ifttt.fun/gh/jarlin8/OSS@main/icons/customize/pros3.svg" height="auto"> | <img src="https://cdn.ifttt.fun/gh/jarlin8/OSS@main/icons/customize/cons3.svg" height="auto"> |
| :--- | :--- |
| 优点 | 缺点 |

![Image](https://prod-files-secure.s3.us-west-2.amazonaws.com/39ed1227-6d7d-4570-be36-9ccd4a2c4241/e1e580a2-2e5c-4780-9ff4-19c318fc2284/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45HZZMZUHI%2F20240910%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20240910T045516Z&X-Amz-Expires=3600&X-Amz-Signature=ad985060d4ce1034503a942d3f08e9d7079f7b156d2e7275b63850dc0ad4aa73&X-Amz-SignedHeaders=host&x-id=GetObject)