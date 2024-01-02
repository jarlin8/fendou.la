---
title: 富文本转markdown代码
post_status: publish
skip_file: no
taxonomy:
  category:
        - toutiao
  post_tag:
        - php
post_excerpt: 
---
```javascript
function convertRichTextToMarkdown(richTexts) {
  if (!Array.isArray(richTexts)) {
    return '';
  }
  return richTexts.map(text => {
    if (text.href) {
      // 处理链接
      return `[${text.plain_text}](${text.href})`;
    } else if (text.annotations && text.annotations.code) {
      // 处理内联代码
      return `\`${text.plain_text}\``;
    } else {
      // 支持粗体和颜色
      var markdownText = text.plain_text;
      if (text.annotations && text.annotations.bold) {
        markdownText = `**${markdownText}**`;
      }
      if (text.color && text.color !== 'default') {
        markdownText = `<span style="color:${text.color}">${markdownText}</span>`;
      }
      return markdownText;
    }
  }).join('');
}
```