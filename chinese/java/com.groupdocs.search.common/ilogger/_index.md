---
title: "ILogger"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "定义用于在索引中记录事件和错误的日志记录器接口。"
type: docs
weight: 38
url: /zh/java/com.groupdocs.search.common/ilogger/
---```
public interface ILogger
```

Defines interface of a logger that is used for logging events and errors in an index.


**Learn more**

* [Logging](../https://docs.groupdocs.com/display/searchjava/Logging)

## Methods

| Method | Description |
| --- | --- |
| [error(String message)](#error-java.lang.String-) | Logs an error that occurred in the index.
 |
| [trace(String message)](#trace-java.lang.String-) | Logs an event that occurred in the index.
 |
### error(String message) {#error-java.lang.String-}
```
public abstract void error(String message)
```


Logs an error that occurred in the index.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| message | java.lang.String | The error message.
 |

### trace(String message) {#trace-java.lang.String-}
```
public abstract void trace(String message)
```


Logs an event that occurred in the index.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| message | java.lang.String | The event message.
 |

