---
title: "IndexingReport"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "表示索引操作的详细信息。"
type: docs
weight: 25
url: /zh/java/com.groupdocs.search.common/indexingreport/
---
**Inheritance:**
java.lang.Object
```
public abstract class IndexingReport
```

表示索引操作的详细信息。


**Learn more**

* [Indexing reports](../https://docs.groupdocs.com/display/searchjava/Indexing+reports)


此示例演示了该类的典型用法。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder1 = "c:\\MyDocuments1\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
// 在指定文件夹中创建索引
Index index = new Index(indexFolder);
// 索引文档
index.add(documentsFolder1);
index.add(documentsFolder2);
// 获取索引报告
IndexingReport[] reports = index.getIndexingReports();
// 将报告打印到控制台
for (IndexingReport report : reports) {
DateFormat df = new SimpleDateFormat("MM/dd/yyyy HH:mm:ss");
System.out.println(\"时间: \" + df.format(report.getStartTime()));
System.out.println(\"持续时间: \" + report.getIndexingTime());
System.out.println(\"文档总数: \" + report.getTotalDocumentsInIndex());
System.out.println(\"词项总数: \" + report.getTotalTermCount());
System.out.println(\"已索引文档大小（MB）: \" + report.getIndexedDocumentsSize());
System.out.println(\"索引大小（MB）: \" + (report.getTotalIndexSize() / 1024.0 / 1024.0));
System.out.println();
}
 
```
 
````


## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [IndexingReport()](#IndexingReport--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getTotalDocumentsInIndex()](#getTotalDocumentsInIndex--) | 获取索引中文档的总数。 |
|
|  | [getTotalTermCount()](#getTotalTermCount--) | 获取索引中词项的总数。 |
|
|  | [getIndexedDocumentsSize()](#getIndexedDocumentsSize--) | 获取已索引文档的总长度（MB）。 |
|
|  | [getSegmentCount()](#getSegmentCount--) | 获取索引段的数量。 |
|
|  | [getTotalIndexSize()](#getTotalIndexSize--) | 获取索引的总大小（字节）。 |
|
|  | [getStartTime()](#getStartTime--) | 获取索引开始时间。 |
|
|  | [getEndTime()](#getEndTime--) | 获取索引结束时间。 |
|
|  | [getIndexingTime()](#getIndexingTime--) | 获取索引持续时间（秒）。 |
|
|  | [getErrors()](#getErrors--) | 获取错误列表。 |
|
|  | [getIndexedDocuments()](#getIndexedDocuments--) | 获取已索引文档列表。 |
|
|  | [getUpdatedDocuments()](#getUpdatedDocuments--) | 获取已更新文档的列表。 |
|
|  | [getRemovedDocuments()](#getRemovedDocuments--) | 获取已从索引中移除的文档列表。 |
|
### IndexingReport() {#IndexingReport--}
```
public IndexingReport()
```


### getTotalDocumentsInIndex() {#getTotalDocumentsInIndex--}
```
public abstract int getTotalDocumentsInIndex()
```


获取索引中文档的总数。


**Returns:**
int - 索引中文档的总数。

### getTotalTermCount() {#getTotalTermCount--}
```
public abstract int getTotalTermCount()
```


获取索引中词项的总数。


**Returns:**
int - 索引中术语的总数。

### getIndexedDocumentsSize() {#getIndexedDocumentsSize--}
```
public abstract double getIndexedDocumentsSize()
```


获取已索引文档的总长度（MB）。


**Returns:**
double - 已索引文档的总长度（单位：MB）。

### getSegmentCount() {#getSegmentCount--}
```
public abstract int getSegmentCount()
```


获取索引段的数量。


**Returns:**
int - 索引段的数量。

### getTotalIndexSize() {#getTotalIndexSize--}
```
public abstract long getTotalIndexSize()
```


获取索引的总大小（字节）。


**Returns:**
long - 索引的总大小（单位：字节）。

### getStartTime() {#getStartTime--}
```
public abstract Date getStartTime()
```


获取索引开始时间。


**Returns:**
java.util.Date - 索引开始时间。

### getEndTime() {#getEndTime--}
```
public abstract Date getEndTime()
```


获取索引结束时间。


**Returns:**
java.util.Date - 索引结束时间。

### getIndexingTime() {#getIndexingTime--}
```
public abstract double getIndexingTime()
```


获取索引持续时间（秒）。


**Returns:**
double - 索引持续时间（单位：秒）。

### getErrors() {#getErrors--}
```
public abstract String[] getErrors()
```


获取错误列表。


**Returns:**
java.lang.String[] - 错误列表。

### getIndexedDocuments() {#getIndexedDocuments--}
```
public abstract String[] getIndexedDocuments()
```


获取已索引文档列表。


**Returns:**
java.lang.String[] - 已索引文档的列表。

### getUpdatedDocuments() {#getUpdatedDocuments--}
```
public abstract String[] getUpdatedDocuments()
```


获取已更新文档的列表。


**Returns:**
java.lang.String[] - 已更新文档的列表。

### getRemovedDocuments() {#getRemovedDocuments--}
```
public abstract String[] getRemovedDocuments()
```


获取已从索引中移除的文档列表。


**Returns:**
java.lang.String[] - 已从索引中移除的文档列表。

