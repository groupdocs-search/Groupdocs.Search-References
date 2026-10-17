---
title: "FileLogger"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "表示将事件和错误记录到本地文件的日志记录器。"
type: docs
weight: 20
url: /zh/java/com.groupdocs.search.common/filelogger/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.search.common.ILogger](../../com.groupdocs.search.common/ilogger)
```
public class FileLogger implements ILogger
```

表示将事件和错误记录到本地文件的日志记录器。


**Learn more**

* [Logging](../https://docs.groupdocs.com/display/searchjava/Logging)


此示例演示了该类的典型用法。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
String logPath = "c:\\Log.txt";
IndexSettings settings = new IndexSettings();
settings.setLogger(new FileLogger(logPath, 4.0)); // 指定日志文件路径以及 4 MB 的最大长度
Index index = new Index(indexFolder, settings); // 在指定文件夹中创建索引
index.add(documentsFolder); // 从指定文件夹索引文档
SearchResult result = index.search(query); // 在索引中搜索
 
```
 
````


## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [FileLogger(String filePath, double maxSize)](#FileLogger-java.lang.String-double-) | 初始化 FileLogger 类的新实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [error(String message)](#error-java.lang.String-) | 记录在索引中发生的错误。 |
|
|  | [trace(String message)](#trace-java.lang.String-) | 记录在索引中发生的事件。 |
|
|  | [getFilePath()](#getFilePath--) | 获取日志文件路径。 |
|
|  | [getMaxSize()](#getMaxSize--) | 获取日志文件的最大大小（单位：兆字节）。 |
|
### FileLogger(String filePath, double maxSize) {#FileLogger-java.lang.String-double-}
```
public FileLogger(String filePath, double maxSize)
```


初始化 FileLogger 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 文件路径 | java.lang.String | 日志文件路径。 |
|
|  | maxSize | double | 日志文件的最大大小（单位：兆字节）。该值必须在 0.1 到 1000 的范围内。 |
|

### error(String message) {#error-java.lang.String-}
```
public final void error(String message)
```


记录在索引中发生的错误。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | message | java.lang.String | 错误消息。 |
|

### trace(String message) {#trace-java.lang.String-}
```
public final void trace(String message)
```


记录在索引中发生的事件。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | message | java.lang.String | 事件消息。 |
|

### getFilePath() {#getFilePath--}
```
public final String getFilePath()
```


获取日志文件路径。


**Returns:**
java.lang.String - 日志文件路径。

### getMaxSize() {#getMaxSize--}
```
public final double getMaxSize()
```


获取日志文件的最大大小（单位：兆字节）。


**Returns:**
double - 日志文件的最大大小（单位：兆字节）。

