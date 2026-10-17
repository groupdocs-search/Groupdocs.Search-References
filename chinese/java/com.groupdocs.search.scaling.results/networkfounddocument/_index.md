---
title: "NetworkFoundDocument"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "表示搜索网络中找到的文档。"
type: docs
weight: 11
url: /zh/java/com.groupdocs.search.scaling.results/networkfounddocument/
---
**Inheritance:**
java.lang.Object
```
public abstract class NetworkFoundDocument
```

表示搜索网络中找到的文档。

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [NetworkFoundDocument()](#NetworkFoundDocument--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getFoundDocument()](#getFoundDocument--) | 获取找到的文档。 |
|
|  | [getShardIndex()](#getShardIndex--) | 获取分片索引。 |
|
### NetworkFoundDocument() {#NetworkFoundDocument--}
```
public NetworkFoundDocument()
```


### getFoundDocument() {#getFoundDocument--}
```
public abstract FoundDocument getFoundDocument()
```


获取找到的文档。


**Returns:**
[FoundDocument](../../com.groupdocs.search.results/founddocument) - The found document.

### getShardIndex() {#getShardIndex--}
```
public abstract int getShardIndex()
```


获取分片索引。


**Returns:**
int - 分片索引。

