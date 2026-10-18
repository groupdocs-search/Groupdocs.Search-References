---
title: "NetworkDocumentInfo"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Stellt einen Deskriptor für ein indiziertes Dokument im Suchnetzwerk dar."
type: docs
weight: 10
url: /de/java/com.groupdocs.search.scaling.results/networkdocumentinfo/
---
**Inheritance:**
java.lang.Object
```
public abstract class NetworkDocumentInfo
```

Stellt einen Deskriptor für ein indiziertes Dokument im Suchnetzwerk dar.

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [NetworkDocumentInfo()](#NetworkDocumentInfo--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getDocumentInfo()](#getDocumentInfo--) | Liefert den Deskriptor für ein indiziertes Dokument. |
|
|  | [getShardIndex()](#getShardIndex--) | Ermittelt den Shard-Index. |
|
### NetworkDocumentInfo() {#NetworkDocumentInfo--}
```
public NetworkDocumentInfo()
```


### getDocumentInfo() {#getDocumentInfo--}
```
public abstract DocumentInfo getDocumentInfo()
```


Liefert den Deskriptor für ein indiziertes Dokument.


**Returns:**
[DocumentInfo](../../com.groupdocs.search.results/documentinfo) - The descriptor for an indexed document.

### getShardIndex() {#getShardIndex--}
```
public abstract int getShardIndex()
```


Ermittelt den Shard-Index.


**Returns:**
int - Der Shard-Index.

