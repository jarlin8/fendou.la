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

<img src="https://prod-files-secure.s3.us-west-2.amazonaws.com/39ed1227-6d7d-4570-be36-9ccd4a2c4241/f51d3d83-55d4-4bdf-9604-f37ec77ab556/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45HZZMZUHI%2F20240521%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20240521T225516Z&X-Amz-Expires=3600&X-Amz-Signature=13920f4c8349e6e7e3915a17b35adcdd48bfe22ed4504042cbbb817a7adc585b&X-Amz-SignedHeaders=host&x-id=GetObject" alt="Image">
</details>

SEO标题：`rank_math_title`

`TMGM测评 %currentyear% 开户必看 %sep% %sitename%`

SEO关键字：`rank_math_focus_keyword`

一句话总结：`_review_post_summary_text`

<details><summary>图片展示使用位置</summary>

<img src="https://prod-files-secure.s3.us-west-2.amazonaws.com/39ed1227-6d7d-4570-be36-9ccd4a2c4241/4b96a922-296c-4f4e-8630-d1c870cbce01/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45HZZMZUHI%2F20240521%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20240521T225517Z&X-Amz-Expires=3600&X-Amz-Signature=015049ef386c6105831883db17e33f4e4c5c19f205123b1699c79f64c637e043&X-Amz-SignedHeaders=host&x-id=GetObject" alt="Image">
</details>

平台亮点 用于SEO展示 **摘要**：`post_excerpt`  等价于 `rank_math_description`

<details><summary>图片展示使用位置</summary>

<img src="https://prod-files-secure.s3.us-west-2.amazonaws.com/39ed1227-6d7d-4570-be36-9ccd4a2c4241/1ee11f63-b60a-4dfe-a7a7-d58ff23b5d88/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45HZZMZUHI%2F20240521%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20240521T225517Z&X-Amz-Expires=3600&X-Amz-Signature=58c17f6a54cee0e8229971988feef4ab23751299ab5403fe51390e4bb3538bca&X-Amz-SignedHeaders=host&x-id=GetObject" alt="Image">
<img src="https://prod-files-secure.s3.us-west-2.amazonaws.com/39ed1227-6d7d-4570-be36-9ccd4a2c4241/ad4118b5-78d8-4fbe-801e-3b29b5d99c01/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45HZZMZUHI%2F20240521%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20240521T225517Z&X-Amz-Expires=3600&X-Amz-Signature=3bf548871187cce0b06025c70bf4c3ad72208bd7f6bc9261426a16f9fa702c6d&X-Amz-SignedHeaders=host&x-id=GetObject" alt="Image">
<img src="https://prod-files-secure.s3.us-west-2.amazonaws.com/39ed1227-6d7d-4570-be36-9ccd4a2c4241/a38cf7c9-a79c-4b64-9e94-13589fe0758b/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45HZZMZUHI%2F20240521%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20240521T225517Z&X-Amz-Expires=3600&X-Amz-Signature=a6043097c5cda5d8321bb413839e4989e9f6c318d456bbc7e511e90a643cde31&X-Amz-SignedHeaders=host&x-id=GetObject" alt="Image">
<img src="https://prod-files-secure.s3.us-west-2.amazonaws.com/39ed1227-6d7d-4570-be36-9ccd4a2c4241/7da6fc1e-d2ac-42ae-8c75-cb5749aa18f6/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45HZZMZUHI%2F20240521%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20240521T225517Z&X-Amz-Expires=3600&X-Amz-Signature=b1312b1dc70b03342545c6a893d1db4bd5cc59664f81c560ce72a534fa258f15&X-Amz-SignedHeaders=host&x-id=GetObject" alt="Image">
<img src="https://prod-files-secure.s3.us-west-2.amazonaws.com/39ed1227-6d7d-4570-be36-9ccd4a2c4241/7e97f40a-eaee-47f5-b2f9-475f96808fa7/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45HZZMZUHI%2F20240521%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20240521T225517Z&X-Amz-Expires=3600&X-Amz-Signature=bcfcc659fa4eeacc3072bd5bd2232b40abc46f31addc8ce0451e735d39e9be00&X-Amz-SignedHeaders=host&x-id=GetObject" alt="Image">
</details>

head：`_review_heading`

<details><summary>图片展示使用位置</summary>

<img src="https://prod-files-secure.s3.us-west-2.amazonaws.com/39ed1227-6d7d-4570-be36-9ccd4a2c4241/3a4650ad-9887-415c-889a-edd51fa54f27/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45HZZMZUHI%2F20240521%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20240521T225517Z&X-Amz-Expires=3600&X-Amz-Signature=c0ef21752a50aa853d9f87c792ed99dbdd249a4e2eb20ad80ed5c5dacdbf0d31&X-Amz-SignedHeaders=host&x-id=GetObject" alt="Image">
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

![Image](https://prod-files-secure.s3.us-west-2.amazonaws.com/39ed1227-6d7d-4570-be36-9ccd4a2c4241/4f898f9d-0fa7-4e43-acd3-ac6bc7be575a/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45HZZMZUHI%2F20240521%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20240521T225515Z&X-Amz-Expires=3600&X-Amz-Signature=01909def9d6c3fd55d30509bcdc7159b8658267f449d84fc345ba553c8e52e41&X-Amz-SignedHeaders=host&x-id=GetObject)

### 单个推荐
`[wpsm_top postid="20641,10424,11542,10447,10406,28706" title="平台推荐列表"]`

[wpsm_top postid="10424" title="ATFX CTA"]

![Image](https://prod-files-secure.s3.us-west-2.amazonaws.com/39ed1227-6d7d-4570-be36-9ccd4a2c4241/5ac620dc-51a8-48b6-b55d-91f47299193c/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45HZZMZUHI%2F20240521%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20240521T225515Z&X-Amz-Expires=3600&X-Amz-Signature=142b7d046d3d0f73450424fb7104d1819d19e779f6e983f6e1eec24bd438fb51&X-Amz-SignedHeaders=host&x-id=GetObject)

详情对比

`[wpsm_woocharts ids="20641,10406,10424" disable="brand,stock,userrate,review"]`

![Image](https://prod-files-secure.s3.us-west-2.amazonaws.com/39ed1227-6d7d-4570-be36-9ccd4a2c4241/bf3ba45f-b9f3-4295-8aef-b4a495fd25f4/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45HZZMZUHI%2F20240521%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20240521T225515Z&X-Amz-Expires=3600&X-Amz-Signature=611f8ba8df554b28e5988db064d5bce855c85ffaa10f3653db2c9a8aff164cfd&X-Amz-SignedHeaders=host&x-id=GetObject)

![Image](https://prod-files-secure.s3.us-west-2.amazonaws.com/39ed1227-6d7d-4570-be36-9ccd4a2c4241/30bc56ef-f383-4b48-9768-2ebc9e436ec0/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45HZZMZUHI%2F20240521%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20240521T225515Z&X-Amz-Expires=3600&X-Amz-Signature=965cb6ec40c6df1d3238988c46285660edccfa681add187034c595e6b1646eec&X-Amz-SignedHeaders=host&x-id=GetObject)

## sync同步模块

### PROs CONs对照表

| <img src="https://cdn.ifttt.fun/gh/jarlin8/OSS@main/icons/customize/pros.svg" height="auto" width="37.3%"> | <img src="https://cdn.ifttt.fun/gh/jarlin8/OSS@main/icons/customize/cons.svg" height="auto" width="28.8%"> |
| :--- | :--- |
| 优点 | 缺点 |

![Image](https://prod-files-secure.s3.us-west-2.amazonaws.com/39ed1227-6d7d-4570-be36-9ccd4a2c4241/8742b755-dfb5-4004-9a5f-d6e561664bd8/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45HZZMZUHI%2F20240521%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20240521T225515Z&X-Amz-Expires=3600&X-Amz-Signature=9a7a99e29e6ba9835c1919749c5bfadd6e8370740b70a6aa6d00a8ad7d0a360b&X-Amz-SignedHeaders=host&x-id=GetObject)

| <img src="https://cdn.ifttt.fun/gh/jarlin8/OSS@main/icons/customize/pros1.svg" height="auto"> | <img src="https://cdn.ifttt.fun/gh/jarlin8/OSS@main/icons/customize/cons1.svg" height="auto"> |
| :--- | :--- |
| 优点 | 缺点 |

![Image](https://prod-files-secure.s3.us-west-2.amazonaws.com/39ed1227-6d7d-4570-be36-9ccd4a2c4241/806358f8-c9c4-4e17-bb35-c6c76a5397a5/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45HZZMZUHI%2F20240521%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20240521T225515Z&X-Amz-Expires=3600&X-Amz-Signature=d8e62076bac9c652adbbfc7669f703aa8b6b5ca6b899025e1ec51702090e64c2&X-Amz-SignedHeaders=host&x-id=GetObject)

| <img src="https://cdn.ifttt.fun/gh/jarlin8/OSS@main/icons/customize/pros2.svg" height="auto"> | <img src="https://cdn.ifttt.fun/gh/jarlin8/OSS@main/icons/customize/cons2.svg" height="auto"> |
| :--- | :--- |
| 优点 | 缺点 |

![Image](https://prod-files-secure.s3.us-west-2.amazonaws.com/39ed1227-6d7d-4570-be36-9ccd4a2c4241/a9245ec9-70dd-4005-b534-0d54315fc5f3/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45HZZMZUHI%2F20240521%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20240521T225515Z&X-Amz-Expires=3600&X-Amz-Signature=9c8ca127f42f505a782df5d72dd2002071dfa3ba60998f2f96040cb11fefe177&X-Amz-SignedHeaders=host&x-id=GetObject)

| <img src="https://cdn.ifttt.fun/gh/jarlin8/OSS@main/icons/customize/pros3.svg" height="auto"> | <img src="https://cdn.ifttt.fun/gh/jarlin8/OSS@main/icons/customize/cons3.svg" height="auto"> |
| :--- | :--- |
| 优点 | 缺点 |

![Image](https://prod-files-secure.s3.us-west-2.amazonaws.com/39ed1227-6d7d-4570-be36-9ccd4a2c4241/e1e580a2-2e5c-4780-9ff4-19c318fc2284/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45HZZMZUHI%2F20240521%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20240521T225515Z&X-Amz-Expires=3600&X-Amz-Signature=31c213463e2e0733d31e2b83e3c6896a22bbdc474685ecb320f31de223060590&X-Amz-SignedHeaders=host&x-id=GetObject)