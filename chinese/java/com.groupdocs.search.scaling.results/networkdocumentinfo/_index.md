---
title: "NetworkDocumentInfo"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "表示搜索网络中已索引文档的描述符。"
type: docs
weight: 10
url: /zh/java/com.groupdocs.search.scaling.results/networkdocumentinfo/
---
**Inheritance:**
java.lang.Object
```
public abstract class NetworkDocumentInfo
```

表示搜索网络中已索引文档的描述符。

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [NetworkDocumentInfo()](#NetworkDocumentInfo--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getDocumentInfo()](#getDocumentInfo--) | 获取已索引文档的描述符。 |
|
|  | [getShardIndex()](#getShardIndex--) | 获取分片索引。 |
|
### NetworkDocumentInfo() {#NetworkDocumentInfo--}
```
public NetworkDocumentInfo()
```


### getDocumentInfo() {#getDocumentInfo--}
```
public abstract DocumentInfo getDocumentInfo()
```


获取已索引文档的描述符。


**Returns:**
[DocumentInfo](../../com.groupdocs.search.results/documentinfo) - The descriptor for an indexed document.

### getShardIndex() {#getShardIndex--}
```
public abstract int getShardIndex()
```


获取分片索引。


**Returns:**
int - 分片索引。

