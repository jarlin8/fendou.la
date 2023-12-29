---
title: "test"
post_status: "publish"
skip_file: "no"
taxonomy:
  category:
        - toutiao
  post_tag:

post_excerpt: ""
---
想知道如何在科技投资中规避泡沫，抓住明日之星？Gartner技术成熟度曲线为您指明方向！了解技术发展周期，精准识别具备长期价值的创新技术，做出明智投资决策。

```php
function convertPagesToMarkdown(pages) {
  return pages.map(page => {
    var title = page.properties["title"].title[0]?.text?.content;
    var slug = page.properties["slug"].rich_text[0].text.content;
    var post_status = page.properties["post_status"].rich_text[0].text.content;
    var skip_file = page.properties["skip_file"].rich_text[0].text.content;
    var category = page.properties["category"].multi_select.map(option => `        - ${option.name}`).join('\n');
    var post_tag = page.properties["post_tag"].multi_select.map(option => `        - ${option.name}`).join('\n');
    var post_excerpt = "";
```