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

<img src="https://prod-files-secure.s3.us-west-2.amazonaws.com/39ed1227-6d7d-4570-be36-9ccd4a2c4241/f51d3d83-55d4-4bdf-9604-f37ec77ab556/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45HZZMZUHI%2F20240812%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20240812T165520Z&X-Amz-Expires=3600&X-Amz-Signature=8e7ee45e72841f930be65b0fe431a011e7d0e178e367b176cb9e6bb065d572e9&X-Amz-SignedHeaders=host&x-id=GetObject" alt="Image">
</details>

SEO标题：`rank_math_title`

`TMGM测评 %currentyear% 开户必看 %sep% %sitename%`

SEO关键字：`rank_math_focus_keyword`

一句话总结：`_review_post_summary_text`

<details><summary>图片展示使用位置</summary>

<img src="https://prod-files-secure.s3.us-west-2.amazonaws.com/39ed1227-6d7d-4570-be36-9ccd4a2c4241/4b96a922-296c-4f4e-8630-d1c870cbce01/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45HZZMZUHI%2F20240812%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20240812T165521Z&X-Amz-Expires=3600&X-Amz-Signature=2d414bd40abe0ca930e398c1fe29410cf465a56d4d1dd15e2af339207e04f222&X-Amz-SignedHeaders=host&x-id=GetObject" alt="Image">
</details>

平台亮点 用于SEO展示 **摘要**：`post_excerpt`  等价于 `rank_math_description`

<details><summary>图片展示使用位置</summary>

<img src="https://prod-files-secure.s3.us-west-2.amazonaws.com/39ed1227-6d7d-4570-be36-9ccd4a2c4241/1ee11f63-b60a-4dfe-a7a7-d58ff23b5d88/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45HZZMZUHI%2F20240812%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20240812T165521Z&X-Amz-Expires=3600&X-Amz-Signature=a002710ac1b9091b90b13b454f0c50aa06ccffe35767e1ae9488f6d69693d880&X-Amz-SignedHeaders=host&x-id=GetObject" alt="Image">
<img src="https://prod-files-secure.s3.us-west-2.amazonaws.com/39ed1227-6d7d-4570-be36-9ccd4a2c4241/ad4118b5-78d8-4fbe-801e-3b29b5d99c01/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45HZZMZUHI%2F20240812%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20240812T165521Z&X-Amz-Expires=3600&X-Amz-Signature=94e3bb138e7c619da59f645b36ea9dd0afdddc9ac90167eb8495af053adc3a2e&X-Amz-SignedHeaders=host&x-id=GetObject" alt="Image">
<img src="https://prod-files-secure.s3.us-west-2.amazonaws.com/39ed1227-6d7d-4570-be36-9ccd4a2c4241/a38cf7c9-a79c-4b64-9e94-13589fe0758b/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45HZZMZUHI%2F20240812%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20240812T165521Z&X-Amz-Expires=3600&X-Amz-Signature=0bc92831f88d0885bb2b8b16b0bf3a6a4136426a81d3594b066a14a5696b4299&X-Amz-SignedHeaders=host&x-id=GetObject" alt="Image">
<img src="https://prod-files-secure.s3.us-west-2.amazonaws.com/39ed1227-6d7d-4570-be36-9ccd4a2c4241/7da6fc1e-d2ac-42ae-8c75-cb5749aa18f6/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45HZZMZUHI%2F20240812%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20240812T165521Z&X-Amz-Expires=3600&X-Amz-Signature=5678e890e9edb2035f464e35421e493708ea26a8aa6e9998e25be003ea6503d3&X-Amz-SignedHeaders=host&x-id=GetObject" alt="Image">
<img src="https://prod-files-secure.s3.us-west-2.amazonaws.com/39ed1227-6d7d-4570-be36-9ccd4a2c4241/7e97f40a-eaee-47f5-b2f9-475f96808fa7/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45HZZMZUHI%2F20240812%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20240812T165521Z&X-Amz-Expires=3600&X-Amz-Signature=bd0388514ff33d153d0e3d3f48d2a9295cc86f3470ec2935430a438f02a72790&X-Amz-SignedHeaders=host&x-id=GetObject" alt="Image">
</details>

head：`_review_heading`

<details><summary>图片展示使用位置</summary>

<img src="https://prod-files-secure.s3.us-west-2.amazonaws.com/39ed1227-6d7d-4570-be36-9ccd4a2c4241/3a4650ad-9887-415c-889a-edd51fa54f27/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45HZZMZUHI%2F20240812%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20240812T165522Z&X-Amz-Expires=3600&X-Amz-Signature=c7c0bdb084bc78ea440d814e62e6f46154f7e66ee3b8a43738c0a473b41ad394&X-Amz-SignedHeaders=host&x-id=GetObject" alt="Image">
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

![Image](https://prod-files-secure.s3.us-west-2.amazonaws.com/39ed1227-6d7d-4570-be36-9ccd4a2c4241/4f898f9d-0fa7-4e43-acd3-ac6bc7be575a/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45HZZMZUHI%2F20240812%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20240812T165519Z&X-Amz-Expires=3600&X-Amz-Signature=458b62a3d3917c971bf0864e94ba7d0d5aa4658c2dac9b387e25fb62d2484654&X-Amz-SignedHeaders=host&x-id=GetObject)

### 单个推荐
`[wpsm_top postid="20641,10424,11542,10447,10406,28706" title="平台推荐列表"]`

[wpsm_top postid="10424" title="ATFX CTA"]

![Image](https://prod-files-secure.s3.us-west-2.amazonaws.com/39ed1227-6d7d-4570-be36-9ccd4a2c4241/5ac620dc-51a8-48b6-b55d-91f47299193c/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45HZZMZUHI%2F20240812%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20240812T165519Z&X-Amz-Expires=3600&X-Amz-Signature=3af5f87b57d960a793abc8359ed93c92ba78f9a231ba432fce44d3386521fee5&X-Amz-SignedHeaders=host&x-id=GetObject)

详情对比

`[wpsm_woocharts ids="20641,10406,10424" disable="brand,stock,userrate,review"]`

![Image](https://prod-files-secure.s3.us-west-2.amazonaws.com/39ed1227-6d7d-4570-be36-9ccd4a2c4241/bf3ba45f-b9f3-4295-8aef-b4a495fd25f4/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45HZZMZUHI%2F20240812%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20240812T165519Z&X-Amz-Expires=3600&X-Amz-Signature=3ba6f684d507024645e689a3899a18191d51cea27f33add7fe0920567bae31b3&X-Amz-SignedHeaders=host&x-id=GetObject)

![Image](https://prod-files-secure.s3.us-west-2.amazonaws.com/39ed1227-6d7d-4570-be36-9ccd4a2c4241/30bc56ef-f383-4b48-9768-2ebc9e436ec0/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45HZZMZUHI%2F20240812%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20240812T165519Z&X-Amz-Expires=3600&X-Amz-Signature=467007693c3e64a27dee9204b91692191d3b0f5868565d744e9cc28296d60f24&X-Amz-SignedHeaders=host&x-id=GetObject)

## sync同步模块

### PROs CONs对照表

| <img src="https://cdn.ifttt.fun/gh/jarlin8/OSS@main/icons/customize/pros.svg" height="auto" width="37.3%"> | <img src="https://cdn.ifttt.fun/gh/jarlin8/OSS@main/icons/customize/cons.svg" height="auto" width="28.8%"> |
| :--- | :--- |
| 优点 | 缺点 |

![Image](https://prod-files-secure.s3.us-west-2.amazonaws.com/39ed1227-6d7d-4570-be36-9ccd4a2c4241/8742b755-dfb5-4004-9a5f-d6e561664bd8/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45HZZMZUHI%2F20240812%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20240812T165519Z&X-Amz-Expires=3600&X-Amz-Signature=0ce32705bf111b274de0b198783a6dc0c48a3dd3a509e0f8162e0cc15a9dc0b0&X-Amz-SignedHeaders=host&x-id=GetObject)

| <img src="https://cdn.ifttt.fun/gh/jarlin8/OSS@main/icons/customize/pros1.svg" height="auto"> | <img src="https://cdn.ifttt.fun/gh/jarlin8/OSS@main/icons/customize/cons1.svg" height="auto"> |
| :--- | :--- |
| 优点 | 缺点 |

![Image](https://prod-files-secure.s3.us-west-2.amazonaws.com/39ed1227-6d7d-4570-be36-9ccd4a2c4241/806358f8-c9c4-4e17-bb35-c6c76a5397a5/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45HZZMZUHI%2F20240812%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20240812T165519Z&X-Amz-Expires=3600&X-Amz-Signature=848b24f3ebdadfc88e2cfd0b08807e15e6a632b02c3bfed9e442b53cf1c999b3&X-Amz-SignedHeaders=host&x-id=GetObject)

| <img src="https://cdn.ifttt.fun/gh/jarlin8/OSS@main/icons/customize/pros2.svg" height="auto"> | <img src="https://cdn.ifttt.fun/gh/jarlin8/OSS@main/icons/customize/cons2.svg" height="auto"> |
| :--- | :--- |
| 优点 | 缺点 |

![Image](https://prod-files-secure.s3.us-west-2.amazonaws.com/39ed1227-6d7d-4570-be36-9ccd4a2c4241/a9245ec9-70dd-4005-b534-0d54315fc5f3/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45HZZMZUHI%2F20240812%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20240812T165519Z&X-Amz-Expires=3600&X-Amz-Signature=b27c2fd1345af4a38418563f7bcdd938ff8e07920f6049fea3f6e01ba14cad31&X-Amz-SignedHeaders=host&x-id=GetObject)

| <img src="https://cdn.ifttt.fun/gh/jarlin8/OSS@main/icons/customize/pros3.svg" height="auto"> | <img src="https://cdn.ifttt.fun/gh/jarlin8/OSS@main/icons/customize/cons3.svg" height="auto"> |
| :--- | :--- |
| 优点 | 缺点 |

![Image](https://prod-files-secure.s3.us-west-2.amazonaws.com/39ed1227-6d7d-4570-be36-9ccd4a2c4241/e1e580a2-2e5c-4780-9ff4-19c318fc2284/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45HZZMZUHI%2F20240812%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20240812T165519Z&X-Amz-Expires=3600&X-Amz-Signature=9ac553c67a477b697f8c2cee66b55b0986c7e171426bb60a0a5d1433bcbbed07&X-Amz-SignedHeaders=host&x-id=GetObject)