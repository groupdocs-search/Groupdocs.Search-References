---
title: "NetworkFoundDocument"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Stelt een gevonden document in het zoeknetwerk voor."
type: docs
weight: 11
url: /nl/java/com.groupdocs.search.scaling.results/networkfounddocument/
---
**Inheritance:**
java.lang.Object
```
public abstract class NetworkFoundDocument
```

Stelt een gevonden document in het zoeknetwerk voor.

## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [NetworkFoundDocument()](#NetworkFoundDocument--) |  |
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getFoundDocument()](#getFoundDocument--) | Haalt het gevonden document op. |
|
|  | [getShardIndex()](#getShardIndex--) | Haalt de shard-index op. |
|
### NetworkFoundDocument() {#NetworkFoundDocument--}
```
public NetworkFoundDocument()
```


### getFoundDocument() {#getFoundDocument--}
```
public abstract FoundDocument getFoundDocument()
```


Haalt het gevonden document op.


**Returns:**
[FoundDocument](../../com.groupdocs.search.results/founddocument) - The found document.

### getShardIndex() {#getShardIndex--}
```
public abstract int getShardIndex()
```


Haalt de shard-index op.


**Returns:**
int - De shard-index.

