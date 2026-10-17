---
title: "NetworkImageSearchResult"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "表示匹配搜索图像的图像搜索结果。"
type: docs
weight: 12
url: /zh/java/com.groupdocs.search.scaling.results/networkimagesearchresult/
---
**Inheritance:**
java.lang.Object
```
public abstract class NetworkImageSearchResult
```

表示匹配搜索图像的图像搜索结果。

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [NetworkImageSearchResult()](#NetworkImageSearchResult--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getImageCount()](#getImageCount--) | 获取找到的图像数量。 |
|
|  | [getFoundImage(int index)](#getFoundImage-int-) | 按索引获取找到的图像。 |
|
|  | [getNetworkImageSearchToken()](#getNetworkImageSearchToken--) | 获取用于搜索下一个块的图像块搜索令牌。 |
|
|  | [getNodeIndex()](#getNodeIndex--) | 获取接收结果的节点索引。 |
|
|  | [getShardIndex()](#getShardIndex--) | 获取接收结果的分片索引。 |
|
### NetworkImageSearchResult() {#NetworkImageSearchResult--}
```
public NetworkImageSearchResult()
```


### getImageCount() {#getImageCount--}
```
public abstract int getImageCount()
```


获取找到的图像数量。


**Returns:**
int - 找到的图像数量。

### getFoundImage(int index) {#getFoundImage-int-}
```
public abstract FoundImageFrame getFoundImage(int index)
```


按索引获取找到的图像。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 索引 | int | 找到的图像索引。 |
|

**Returns:**
[FoundImageFrame](../../com.groupdocs.search.results/foundimageframe) - The found image.

### getNetworkImageSearchToken() {#getNetworkImageSearchToken--}
```
public abstract NetworkImageSearchToken getNetworkImageSearchToken()
```


获取用于搜索下一个块的图像块搜索令牌。


**Returns:**
[NetworkImageSearchToken](../../com.groupdocs.search.scaling.results/networkimagesearchtoken) - A chunk image search token for searching the next chunk.

### getNodeIndex() {#getNodeIndex--}
```
public abstract int getNodeIndex()
```


获取接收结果的节点索引。


**Returns:**
int - 接收结果的节点索引。

### getShardIndex() {#getShardIndex--}
```
public abstract int getShardIndex()
```


获取接收结果的分片索引。


**Returns:**
int - 接收结果的分片索引。

