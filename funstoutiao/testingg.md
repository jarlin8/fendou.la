---
title: testtttt
post_status: publish
skip_file: no
taxonomy:
  category:
        - toutiao
  post_tag:

post_excerpt: 
---
function push2GitHub(pages) {
pages.forEach(page => {
var githubApiUrl = "[https://api.github.com/repos/](https://api.github.com/repos/)" + repo + "/contents/" + path + encodeURIComponent(page.slug) + ".md" + "?ref=" + branch;
var headers = {
"Authorization": "token " + githubToken,
"Content-Type": "application/json"
};

```plain text
var sha; // 不需要初始化为null
var fileExists = false; // 标记文件是否存在

// 尝试获取文件信息以检查文件是否存在
var getFileResponse = UrlFetchApp.fetch(githubApiUrl, { method: "get", headers: headers, muteHttpExceptions: true });
if (getFileResponse.getResponseCode() === 200) {
  sha = JSON.parse(getFileResponse.getContentText()).sha;
  fileExists = true; // 文件存在
}

var blob = Utilities.newBlob(page.markdown, 'text/plain', 'UTF-8');
var fileContent = Utilities.base64Encode(blob.getBytes());

var payload = {
  message: "Updated via Google Apps Script",
  content: fileContent,
  branch: branch
};

// 仅在文件存在时添加SHA
if (fileExists) {
  payload.sha = sha;
}

var putOptions = { method: "put", headers: headers, payload: JSON.stringify(payload), muteHttpExceptions: true };
var putResponse = UrlFetchApp.fetch(githubApiUrl, putOptions);
if (putResponse.getResponseCode() !== 200 && putResponse.getResponseCode() !== 201) {
  Logger.log("Error pushing to GitHub: " + putResponse.getContentText());
}

```

});
}