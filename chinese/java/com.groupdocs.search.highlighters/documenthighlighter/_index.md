---
title: "DocumentHighlighter"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "表示在整个文档文本中突出显示搜索结果的搜索结果高亮器。"
type: docs
weight: 10
url: /zh/java/com.groupdocs.search.highlighters/documenthighlighter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.highlighters.Highlighter](../../com.groupdocs.search.highlighters/highlighter)

**All Implemented Interfaces:**
[com.groupdocs.search.highlighters.IDocumentHighlighter](../../com.groupdocs.search.highlighters/idocumenthighlighter)
```
public class DocumentHighlighter extends Highlighter implements IDocumentHighlighter
```

表示在整个文档文本中突出显示搜索结果的搜索结果高亮器。


**Learn more**

* [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)


此示例演示了该类的典型用法。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// 创建索引
Index index = new Index(indexFolder);
// 索引来自指定文件夹的文档
index.add(documentsFolder);
// 搜索短语 'Theory of Relativity'
SearchResult result = index.search("\"Theory of Relativity\"");
// 高亮文档文本中找到的单词
FoundDocument document = result.getFoundDocument(0);
OutputAdapter outputAdapter = new FileOutputAdapter(OutputFormat.Html, "Highlighted.html");
Highlighter highlighter = new DocumentHighlighter(outputAdapter);
index.highlight(document, highlighter);
 
```
 
````


## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [DocumentHighlighter(OutputAdapter outputAdapter)](#DocumentHighlighter-com.groupdocs.search.common.OutputAdapter-) | 初始化 DocumentHighlighter 类的新实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getOutputAdapter()](#getOutputAdapter--) | 获取在构造函数中传入的输出适配器。 |
|
### DocumentHighlighter(OutputAdapter outputAdapter) {#DocumentHighlighter-com.groupdocs.search.common.OutputAdapter-}
```
public DocumentHighlighter(OutputAdapter outputAdapter)
```


初始化 DocumentHighlighter 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | outputAdapter | [OutputAdapter](../../com.groupdocs.search.common/outputadapter) | 输出适配器传输高亮的结果。 |
|

### getOutputAdapter() {#getOutputAdapter--}
```
public final OutputAdapter getOutputAdapter()
```


获取在构造函数中传入的输出适配器。


**Returns:**
[OutputAdapter](../../com.groupdocs.search.common/outputadapter) - The output adapter passed in the constructor.

