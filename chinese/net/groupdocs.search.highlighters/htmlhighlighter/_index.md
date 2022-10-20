---
title: HtmlHighlighter
second_title: GroupDocs.Search for .NET API 参考
description: 表示一个搜索结果突出显示它突出显示以 HTML 格式格式化的整个文档文本中的搜索结果
type: docs
weight: 640
url: /zh/net/groupdocs.search.highlighters/htmlhighlighter/
---
## HtmlHighlighter class

表示一个搜索结果突出显示，它突出显示以 HTML 格式格式化的整个文档文本中的搜索结果。

```csharp
public class HtmlHighlighter : Highlighter
```

## 构造函数

| 姓名 | 描述 |
| --- | --- |
| [HtmlHighlighter](htmlhighlighter)(OutputAdapter) | 初始化[`HtmlHighlighter`](../htmlhighlighter)类. |

## 特性

| 姓名 | 描述 |
| --- | --- |
| [OutputAdapter](../../groupdocs.search.highlighters/htmlhighlighter/outputadapter) { get; } | 获取构造函数中传入的输出适配器。 |

### 评论

**学到更多**

* [突出显示搜索结果](https://docs.groupdocs.com/display/searchnet/Highlighting+search+results)

### 例子

该示例演示了类的典型用法。

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

// 创建索引
Index index = new Index(indexFolder);

// 索引指定文件夹中的文档
index.Add(documentsFolder);

// 搜索“相对论”阶段
SearchResult result = index.Search("\"Theory of Relativity\"");

// 突出显示文档文本中找到的单词
FoundDocument document = result.GetFoundDocument(0);
OutputAdapter outputAdapter = new FileOutputAdapter("Highlighted.html");
Highlighter highlighter = new HtmlHighlighter(outputAdapter);
index.Highlight(document, highlighter);
```

### 也可以看看

* class [Highlighter](../highlighter)
* 命名空间 [GroupDocs.Search.Highlighters](../../groupdocs.search.highlighters)
* 部件 [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->