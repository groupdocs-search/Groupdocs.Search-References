---
title: NetworkImageSearchResult
second_title: GroupDocs.Search for Java API Reference
description: Represents an image search result matching a search image.
type: docs
weight: 12
url: /java/com.groupdocs.search.scaling.results/networkimagesearchresult/
---
**Inheritance:**
java.lang.Object
```
public abstract class NetworkImageSearchResult
```

Represents an image search result matching a search image.
## Constructors

| Constructor | Description |
| --- | --- |
| [NetworkImageSearchResult()](#NetworkImageSearchResult--) |  |
## Methods

| Method | Description |
| --- | --- |
| [getImageCount()](#getImageCount--) | Gets the number of images found. |
| [getFoundImage(int index)](#getFoundImage-int-) | Gets the found image by index. |
| [getNetworkImageSearchToken()](#getNetworkImageSearchToken--) | Gets a chunk image search token for searching the next chunk. |
| [getNodeIndex()](#getNodeIndex--) | Gets the index of the node from which the result was received. |
| [getShardIndex()](#getShardIndex--) | Gets the index of the shard from which the result was received. |
### NetworkImageSearchResult() {#NetworkImageSearchResult--}
```
public NetworkImageSearchResult()
```


### getImageCount() {#getImageCount--}
```
public abstract int getImageCount()
```


Gets the number of images found.

**Returns:**
int - The number of images found.
### getFoundImage(int index) {#getFoundImage-int-}
```
public abstract FoundImageFrame getFoundImage(int index)
```


Gets the found image by index.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The index of a found image. |

**Returns:**
[FoundImageFrame](../../com.groupdocs.search.results/foundimageframe) - The found image.
### getNetworkImageSearchToken() {#getNetworkImageSearchToken--}
```
public abstract NetworkImageSearchToken getNetworkImageSearchToken()
```


Gets a chunk image search token for searching the next chunk.

**Returns:**
[NetworkImageSearchToken](../../com.groupdocs.search.scaling.results/networkimagesearchtoken) - A chunk image search token for searching the next chunk.
### getNodeIndex() {#getNodeIndex--}
```
public abstract int getNodeIndex()
```


Gets the index of the node from which the result was received.

**Returns:**
int - The index of the node from which the result was received.
### getShardIndex() {#getShardIndex--}
```
public abstract int getShardIndex()
```


Gets the index of the shard from which the result was received.

**Returns:**
int - The index of the shard from which the result was received.
