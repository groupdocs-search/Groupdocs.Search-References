---
title: "IndexErrorEventArgs"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "表示索引错误发生事件的参数。"
type: docs
weight: 16
url: /zh/java/com.groupdocs.search.events/indexerroreventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class IndexErrorEventArgs extends BaseIndexEventArgs
```

表示索引错误发生事件的参数。


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getMessage()](#getMessage--) | 获取错误信息。 |
|
|  | [isCritical()](#isCritical--) | 获取一个标志，指示发生的错误是关键的，并且应重新启动索引。 |
|
### getMessage() {#getMessage--}
```
public final String getMessage()
```


获取错误信息。


**Returns:**
java.lang.String - 错误信息。

### isCritical() {#isCritical--}
```
public final boolean isCritical()
```


获取一个标志，指示发生的错误是关键的，并且应重新启动索引。


**Returns:**
boolean - 指示发生的错误是关键的并且应重新启动索引的标志。

