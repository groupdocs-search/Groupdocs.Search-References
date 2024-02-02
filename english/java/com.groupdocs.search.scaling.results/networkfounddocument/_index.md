---
title: NetworkFoundDocument
second_title: GroupDocs.Search for Java API Reference
description: Represents a found document in the search network.
type: docs
weight: 11
url: /java/com.groupdocs.search.scaling.results/networkfounddocument/
---
**Inheritance:**
java.lang.Object
```
public abstract class NetworkFoundDocument
```

Represents a found document in the search network.
## Constructors

| Constructor | Description |
| --- | --- |
| [NetworkFoundDocument()](#NetworkFoundDocument--) |  |
## Methods

| Method | Description |
| --- | --- |
| [getFoundDocument()](#getFoundDocument--) | Gets the found document. |
| [getShardIndex()](#getShardIndex--) | Gets the shard index. |
### NetworkFoundDocument() {#NetworkFoundDocument--}
```
public NetworkFoundDocument()
```


### getFoundDocument() {#getFoundDocument--}
```
public abstract FoundDocument getFoundDocument()
```


Gets the found document.

**Returns:**
[FoundDocument](../../com.groupdocs.search.results/founddocument) - The found document.
### getShardIndex() {#getShardIndex--}
```
public abstract int getShardIndex()
```


Gets the shard index.

**Returns:**
int - The shard index.
