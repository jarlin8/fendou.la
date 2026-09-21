---
title: "PHP&Linux 服务器配置笔记"
post_status: "publish"
skip_file: "no"
post_date: "2023-12-29T04:10:00.000Z"
taxonomy:
  category:
        - project
  post_tag:
        - code
        - php
        - redis
post_excerpt: ""
---
## 有趣的网站

* [https://www.gwern.net/index ](https://www.gwern.net/index) 这个是一个高度模仿wikipedia的悬停弹窗设计的网站，作者是因为很喜欢那种在同一个页面，浏览所有需要查看的主题，而不需要反复跳转。

* [https://xianxie6.github.io/qingming-riverside/](https://xianxie6.github.io/qingming-riverside/) 清明上河图可交互版本 有声音与动画

<details><summary>ByteByteGoHq https://github.com/ByteByteGoHq/system-design-101</summary>

[ByteByteGo](https://bytebytego.com/guides/?utm_source=gemini) 是一个专注于软件工程与系统设计（System Design）的技术学习平台，由知名技术图书《System Design Interview》作者 Alex Xu（许式伟）创立。

![image](https://cdn.jsdmirror.com/gh/jarlin8/fendou.la@main/fendou-posts/images/a50567db3b2d508ca591fda6d7d14956.png)
</details>

该网站的核心特色是用**高度结构化的可视化图解（Infographics）**，将复杂晦涩的后端架构与底层技术拆解得直观易懂。

页面展示的 **Visual Guides** 板块主要涵盖：

* **核心技术主题**：包括 API 与 Web 开发、数据库与存储、缓存与性能优化、分布式系统、微服务架构、DevOps/CI-CD 及网络协议。

* **真实系统案例分析**：解析 Netflix、Twitter、YouTube 等大型科技公司的实际架构方案。

* **面试与编码进阶**：系统设计面试重点、编码规范、计算机基础及 AI/LLM 底层机制拆解。

## Redis相关知识

PHP 中使用 Redis 前，我们需要确保已经安装了 redis 服务，且你的机器上能正常使用 PHP。 接下来让我们安装 PHP redis 驱动，下载地址为:[https://github.com/phpredis/phpredis/](https://github.com/phpredis/phpredis/)

![image](https://cdn.jsdmirror.com/gh/jarlin8/fendou.la@main/fendou-posts/images/9cbee606633834e6d48205cc95f8b463.png)

## argon 主题底部版权申明

argon: Theme Footer (footer.php):5

`<div>Theme <a href="https://github.com/solstice23/argon-theme" target="_blank"><strong>Argon</strong></a><?php if (get_option('argon_hide_footer_author') != 'true') {echo " By solstice23"; }?></div>`

argon: Theme Functions (functions.php):2007

```php
//检测页面底部版权是否被修改
function alert_footer_copyright_changed(){ ?>
    <div class='notice notice-warning is-dismissible'>
        <p><?php _e("警告：你可能修改了 Argon 主题页脚的版权声明，Argon 主题要求你至少保留主题的 Github 链接或主题的发布文章链接。", 'argon');?></p>
    </div>
<?php }
function check_footer_copyright(){
    $footer = file_get_contents(get_theme_root() . "/" . wp_get_theme() -> template . "/footer.php");
    if ((strpos($footer, "github.com/solstice23/argon-theme") === false) && (strpos($footer, "solstice23.top") === false)){
        add_action('admin_notices', 'alert_footer_copyright_changed');
    }
}
check_footer_copyright();
```

argontheme.js:2611

```php
/*Console*/
!function(){...}();
```

## 禁用 wp-emoji-release.min.js

```php
// Disable the emoji's
function disable_emojis() {
 remove_action( 'wp_head', 'print_emoji_detection_script', 7 );
 remove_action( 'admin_print_scripts', 'print_emoji_detection_script' );
 remove_action( 'wp_print_styles', 'print_emoji_styles' );
 remove_action( 'admin_print_styles', 'print_emoji_styles' );
 remove_filter( 'the_content_feed', 'wp_staticize_emoji' );
 remove_filter( 'comment_text_rss', 'wp_staticize_emoji' );
 remove_filter( 'wp_mail', 'wp_staticize_emoji_for_email' );
 add_filter( 'tiny_mce_plugins', 'disable_emojis_tinymce' );
 add_filter( 'wp_resource_hints', 'disable_emojis_remove_dns_prefetch', 10, 2 );
}
add_action( 'init', 'disable_emojis' );

/**
 * Filter function used to remove the tinymce emoji plugin.
 * @param array $plugins
 * @return array Difference betwen the two arrays
 */
function disable_emojis_tinymce( $plugins ) {
 if ( is_array( $plugins ) ) {
 return array_diff( $plugins, array( 'wpemoji' ) );
 } else {
 return array();
 }
}

/**
 * Remove emoji CDN hostname from DNS prefetching hints.
 * @param array $urls URLs to print for resource hints.
 * @param string $relation_type The relation type the URLs are printed for.
 * @return array Difference betwen the two arrays.
 */
function disable_emojis_remove_dns_prefetch( $urls, $relation_type ) {
 if ( 'dns-prefetch' == $relation_type ) {
 /** This filter is documented in wp-includes/formatting.php */
 $emoji_svg_url = apply_filters( 'emoji_svg_url', 'https://s.w.org/images/core/emoji/2/svg/' );

$urls = array_diff( $urls, array( $emoji_svg_url ) );
 }

return $urls;
}
```

## jsDelivr 域名遭 DNS 污染解决方案

### 官方子域

* CloudFlare：test1.jsdelivr.net

* CloudFlare：testingcf.jsdelivr.net

* Fastly：fastly.jsdelivr.net

* GCORE：gcore.jsdelivr.net

* originfastly.jsdelivr.net

### 针对 GH 的反向代理

```php
#针对/gh目录的反代
location /gh
{
proxy_pass https://104.16.86.20;
proxy_set_header Host cdn.jsdelivr.net;
proxy_ssl_server_name on;
proxy_ssl_name cdn.jsdelivr.net;
proxy_set_header X-Real-IP $remote_addr;
proxy_set_header X-Forwarded-For $proxy_add_x_forwarded_for;
proxy_set_header REMOTE-HOST $remote_addr;
}
```