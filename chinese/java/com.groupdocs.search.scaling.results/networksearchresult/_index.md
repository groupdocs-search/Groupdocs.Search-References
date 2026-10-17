---
title: "NetworkSearchResult"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "表示匹配搜索查询的搜索结果。"
type: docs
weight: 14
url: /zh/java/com.groupdocs.search.scaling.results/networksearchresult/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public abstract class NetworkSearchResult implements Iterable<NetworkFoundDocument>
```

表示匹配搜索查询的搜索结果。

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [NetworkSearchResult()](#NetworkSearchResult--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getDocumentCount()](#getDocumentCount--) | 获取找到的文档数量。 |
|
|  | [getOccurrenceCount()](#getOccurrenceCount--) | 获取找到的总出现次数。 |
|
|  | [getTruncated()](#getTruncated--) | 获取指示结果已被截断的值。 |
|
|  | [getWarnings()](#getWarnings--) | 获取描述结果的警告。 |
|
|  | [getStartTime()](#getStartTime--) | 获取搜索的开始时间。 |
|
|  | [getEndTime()](#getEndTime--) | 获取搜索的结束时间。 |
|
|  | [getSearchDuration()](#getSearchDuration--) | 获取搜索持续时间（秒）。 |
|
|  | [getFoundDocument(int index)](#getFoundDocument-int-) | 按索引获取找到的文档。 |
|
|  | [iterator()](#iterator--) | 返回一个迭代器，用于遍历找到的文档集合。 |
|
|  | [getNextChunkSearchToken()](#getNextChunkSearchToken--) | 获取用于搜索下一个块的块搜索令牌。 |
|
|  | [getNodeIndex()](#getNodeIndex--) | 获取接收结果的节点索引。 |
|
### NetworkSearchResult() {#NetworkSearchResult--}
```
public NetworkSearchResult()
```


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

### getTruncated() {#getTruncated--}
```
public abstract boolean getTruncated()
```


获取指示结果已被截断的值。


**Returns:**
boolean - 指示结果已被截断的值。

### getWarnings() {#getWarnings--}
```
public abstract String getWarnings()
```


获取描述结果的警告。


**Returns:**
java.lang.String - 描述结果的警告。

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

### getFoundDocument(int index) {#getFoundDocument-int-}
```
public abstract NetworkFoundDocument getFoundDocument(int index)
```


按索引获取找到的文档。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 索引 | int | 找到的文档索引。 |
|

**Returns:**
[NetworkFoundDocument](../../com.groupdocs.search.scaling.results/networkfounddocument) - The found document.

### iterator() {#iterator--}
```
public abstract Iterator<NetworkFoundDocument> iterator()
```


返回一个迭代器，用于遍历找到的文档集合。


**Returns:**
java.util.Iterator<com.groupdocs.search.scaling.results.NetworkFoundDocument> - 可用于遍历找到的文档集合的迭代器。

### getNextChunkSearchToken() {#getNextChunkSearchToken--}
```
public abstract NetworkSearchToken getNextChunkSearchToken()
```


获取用于搜索下一个块的块搜索令牌。


**Returns:**
[NetworkSearchToken](../../com.groupdocs.search.scaling.results/networksearchtoken) - A chunk search token for searching the next chunk.

### getNodeIndex() {#getNodeIndex--}
```
public abstract int getNodeIndex()
```


获取接收结果的节点索引。


**Returns:**
int - 接收结果的节点索引。

