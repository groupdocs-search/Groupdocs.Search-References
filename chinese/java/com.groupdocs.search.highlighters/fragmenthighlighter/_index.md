---
title: "FragmentHighlighter"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "表示在文本片段中突出显示搜索结果的搜索结果高亮器。"
type: docs
weight: 11
url: /zh/java/com.groupdocs.search.highlighters/fragmenthighlighter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.highlighters.Highlighter](../../com.groupdocs.search.highlighters/highlighter)

**All Implemented Interfaces:**
[com.groupdocs.search.highlighters.IFragmentHighlighter](../../com.groupdocs.search.highlighters/ifragmenthighlighter)
```
public class FragmentHighlighter extends Highlighter implements IFragmentHighlighter
```

表示在文本片段中突出显示搜索结果的搜索结果高亮器。


**Learn more**

* [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// 创建索引
Index index = new Index(indexFolder);
// 索引来自指定文件夹的文档
index.add(documentsFolder);
// 搜索单词 'Einstein'
SearchResult result = index.search("Einstein");
// 设置高亮选项
HighlightOptions options = new HighlightOptions();
options.setTermsBefore(5);
options.setTermsAfter(5);
options.setTermsTotal(15);
// 高亮文档文本中找到的单词
FoundDocument document = result.getFoundDocument(0);
FragmentHighlighter highlighter = new FragmentHighlighter(OutputFormat.Html);
index.highlight(document, highlighter, options);
// 获取结果
FragmentContainer[] fragmentContainers = highlighter.getResult();
for (int i = 0; i < fragmentContainers.length; i++) {
FragmentContainer container = fragmentContainers[i];
String[] fragments = container.getFragments();
if (fragments.length > 0) {
System.out.println(container.getFieldName());
System.out.println();
for (int j = 0; j < fragments.length; j++) {
// 打印 HTML 标记到控制台
System.out.println(fragments[j]);
System.out.println();
}
}
}
 
```
 
````


## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [FragmentHighlighter(OutputFormat outputFormat)](#FragmentHighlighter-com.groupdocs.search.options.OutputFormat-) | 初始化 FragmentHighlighter 类的新实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getResult()](#getResult--) | 获取结果片段容器的数组。 |
|
### FragmentHighlighter(OutputFormat outputFormat) {#FragmentHighlighter-com.groupdocs.search.options.OutputFormat-}
```
public FragmentHighlighter(OutputFormat outputFormat)
```


初始化 FragmentHighlighter 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | outputFormat | [OutputFormat](../../com.groupdocs.search.options/outputformat) | 输出格式。 |
|

### getResult() {#getResult--}
```
public final FragmentContainer[] getResult()
```


获取结果片段容器的数组。


**Returns:**
com.groupdocs.search.common.FragmentContainer[] - 结果片段容器的数组。

