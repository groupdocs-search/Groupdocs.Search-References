---
title: "NetworkDocumentInfo"
second_title: "GroupDocs.Search för Java API-referens"
description: "Representerar en beskrivning för ett indexerat dokument i söknätverket."
type: docs
weight: 10
url: /sv/java/com.groupdocs.search.scaling.results/networkdocumentinfo/
---
**Inheritance:**
java.lang.Object
```
public abstract class NetworkDocumentInfo
```

Representerar en beskrivning för ett indexerat dokument i söknätverket.

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [NetworkDocumentInfo()](#NetworkDocumentInfo--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getDocumentInfo()](#getDocumentInfo--) | Hämtar beskrivningen för ett indexerat dokument. |
|
|  | [getShardIndex()](#getShardIndex--) | Hämtar fragmentets index. |
|
### NetworkDocumentInfo() {#NetworkDocumentInfo--}
```
public NetworkDocumentInfo()
```


### getDocumentInfo() {#getDocumentInfo--}
```
public abstract DocumentInfo getDocumentInfo()
```


Hämtar beskrivningen för ett indexerat dokument.


**Returns:**
[DocumentInfo](../../com.groupdocs.search.results/documentinfo) - The descriptor for an indexed document.

### getShardIndex() {#getShardIndex--}
```
public abstract int getShardIndex()
```


Hämtar fragmentets index.


**Returns:**
int - Fragmentets index.

