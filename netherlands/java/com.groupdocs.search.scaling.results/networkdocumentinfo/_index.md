---
title: "NetworkDocumentInfo"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Stelt een descriptor voor een geïndexeerd document in het zoeknetwerk voor."
type: docs
weight: 10
url: /nl/java/com.groupdocs.search.scaling.results/networkdocumentinfo/
---
**Inheritance:**
java.lang.Object
```
public abstract class NetworkDocumentInfo
```

Stelt een descriptor voor een geïndexeerd document in het zoeknetwerk voor.

## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [NetworkDocumentInfo()](#NetworkDocumentInfo--) |  |
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getDocumentInfo()](#getDocumentInfo--) | Haalt de descriptor op voor een geïndexeerd document. |
|
|  | [getShardIndex()](#getShardIndex--) | Haalt de shard-index op. |
|
### NetworkDocumentInfo() {#NetworkDocumentInfo--}
```
public NetworkDocumentInfo()
```


### getDocumentInfo() {#getDocumentInfo--}
```
public abstract DocumentInfo getDocumentInfo()
```


Haalt de descriptor op voor een geïndexeerd document.


**Returns:**
[DocumentInfo](../../com.groupdocs.search.results/documentinfo) - The descriptor for an indexed document.

### getShardIndex() {#getShardIndex--}
```
public abstract int getShardIndex()
```


Haalt de shard-index op.


**Returns:**
int - De shard-index.

