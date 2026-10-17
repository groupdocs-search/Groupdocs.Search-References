---
title: "SearchReport"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "表示搜索操作的详细信息。"
type: docs
weight: 30
url: /zh/java/com.groupdocs.search.common/searchreport/
---
**Inheritance:**
java.lang.Object
```
public abstract class SearchReport
```

表示搜索操作的详细信息。


**Learn more**

* [Search reports](../https://docs.groupdocs.com/display/searchjava/Search+reports)


此示例演示了该类的典型用法。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// 在指定文件夹中创建索引
Index index = new Index(indexFolder);
// 索引来自指定文件夹的文档
index.add(documentsFolder);
// 在索引中搜索
SearchResult result1 = index.search("Einstein");
SearchResult result2 = index.search("\"Theory of Relativity\"");
// 获取搜索报告
SearchReport[] reports = index.getSearchReports();
// 将报告打印到控制台
for (SearchReport report : reports) {
System.out.println("Query: " + report.getTextQuery());
DateFormat df = new SimpleDateFormat("MM/dd/yyyy HH:mm:ss");
System.out.println(\"时间: \" + df.format(report.getStartTime()));
System.out.println("Duration: " + report.getSearchDuration());
System.out.println("Documents: " + report.getDocumentCount());
System.out.println("Occurrences: " + report.getOccurrenceCount());
System.out.println();
}
 
```
 
````


## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [SearchReport()](#SearchReport--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getStartTime()](#getStartTime--) | 获取搜索的开始时间。 |
|
|  | [getEndTime()](#getEndTime--) | 获取搜索的结束时间。 |
|
|  | [getSearchDuration()](#getSearchDuration--) | 获取搜索持续时间（秒）。 |
|
|  | [getDocumentCount()](#getDocumentCount--) | 获取找到的文档数量。 |
|
|  | [getOccurrenceCount()](#getOccurrenceCount--) | 获取找到的总出现次数。 |
|
|  | [getTextQuery()](#getTextQuery--) | 获取文本形式的搜索查询。 |
|
|  | [getObjectQuery()](#getObjectQuery--) | 获取对象形式的搜索查询。 |
|
|  | [getSearchOptions()](#getSearchOptions--) | 获取搜索选项。 |
|
|  | [toString()](#toString--) | 返回一个表示当前  SearchReport 的字符串。 |
|
### SearchReport() {#SearchReport--}
```
public SearchReport()
```


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

### getTextQuery() {#getTextQuery--}
```
public abstract String getTextQuery()
```


获取文本形式的搜索查询。


**Returns:**
java.lang.String - 文本形式的搜索查询。

### getObjectQuery() {#getObjectQuery--}
```
public abstract SearchQuery getObjectQuery()
```


获取对象形式的搜索查询。


**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - The search query in object form.

### getSearchOptions() {#getSearchOptions--}
```
public abstract SearchOptions getSearchOptions()
```


获取搜索选项。


**Returns:**
[SearchOptions](../../com.groupdocs.search.options/searchoptions) - The search options.

### toString() {#toString--}
```
public abstract String toString()
```


返回一个表示当前  SearchReport 的字符串。


**Returns:**
java.lang.String - 表示当前 SearchReport 的字符串。

