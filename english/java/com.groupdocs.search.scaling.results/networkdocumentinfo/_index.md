---
title: NetworkDocumentInfo
second_title: GroupDocs.Search for Java API Reference
description: Represents a descriptor for an indexed document in the search network.
type: docs
weight: 10
url: /java/com.groupdocs.search.scaling.results/networkdocumentinfo/
---
**Inheritance:**
java.lang.Object
```
public abstract class NetworkDocumentInfo
```

Represents a descriptor for an indexed document in the search network.
## Constructors

| Constructor | Description |
| --- | --- |
| [NetworkDocumentInfo()](#NetworkDocumentInfo--) |  |
## Methods

| Method | Description |
| --- | --- |
| [getDocumentInfo()](#getDocumentInfo--) | Gets the descriptor for an indexed document. |
| [getShardIndex()](#getShardIndex--) | Gets the shard index. |
### NetworkDocumentInfo() {#NetworkDocumentInfo--}
```
public NetworkDocumentInfo()
```


### getDocumentInfo() {#getDocumentInfo--}
```
public abstract DocumentInfo getDocumentInfo()
```


Gets the descriptor for an indexed document.

**Returns:**
[DocumentInfo](../../com.groupdocs.search.results/documentinfo) - The descriptor for an indexed document.
### getShardIndex() {#getShardIndex--}
```
public abstract int getShardIndex()
```


Gets the shard index.

**Returns:**
int - The shard index.
