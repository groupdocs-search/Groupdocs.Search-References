---
title: "SearchResult"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "表示匹配搜索查询的搜索结果。"
type: docs
weight: 19
url: /zh/java/com.groupdocs.search.results/searchresult/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public abstract class SearchResult implements Iterable<FoundDocument>
```

表示匹配搜索查询的搜索结果。


**Learn more**

* [Searching](../https://docs.groupdocs.com/display/searchjava/Searching)
* [Search results](../https://docs.groupdocs.com/display/searchjava/Search+results)


此示例演示了该类的典型用法。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentFolder = "c:\\MyDocuments\\";
// 创建索引
Index index = new Index(indexFolder);
// 索引来自指定文件夹的文档
index.add(documentFolder);
// 设置搜索选项
SearchOptions options = new SearchOptions();
options.getFuzzySearch().setEnabled(true); // 启用模糊搜索
options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(3)); // 将最大差异数设置为 3
// 搜索包含单词 'Einstein' 或短语 'Theory of Relativity' 的文档
SearchResult result = index.search("Einstein OR \"Theory of Relativity\"", options);
// 打印结果
System.out.println("文档：" + result.getDocumentCount());
System.out.println("总出现次数：" + result.getOccurrenceCount());
for (int i = 0; i < result.getDocumentCount(); i++) {
FoundDocument document = result.getFoundDocument(i);
System.out.println("\t文档：" + document.getDocumentInfo().getFilePath());
System.out.println("\t出现次数：" + document.getOccurrenceCount());
for (int j = 0; j < document.getFoundFields().length; j++) {
FoundDocumentField field = document.getFoundFields()[j];
System.out.println("\t\t字段：" + field.getFieldName());
System.out.println("\t\t出现次数: " + document.getOccurrenceCount());
// 打印找到的术语
if (field.getTerms() != null) {
for (int k = 0; k < field.getTerms().length; k++) {
System.out.println("\t\t\t" + field.getTerms()[k] + " - " + field.getTermsOccurrences()[k]);
}
}
// 打印找到的短语
if (field.getTermSequences() != null) {
for (int k = 0; k < field.getTermSequences().length; k++) {
String[] terms = field.getTermSequences()[k];
String sequence = "";
for (int m = 0; m < terms.length; m++) {
sequence += terms[m] + " ";
}
System.out.println("\t\t\t" + sequence + " - " + field.getTermSequencesOccurrences()[k]);
}
}
}
}
 
```
 
````


## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [SearchResult()](#SearchResult--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getDocumentCount()](#getDocumentCount--) | 获取找到的文档数量。 |
|
|  | [getOccurrenceCount()](#getOccurrenceCount--) | 获取找到的总出现次数。 |
|
|  | [getTruncated()](#getTruncated--) | 获取指示结果已被截断的值。 |
|
|  | [getWarnings()](#getWarnings--) | 获取描述结果的警告。 |
|
|  | [getNextChunkSearchToken()](#getNextChunkSearchToken--) | 获取用于搜索下一个块的块搜索令牌。 |
|
|  | [getStartTime()](#getStartTime--) | 获取搜索的开始时间。 |
|
|  | [getEndTime()](#getEndTime--) | 获取搜索的结束时间。 |
|
|  | [getSearchDuration()](#getSearchDuration--) | 获取搜索持续时间（秒）。 |
|
|  | [getFoundDocument(int index)](#getFoundDocument-int-) | 按索引获取找到的文档。 |
|
|  | [iterator()](#iterator--) | 返回一个迭代器，用于遍历找到的文档集合。 |
|
### SearchResult() {#SearchResult--}
```
public SearchResult()
```


### getDocumentCount() {#getDocumentCount--}
```
public abstract int getDocumentCount()
```


获取找到的文档数量。


**Returns:**
int - 找到的文档数量。

### getOccurrenceCount() {#getOccurrenceCount--}
```
public abstract int getOccurrenceCount()
```


获取找到的总出现次数。


**Returns:**
int - 找到的总出现次数。

### getTruncated() {#getTruncated--}
```
public abstract boolean getTruncated()
```


获取指示结果已被截断的值。


**Returns:**
boolean - 指示结果已被截断的值。

### getWarnings() {#getWarnings--}
```
public abstract String getWarnings()
```


获取描述结果的警告。


**Returns:**
java.lang.String - 描述结果的警告。

### getNextChunkSearchToken() {#getNextChunkSearchToken--}
```
public abstract ChunkSearchToken getNextChunkSearchToken()
```


获取用于搜索下一个块的块搜索令牌。


**Returns:**
[ChunkSearchToken](../../com.groupdocs.search.common/chunksearchtoken) - A chunk search token for searching the next chunk.

### getStartTime() {#getStartTime--}
```
public abstract Date getStartTime()
```


获取搜索的开始时间。


**Returns:**
java.util.Date - 搜索的开始时间。

### getEndTime() {#getEndTime--}
```
public abstract Date getEndTime()
```


获取搜索的结束时间。


**Returns:**
java.util.Date - 搜索的结束时间。

### getSearchDuration() {#getSearchDuration--}
```
public abstract double getSearchDuration()
```


获取搜索持续时间（秒）。


**Returns:**
double - 搜索持续时间（秒）。

### getFoundDocument(int index) {#getFoundDocument-int-}
```
public abstract FoundDocument getFoundDocument(int index)
```


按索引获取找到的文档。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 索引 | int | 找到的文档索引。 |
|

**Returns:**
[FoundDocument](../../com.groupdocs.search.results/founddocument) - The found document.

### iterator() {#iterator--}
```
public abstract Iterator<FoundDocument> iterator()
```


返回一个迭代器，用于遍历找到的文档集合。


**Returns:**
java.util.Iterator<com.groupdocs.search.results.FoundDocument> - 可用于遍历已找到文档集合的迭代器。

