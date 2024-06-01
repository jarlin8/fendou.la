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

<img src="https://prod-files-secure.s3.us-west-2.amazonaws.com/39ed1227-6d7d-4570-be36-9ccd4a2c4241/f51d3d83-55d4-4bdf-9604-f37ec77ab556/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45HZZMZUHI%2F20240601%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20240601T225514Z&X-Amz-Expires=3600&X-Amz-Signature=49768191e72a9f50ca273efacc166ddfbedc97ec585cd00f49ad78fd6e946a13&X-Amz-SignedHeaders=host&x-id=GetObject" alt="Image">
</details>

SEO标题：`rank_math_title`

`TMGM测评 %currentyear% 开户必看 %sep% %sitename%`

SEO关键字：`rank_math_focus_keyword`

一句话总结：`_review_post_summary_text`

<details><summary>图片展示使用位置</summary>

<img src="https://prod-files-secure.s3.us-west-2.amazonaws.com/39ed1227-6d7d-4570-be36-9ccd4a2c4241/4b96a922-296c-4f4e-8630-d1c870cbce01/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45HZZMZUHI%2F20240601%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20240601T225515Z&X-Amz-Expires=3600&X-Amz-Signature=21b9cb52e6ee099f21724e55547009246441614ccec47672c0d08f0a4bc0b8cf&X-Amz-SignedHeaders=host&x-id=GetObject" alt="Image">
</details>

平台亮点 用于SEO展示 **摘要**：`post_excerpt`  等价于 `rank_math_description`

<details><summary>图片展示使用位置</summary>

<img src="https://prod-files-secure.s3.us-west-2.amazonaws.com/39ed1227-6d7d-4570-be36-9ccd4a2c4241/1ee11f63-b60a-4dfe-a7a7-d58ff23b5d88/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45HZZMZUHI%2F20240601%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20240601T225515Z&X-Amz-Expires=3600&X-Amz-Signature=f4d4b03a16156107ba4f17e2cee2bc82ff532119ca0ec4269dc1d382a0a09f05&X-Amz-SignedHeaders=host&x-id=GetObject" alt="Image">
<img src="https://prod-files-secure.s3.us-west-2.amazonaws.com/39ed1227-6d7d-4570-be36-9ccd4a2c4241/ad4118b5-78d8-4fbe-801e-3b29b5d99c01/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45HZZMZUHI%2F20240601%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20240601T225515Z&X-Amz-Expires=3600&X-Amz-Signature=a111b67ef9eea68a0485f4f50e7a55c903dbf095763a8cb43c239636961f88a2&X-Amz-SignedHeaders=host&x-id=GetObject" alt="Image">
<img src="https://prod-files-secure.s3.us-west-2.amazonaws.com/39ed1227-6d7d-4570-be36-9ccd4a2c4241/a38cf7c9-a79c-4b64-9e94-13589fe0758b/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45HZZMZUHI%2F20240601%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20240601T225515Z&X-Amz-Expires=3600&X-Amz-Signature=834fb85c0ddaa0564b962e6b7d8f4a0155608c2b2d51d530d68d583f713c4405&X-Amz-SignedHeaders=host&x-id=GetObject" alt="Image">
<img src="https://prod-files-secure.s3.us-west-2.amazonaws.com/39ed1227-6d7d-4570-be36-9ccd4a2c4241/7da6fc1e-d2ac-42ae-8c75-cb5749aa18f6/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45HZZMZUHI%2F20240601%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20240601T225515Z&X-Amz-Expires=3600&X-Amz-Signature=11212bddfcd1e7fe2217bd00c8eda67c9869cc1ce2ac47766a52ed232b10a93e&X-Amz-SignedHeaders=host&x-id=GetObject" alt="Image">
<img src="https://prod-files-secure.s3.us-west-2.amazonaws.com/39ed1227-6d7d-4570-be36-9ccd4a2c4241/7e97f40a-eaee-47f5-b2f9-475f96808fa7/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45HZZMZUHI%2F20240601%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20240601T225515Z&X-Amz-Expires=3600&X-Amz-Signature=d07068ec8fa4296fb7906c4a1216f488f1203d19578b044fbaa575642a422362&X-Amz-SignedHeaders=host&x-id=GetObject" alt="Image">
</details>

head：`_review_heading`

<details><summary>图片展示使用位置</summary>

<img src="https://prod-files-secure.s3.us-west-2.amazonaws.com/39ed1227-6d7d-4570-be36-9ccd4a2c4241/3a4650ad-9887-415c-889a-edd51fa54f27/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45HZZMZUHI%2F20240601%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20240601T225515Z&X-Amz-Expires=3600&X-Amz-Signature=72f8fe8291084059539c1cf0a1acf0e775ef1fcf92b11d97f2bf9e2e108d2d60&X-Amz-SignedHeaders=host&x-id=GetObject" alt="Image">
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

![Image](https://prod-files-secure.s3.us-west-2.amazonaws.com/39ed1227-6d7d-4570-be36-9ccd4a2c4241/4f898f9d-0fa7-4e43-acd3-ac6bc7be575a/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45HZZMZUHI%2F20240601%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20240601T225513Z&X-Amz-Expires=3600&X-Amz-Signature=efcffe848a8b697644c4c8154469a32f485a389e7d7ee9e0671d0f9c90e91d2d&X-Amz-SignedHeaders=host&x-id=GetObject)

### 单个推荐
`[wpsm_top postid="20641,10424,11542,10447,10406,28706" title="平台推荐列表"]`

[wpsm_top postid="10424" title="ATFX CTA"]

![Image](https://prod-files-secure.s3.us-west-2.amazonaws.com/39ed1227-6d7d-4570-be36-9ccd4a2c4241/5ac620dc-51a8-48b6-b55d-91f47299193c/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45HZZMZUHI%2F20240601%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20240601T225513Z&X-Amz-Expires=3600&X-Amz-Signature=6c59808e14272dca5fb49435cfdbc86a25223ed4ea6e12e8bc26ad09f3c5423a&X-Amz-SignedHeaders=host&x-id=GetObject)

详情对比

`[wpsm_woocharts ids="20641,10406,10424" disable="brand,stock,userrate,review"]`

![Image](https://prod-files-secure.s3.us-west-2.amazonaws.com/39ed1227-6d7d-4570-be36-9ccd4a2c4241/bf3ba45f-b9f3-4295-8aef-b4a495fd25f4/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45HZZMZUHI%2F20240601%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20240601T225513Z&X-Amz-Expires=3600&X-Amz-Signature=25f7df0422446cf28587975cea1cdb85255727cf67619d78ac6c9681e877e895&X-Amz-SignedHeaders=host&x-id=GetObject)

![Image](https://prod-files-secure.s3.us-west-2.amazonaws.com/39ed1227-6d7d-4570-be36-9ccd4a2c4241/30bc56ef-f383-4b48-9768-2ebc9e436ec0/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45HZZMZUHI%2F20240601%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20240601T225513Z&X-Amz-Expires=3600&X-Amz-Signature=76508b2d8fe5015f17b1a0894b6ee65e7c00675d9b564ba4210f21085c3f2cae&X-Amz-SignedHeaders=host&x-id=GetObject)

## sync同步模块

### PROs CONs对照表

| <img src="https://cdn.ifttt.fun/gh/jarlin8/OSS@main/icons/customize/pros.svg" height="auto" width="37.3%"> | <img src="https://cdn.ifttt.fun/gh/jarlin8/OSS@main/icons/customize/cons.svg" height="auto" width="28.8%"> |
| :--- | :--- |
| 优点 | 缺点 |

![Image](https://prod-files-secure.s3.us-west-2.amazonaws.com/39ed1227-6d7d-4570-be36-9ccd4a2c4241/8742b755-dfb5-4004-9a5f-d6e561664bd8/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45HZZMZUHI%2F20240601%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20240601T225513Z&X-Amz-Expires=3600&X-Amz-Signature=a87c81e720b0dbace3bd259a800b15fda0516c85c65b42515186cf6dfd54607d&X-Amz-SignedHeaders=host&x-id=GetObject)

| <img src="https://cdn.ifttt.fun/gh/jarlin8/OSS@main/icons/customize/pros1.svg" height="auto"> | <img src="https://cdn.ifttt.fun/gh/jarlin8/OSS@main/icons/customize/cons1.svg" height="auto"> |
| :--- | :--- |
| 优点 | 缺点 |

![Image](https://prod-files-secure.s3.us-west-2.amazonaws.com/39ed1227-6d7d-4570-be36-9ccd4a2c4241/806358f8-c9c4-4e17-bb35-c6c76a5397a5/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45HZZMZUHI%2F20240601%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20240601T225513Z&X-Amz-Expires=3600&X-Amz-Signature=dd65db816eb985b1d353ad66d7b910c60a658fd4ddb4ff5343cc60857e6709a5&X-Amz-SignedHeaders=host&x-id=GetObject)

| <img src="https://cdn.ifttt.fun/gh/jarlin8/OSS@main/icons/customize/pros2.svg" height="auto"> | <img src="https://cdn.ifttt.fun/gh/jarlin8/OSS@main/icons/customize/cons2.svg" height="auto"> |
| :--- | :--- |
| 优点 | 缺点 |

![Image](https://prod-files-secure.s3.us-west-2.amazonaws.com/39ed1227-6d7d-4570-be36-9ccd4a2c4241/a9245ec9-70dd-4005-b534-0d54315fc5f3/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45HZZMZUHI%2F20240601%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20240601T225513Z&X-Amz-Expires=3600&X-Amz-Signature=92055731aee51d356d5b514bc6ac7e937096670ae5bdc2d9a6dbb30fd0878b9e&X-Amz-SignedHeaders=host&x-id=GetObject)

| <img src="https://cdn.ifttt.fun/gh/jarlin8/OSS@main/icons/customize/pros3.svg" height="auto"> | <img src="https://cdn.ifttt.fun/gh/jarlin8/OSS@main/icons/customize/cons3.svg" height="auto"> |
| :--- | :--- |
| 优点 | 缺点 |

![Image](https://prod-files-secure.s3.us-west-2.amazonaws.com/39ed1227-6d7d-4570-be36-9ccd4a2c4241/e1e580a2-2e5c-4780-9ff4-19c318fc2284/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45HZZMZUHI%2F20240601%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20240601T225513Z&X-Amz-Expires=3600&X-Amz-Signature=cb41a32cff85aa81309a788141d2c5e3191137a49fc5f34195e5dd31f8d30814&X-Amz-SignedHeaders=host&x-id=GetObject)