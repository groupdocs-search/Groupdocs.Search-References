---
title: "BaseIndexEventArgs"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "表示事件参数的基类。"
type: docs
weight: 10
url: /zh/java/com.groupdocs.search.events/baseindexeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class BaseIndexEventArgs extends EventArgs
```

表示事件参数的基类。


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getTime()](#getTime--) | 获取事件的时间。 |
|
|  | [getIndexId()](#getIndexId--) | 获取索引 ID。 |
|
|  | [getIndexFolder()](#getIndexFolder--) | 获取索引文件夹。 |
|
|  | [getStatus()](#getStatus--) | 获取索引状态。 |
|
### getTime() {#getTime--}
```
public final Date getTime()
```


获取事件的时间。


**Returns:**
java.util.Date - 事件的时间。

### getIndexId() {#getIndexId--}
```
public final UUID getIndexId()
```


获取索引 ID。


**Returns:**
java.util.UUID - 索引 ID。

### getIndexFolder() {#getIndexFolder--}
```
public final String getIndexFolder()
```


获取索引文件夹。


**Returns:**
java.lang.String - 索引文件夹。

### getStatus() {#getStatus--}
```
public final IndexStatus getStatus()
```


获取索引状态。


**Returns:**
[IndexStatus](../../com.groupdocs.search.common/indexstatus) - The index status.

