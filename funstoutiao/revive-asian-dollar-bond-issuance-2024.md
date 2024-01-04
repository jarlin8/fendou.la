---
title: 稳定利率为 2024 年亚洲美元债券发行注入活力
post_status: publish
skip_file: no
taxonomy:
  category:
        - toutiao
  post_tag:
        - 美股
post_excerpt: 
---
![Image](https://images.unsplash.com/photo-1492571350019-22de08371fd3?ixlib=rb-4.0.3&q=85&fm=jpg&crop=entropy&cs=srgb)

亚洲几个大的交易商预计，随着利率趋于稳定以及企业加大借贷力度以满足资本支出计划，2024年亚洲的美元债券发行量将增长10%，扭转债券市场过去8年中最疲软的一年。

2024年伊始，一些亚洲大型企业纷纷涌入美元债券市场，其中包括SK海力士和浦项制铁，两家公司计划合计筹集20亿美元资金。印尼共和国也早早进入美元融资市场，通过一笔三期交易筹集了20.5亿美元。

[mark_e]

根据Dealogic的数据，2023年亚太地区（包括日本）共发行了2720亿美元的美元债券，为2015年以来最低水平。由于美国的利率上升，使得在一些本币和国内银行市场借贷成本更低，导致企业推迟了发债计划。

[/mark_e]

对于亚洲的投资银行来说，债券发行的下滑又一次打击了他们的收费收入，因为股票资本市场和企业并购咨询业务的收入也因活动水平低迷而放缓。

美元债券发行前景改善的关键在于，美联储将在2024年开始降息，因为有迹象表明通胀开始得到控制。

摩根士丹利亚太区债务银团主管 Elaine He 表示：“亚洲一个非常重要的主题是境内利率与境外利率，因此在亚洲的许多地区，境内借贷成本要低得多。随着美联储可能在2024年降息，境内外借贷成本差距的缩小可能鼓励境外美元借贷活动的增加。”

2021年新冠疫情期间，亚洲的美元债券发行量创下了历史新高，当时各国央行纷纷降息，大多数主要国家政府都下令采取紧急财政刺激措施。然而，随着利率在过去两年被上调，美元债券发行量有所下降。

美国银行亚太区债务资本市场（DCM）银团主管 Joseph Pepping 表示，他预计，随着利率前景更加明朗，亚太区美元债券发行量将在2024年增长约10%。

他表示：“现在大家都很放心，我们已经处于加息周期的顶部，央行已经相当明确地表示，利率将在更长时间内保持高位。过去两年一直在观望市场的企业将开始重新进入市场。”

瑞银亚洲债务资本市场联席主管 Terry Schmassmann 表示，亚洲地区的企业，尤其是可再生能源和电动汽车供应链领域的企业，需要进入市场以获得资金支持其扩张计划。

他说：“鉴于发达市场不确定的利率环境，很多企业都搁置了海外资本支出计划。现在，随着‘高利率将持续更长时间’的说法开始被市场接受，我们看到一些资本支出需求开始显现。我预计今年的离岸发行将会更为繁忙。”

然而，在中国，高收益美元债券发行仍然低迷，原因是曾经活跃的美元债券市场参与者——房地产行业仍然陷入困境。Dealogic的数据显示，2023年中国发行的美元债券为425亿美元，远低于2019年的市场峰值2105亿美元。

摩根士丹利的 He 表示：“这取决于企业需要多少资金，以及他们是否能找到更便宜的境内融资渠道。鉴于中国经济的规模，预计2024年高收益债券发行将会增加。”

根据Dealogic的数据，2023年亚太地区所有币种的债券发行总额为1.72万亿美元，为2015年以来最低水平。

![Image](https://images.unsplash.com/photo-1634704784915-aacf363b021f?ixlib=rb-4.0.3&q=85&fm=jpg&crop=entropy&cs=srgb)
赶紧开户赚钱去!!!！

<details><summary>这是什么模块</summary>

<p>文字？段落？</p>
<h1>标题一</h1>
<h2>标题二</h2>
<h3>标题三</h3>
<blockquote>我是BLOCK引用
第三第四</blockquote>
<li>快吃饭客单数狂饭</li>
<li>多多多死多哦打死佛</li>
<li>东老佛哦对睡戳</li>
<li>老热or哦</li>
<li>二看诶诶诶金耳环</li>
<pre><code class="javascript">// 全局变量
var notionToken =
  PropertiesService.getScriptProperties().getProperty("notionToken"); // Notion API密钥
var databaseId = "83db87faf6a64609ab70fed435a23ca7"; // Notion数据库ID
var githubToken =
  PropertiesService.getScriptProperties().getProperty("GITHUB_TOKEN"); // GitHub访问令牌
var repo = "jarlin8/fendou.la"; // 替换为您的GitHub用户名和仓库名
var path = "funstoutiao"; // 文件路径
var branch = "main"; // 分支名

function getNotionPages(databaseId, notionToken) {
  var headers = {
    Authorization: "Bearer " + notionToken,
    "Content-Type": "application/json",
    "Notion-Version": "2022-06-28",
  };

  var allPages = [];
  var hasMore = true;
  var startCursor = null;

  while (hasMore) {
    var apiUrl = "https://api.notion.com/v1/databases/" + databaseId + "/query";

    var postBody = {
      page_size: 100, // 可以请求最多100条数据
    };

    if (startCursor) {
      postBody["start_cursor"] = startCursor;
    }

    var response = UrlFetchApp.fetch(apiUrl, {
      method: "post",
      headers: headers,
      payload: JSON.stringify(postBody),
    });

    var data = JSON.parse(response.getContentText());
    allPages = allPages.concat(data.results);

    hasMore = data.has_more;
    startCursor = data.next_cursor;
  }

  return allPages;
}

function convertPagesToMarkdown(pages) {
  return pages.map((page) => {
    var title = page.properties["title"].title[0]?.text?.content;
    var slug = page.properties["slug"].rich_text[0].text.content;
    var post_status = page.properties["post_status"].select
      ? page.properties["post_status"].select.name
      : "";
    var skip_file = page.properties["skip_file"].select
      ? page.properties["skip_file"].select.name
      : "";
    var category = page.properties["category"].multi_select
      .map((option) => `        - ${option.name}`)
      .join("\n");
    var post_tag = page.properties["post_tag"].multi_select
      .map((option) => `        - ${option.name}`)
      .join("\n");
    var post_excerpt = "";

    // 检查post_excerpt属性是否存在，并且它的rich_text数组是否有元素
    if (
      page.properties["Description"] &&
      Array.isArray(page.properties["Description"].rich_text) &&
      page.properties["Description"].rich_text.length > 0
    ) {
      post_excerpt = page.properties["Description"].rich_text[0].text.content;
    }

    // 获取子页面内容
    var childrenContent = getChildrenContent(page.id, notionToken);

    // 构造YAML表头
    var yamlHeader = `---
title: ${title}
post_status: ${post_status}
skip_file: ${skip_file}
taxonomy:
  category:
${category}
  post_tag:
${post_tag}
post_excerpt: ${post_excerpt}
---\n`;

    var markdownContent = convertNotionBlocksToMarkdown(childrenContent);
    var markdown = yamlHeader + markdownContent;
    // 如果页面的 post_status 为 draft 或 skip_file 为 true，就跳过该页面，不转换为 Markdown 格式
    if (post_status === "draft" || skip_file === "true") {
      markdown = "";
    }
    return { slug, markdown };
  });
}

function getChildrenContent(pageId, notionToken) {
  var headers = {
    Authorization: "Bearer " + notionToken,
    "Content-Type": "application/json",
    "Notion-Version": "2022-06-28",
  };
  var apiUrl = `https://api.notion.com/v1/blocks/${pageId}/children`;

  try {
    var response = UrlFetchApp.fetch(apiUrl, {
      method: "get",
      headers: headers,
    });
    var blocks = JSON.parse(response.getContentText()).results;

    console.log("Blocks for page ID " + pageId + ": ", blocks); // 日志输出

    if (blocks.length === 0) {
      console.log("No child blocks found for page ID:", pageId);
    }

    return blocks;
  } catch (e) {
    console.error(
      "Error fetching child blocks for page ID:",
      pageId,
      "; Error:",
      e
    );
    return []; // 返回空数组以防错误
  }
}

function convertNotionBlocksToMarkdown(blocks) {
  var markdown = blocks
    .map((block) => {
      switch (block.type) {
        case "paragraph": //富文本段落
          return convertRichTextToMarkdown(block.paragraph.rich_text);
        case "heading_1": //H1
          return "# " + convertRichTextToMarkdown(block.heading_1.rich_text);
        case "heading_2": //H2
          return "## " + convertRichTextToMarkdown(block.heading_2.rich_text);
        case "heading_3": //H3
          return "### " + convertRichTextToMarkdown(block.heading_3.rich_text);
        case "bulleted_list_item": //子弹列表
          return (
            "* " + convertRichTextToMarkdown(block.bulleted_list_item.rich_text)
          );
        case "numbered_list_item": //数字列表
          return (
            "1. " +
            convertRichTextToMarkdown(block.numbered_list_item.rich_text)
          );
        case "table": //表格
          return convertTableBlockToMarkdown(block);
        case "quote": //引用
          return processQuoteBlock(block);
        case "toggle": //点击折叠行
          return processToggleBlock(block);
        case "synced_block": //同步块
          return processSyncedBlock(block);
        case "image": //图片
          if (block.image && (block.image.file || block.image.external)) {
            var imageUrl =
              block.image.type === "file"
                ? block.image.file.url
                : block.image.external.url;
            return `![Image](${imageUrl})`;
          }
          return "";
        case "code": //代码
          var codeText = block.code.rich_text
            .map((text) => text.plain_text)
            .join("\n");
          if (codeText.includes("\n")) {
            // 多行代码块
            var language = block.code.language || "";
            return `\`\`\`${language}\n${codeText}\n\`\`\``;
          } else {
            // 单行代码块
            return `\`${codeText}\``;
          }
        default:
          return "";
      }
    })
    .join("\n\n");

  return markdown;
}

function convertRichTextToMarkdown(richTexts) {
  if (!Array.isArray(richTexts)) {
    return "";
  }
  return richTexts
    .map((text) => {
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
        if (text.color && text.color !== "default") {
          markdownText = `<span style="color:${text.color}">${markdownText}</span>`;
        }
        return markdownText;
      }
    })
    .join("");
}

//开始处理表格
// 新增函数来获取表格行
function getTableRows(blockId) {
  var apiUrl = "https://api.notion.com/v1/blocks/" + blockId + "/children";
  var headers = {
    Authorization: "Bearer " + notionToken,
    "Content-Type": "application/json",
    "Notion-Version": "2022-06-28",
  };
  var params = {
    method: "get",
    headers: headers,
    muteHttpExceptions: true,
  };

  var results = [];
  var hasMore = true;
  var startCursor = "";

  while (hasMore) {
    var fullUrl = apiUrl + (startCursor ? "?start_cursor=" + startCursor : "");
    var response = UrlFetchApp.fetch(fullUrl, params);
    var json = JSON.parse(response.getContentText());

    if (json.object === "error") {
      Logger.log("Error fetching table rows: " + json.message);
      return [];
    }

    results = results.concat(json.results);
    hasMore = json.has_more;
    startCursor = json.next_cursor;
  }

  return results
    .map((blockObject) => {
      if (blockObject.type === "table_row" && blockObject.table_row) {
        return blockObject.table_row.cells
          .map((cell) => {
            // 处理单元格中的富文本内容
            return convertCellToMarkdown(cell);
          })
          .join(" | ");
      }
      return null;
    })
    .filter((row) => row !== null);
}

function convertCellToMarkdown(cell) {
  var markdownContent = [];
  var inList = false;

  cell.forEach((richTextItem) => {
    if (richTextItem.type === "text") {
      if (richTextItem.text.link) {
        // 处理链接
        markdownContent.push(
          `[${richTextItem.plain_text}](${richTextItem.text.link.url})`
        );
      } else if (richTextItem.annotations && richTextItem.annotations.bold) {
        // 处理加粗文本
        markdownContent.push(`**${richTextItem.plain_text}**`);
      } else {
        // 普通文本
        markdownContent.push(richTextItem.plain_text);
      }
    } else if (richTextItem.type === "bulleted_list_item") {
      // 处理无序列表项
      inList = true;
      markdownContent.push(`* ${richTextItem.plain_text}`);
    } else if (richTextItem.type === "image") {
      // 处理图片
      var imageUrl =
        richTextItem.image.type === "file"
          ? richTextItem.image.file.url
          : richTextItem.image.external.url;
      markdownContent.push(`![Image](${imageUrl})`);
    }

    // 检查是否是列表的结尾
    if (inList && richTextItem.type !== "bulleted_list_item") {
      inList = false;
      markdownContent.push("\n"); // 在列表后添加换行
    }
  });

  return markdownContent.join(inList ? "\n" : " "); // 列表内部使用换行符，普通文本使用空格
}

function convertTableBlockToMarkdown(tableBlock) {
  // 获取表格行
  var tableRows = getTableRows(tableBlock.id);

  // 如果没有表格行，则直接返回空字符串
  if (!tableRows.length) {
    return "";
  }

  // 生成表头行（假设第一行为表头）
  var headerRow = tableRows[0];

  // 根据表头行生成表头分隔行
  var headerSeparator = "|" + " :--- |".repeat(headerRow.split(" | ").length);

  // 生成表格Markdown，包括表头行和表头分隔行
  var tableMarkdown = `| ${headerRow} |\n${headerSeparator}\n`;
  tableMarkdown += tableRows
    .slice(1)
    .map((row) => `| ${row} |`)
    .join("\n"); // 添加剩余的数据行

  return tableMarkdown;
}
// 处理表格结束

//开始为toggle处理HTML
function convertNotionBlocksToHTML(blocks) {
  var html = blocks
    .map((block) => {
      switch (block.type) {
        case "paragraph":
          return `<p>${convertRichTextToHTML(block.paragraph.rich_text)}</p>`;
        case "heading_1":
          return `<h1>${convertRichTextToHTML(block.heading_1.rich_text)}</h1>`;
        case "heading_2":
          return `<h2>${convertRichTextToHTML(block.heading_2.rich_text)}</h2>`;
        case "heading_3":
          return `<h3>${convertRichTextToHTML(block.heading_3.rich_text)}</h3>`;
        case "bulleted_list_item":
          return `<li>${convertRichTextToHTML(
            block.bulleted_list_item.rich_text
          )}</li>`;
        case "numbered_list_item":
          return `<li>${convertRichTextToHTML(
            block.numbered_list_item.rich_text
          )}</li>`;
        case "quote":
          return `<blockquote>${convertRichTextToHTML(
            block.quote.rich_text
          )}</blockquote>`;
        case "image":
          if (block.image && (block.image.file || block.image.external)) {
            var imageUrl =
              block.image.type === "file"
                ? block.image.file.url
                : block.image.external.url;
            return `<img src="${imageUrl}" alt="Image">`;
          }
          return "";
        case "code":
          var codeText = block.code.rich_text
            .map((text) => text.plain_text)
            .join("\n");
          if (codeText.includes("\n")) {
            var language = block.code.language || "";
            return `<pre><code class="${language}">${codeText}</code></pre>`;
          } else {
            return `<code>${codeText}</code>`;
          }
        default:
          return "";
      }
    })
    .join("\n\n");

  return html;
}

function convertRichTextToHTML(richTexts) {
  if (!Array.isArray(richTexts)) {
    return "";
  }
  return richTexts
    .map((text) => {
      if (text.href) {
        return `<a href="${text.href}">${text.plain_text}</a>`;
      } else if (text.annotations && text.annotations.code) {
        return `<code>${text.plain_text}</code>`;
      } else {
        var htmlText = text.plain_text;
        if (text.annotations && text.annotations.bold) {
          htmlText = `<strong>${htmlText}</strong>`;
        }
        if (text.color && text.color !== "default") {
          htmlText = `<span style="color:${text.color}">${htmlText}</span>`;
        }
        return htmlText;
      }
    })
    .join("");
}
//为toggle处理HTML结束

// toggle处理
function processToggleBlock(blockObject) {
  if (blockObject.type === "toggle" && blockObject.toggle) {
    // 提取Toggle块的标题
    var toggleTitle = blockObject.toggle.rich_text
      .map((text) => text.plain_text)
      .join("");

    // 获取子块（如果有）
    var childrenBlocks = [];
    if (blockObject.has_children) {
      childrenBlocks = getChildrenContent(blockObject.id, notionToken);
    }

    // 将子块转换为Markdown
    var childrenMarkdown = childrenBlocks
      .map((childBlock) => convertNotionBlocksToHTML([childBlock]))
      .join("\n");

    // 构造Markdown表示的Toggle块
    var toggleMarkdown = `<details><summary>${toggleTitle}</summary>\n\n${childrenMarkdown}\n</details>`;

    return toggleMarkdown;
  }
  return "";
}

//处理同步模块synced_block
function processSyncedBlock(blockObject) {
  if (blockObject.type === "synced_block" && blockObject.synced_block) {
    var syncedBlockContent = [];

    // 获取同步块的子块
    if (blockObject.has_children) {
      syncedBlockContent = getChildrenContent(blockObject.id, notionToken);
    }

    // 将子块转换为Markdown
    var childrenMarkdown = syncedBlockContent
      .map((childBlock) => convertNotionBlocksToMarkdown([childBlock]))
      .join("\n");

    return childrenMarkdown;
  }
  return "";
}
//处理引用quote模块
function processQuoteBlock(blockObject) {
  if (blockObject.type === "quote" && blockObject.quote) {
    // 提取Quote块的内容
    var quoteContent = blockObject.quote.rich_text
      .map((text) => text.plain_text)
      .join("");
    // 构造Markdown表示的Quote块
    var quoteMarkdown = `> ${quoteContent}`;
    return quoteMarkdown;
  }
  return "";
}

function push2GitHub(pages) {
  var githubApiUrl = "https://api.github.com/repos/" + repo; // GitHub的API地址
  // 定义一个headers对象
  var headers = {
    Authorization: "token " + githubToken,
    "Content-Type": "application/json",
  };

  // 获取分支的最新commit sha
  var getRefResponse = UrlFetchApp.fetch(
    githubApiUrl + "/git/ref/heads/" + branch,
    { method: "get", headers: headers, muteHttpExceptions: true }
  );
  if (getRefResponse.getResponseCode() !== 200) {
    Logger.log("Error getting ref: " + getRefResponse.getContentText());
    return;
  }
  var latestCommitSha = JSON.parse(getRefResponse.getContentText()).object.sha;

  // 创建一个tree对象，包含所有要修改的文件
  var tree = [];
  pages.forEach((page) => {
    var fileUrl =
      githubApiUrl +
      "/contents/" +
      path +
      "/" +
      encodeURIComponent(page.slug) +
      ".md" +
      "?ref=" +
      branch;
    var headers = {
      Authorization: "token " + githubToken,
      "Content-Type": "application/json",
    };
    var sha = null; // 初始化sha为null
    var fileExists = false; // 标记文件是否存在

    // 尝试获取文件信息以检查文件是否存在
    var getFileResponse = UrlFetchApp.fetch(fileUrl, {
      method: "get",
      headers: headers,
      muteHttpExceptions: true,
    });
    if (getFileResponse.getResponseCode() === 200) {
      sha = JSON.parse(getFileResponse.getContentText()).sha;
      fileExists = true; // 文件存在
    }

    // 获取页面的 Markdown 内容
    var markdownContent = page.markdown;

    // 如果文件存在，则获取文件内容并与新的内容比较
    if (fileExists) {
      var existingContent = Utilities.base64Decode(sha).toString();
      if (markdownContent === existingContent) {
        Logger.log("No changes for file: " + page.slug);
        return; // 跳过当前循环
      }
    }

    // 添加文件信息到tree对象
    tree.push({
      path: path + "/" + page.slug + ".md",
      mode: "100644",
      type: "blob",
      content: markdownContent,
    });
  });

  var treePayload = {
    base_tree: latestCommitSha,
    tree: tree,
  };
  var postTreeResponse = UrlFetchApp.fetch(githubApiUrl + "/git/trees", {
    method: "post",
    headers: headers,
    payload: JSON.stringify(treePayload),
    muteHttpExceptions: true,
  });
  if (postTreeResponse.getResponseCode() !== 201) {
    Logger.log("Error creating tree: " + postTreeResponse.getContentText());
    return;
  }
  var treeSha = JSON.parse(postTreeResponse.getContentText()).sha;

  // 创建一个新的commit对象，引用tree对象和父commit sha，以及提交的信息
  var commitPayload = {
    message: "GoogleAppsScript for " + path,
    tree: treeSha,
    parents: [latestCommitSha],
  };
  var postCommitResponse = UrlFetchApp.fetch(githubApiUrl + "/git/commits", {
    method: "post",
    headers: headers,
    payload: JSON.stringify(commitPayload),
    muteHttpExceptions: true,
  });
  if (postCommitResponse.getResponseCode() !== 201) {
    Logger.log("Error creating commit: " + postCommitResponse.getContentText());
    return;
  }
  var newCommitSha = JSON.parse(postCommitResponse.getContentText()).sha;

  // 更新分支的 ref，指向新的 commit sha
  var refPayload = {
    sha: newCommitSha,
  };

  var patchRefResponse = UrlFetchApp.fetch(
    githubApiUrl + "/git/refs/heads/" + branch,
    {
      method: "patch",
      headers: {
        "Content-Type": "application/json",
        Authorization: "token " + githubToken,
        "X-GitHub-Api-Version": "2022-11-28",
      },
      payload: JSON.stringify(refPayload),
      muteHttpExceptions: true,
    }
  );

  if (patchRefResponse.getResponseCode() !== 200) {
    Logger.log("Error updating ref: " + patchRefResponse.getContentText());
    return;
  }

  Logger.log("Successfully pushed to GitHub");
}

function updateMarkdownInGitHub() {
  Logger.log("updateMarkdownInGitHub called"); // 添加日志
  var pages = getNotionPages(databaseId, notionToken);
  var markdownPages = convertPagesToMarkdown(pages);
  push2GitHub(markdownPages);
  Logger.log("updateMarkdownInGitHub completed"); // 添加日志
}</code></pre>
<img src="https://images.unsplash.com/photo-1581044777550-4cfa60707c03?ixlib=rb-4.0.3&q=85&fm=jpg&crop=entropy&cs=srgb" alt="Image">
</details>