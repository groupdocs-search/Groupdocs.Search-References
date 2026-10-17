---
title: "DocumentIndexedEventArgs"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "表示文档索引完成事件的参数。"
type: docs
weight: 12
url: /zh/java/com.groupdocs.search.scaling.events/documentindexedeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class DocumentIndexedEventArgs extends EventArgs
```

表示文档索引完成事件的参数。

## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getShardIndex()](#getShardIndex--) | 获取分片索引。 |
|
|  | [getDocumentKey()](#getDocumentKey--) | 获取文档键。 |
|
### getShardIndex() {#getShardIndex--}
```
public final int getShardIndex()
```


获取分片索引。


**Returns:**
int - 分片索引。

### getDocumentKey() {#getDocumentKey--}
```
public final String getDocumentKey()
```


获取文档键。


**Returns:**
java.lang.String - 文档键。

