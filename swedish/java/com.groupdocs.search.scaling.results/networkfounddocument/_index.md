---
title: "NetworkFoundDocument"
second_title: "GroupDocs.Search för Java API-referens"
description: "Representerar ett hittat dokument i söknätverket."
type: docs
weight: 11
url: /sv/java/com.groupdocs.search.scaling.results/networkfounddocument/
---
**Inheritance:**
java.lang.Object
```
public abstract class NetworkFoundDocument
```

Representerar ett hittat dokument i söknätverket.

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [NetworkFoundDocument()](#NetworkFoundDocument--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getFoundDocument()](#getFoundDocument--) | Hämtar det hittade dokumentet. |
|
|  | [getShardIndex()](#getShardIndex--) | Hämtar fragmentets index. |
|
### NetworkFoundDocument() {#NetworkFoundDocument--}
```
public NetworkFoundDocument()
```


### getFoundDocument() {#getFoundDocument--}
```
public abstract FoundDocument getFoundDocument()
```


Hämtar det hittade dokumentet.


**Returns:**
[FoundDocument](../../com.groupdocs.search.results/founddocument) - The found document.

### getShardIndex() {#getShardIndex--}
```
public abstract int getShardIndex()
```


Hämtar fragmentets index.


**Returns:**
int - Fragmentets index.

