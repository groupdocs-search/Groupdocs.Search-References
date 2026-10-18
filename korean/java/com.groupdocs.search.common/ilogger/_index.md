---
title: "ILogger"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "인덱스에서 이벤트와 오류를 기록하는 데 사용되는 로거 인터페이스를 정의합니다."
type: docs
weight: 38
url: /ko/java/com.groupdocs.search.common/ilogger/
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

