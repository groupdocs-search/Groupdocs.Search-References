---
title: "NetworkFoundDocument"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Stellt ein gefundenes Dokument im Suchnetzwerk dar."
type: docs
weight: 11
url: /de/java/com.groupdocs.search.scaling.results/networkfounddocument/
---
**Inheritance:**
java.lang.Object
```
public abstract class NetworkFoundDocument
```

Stellt ein gefundenes Dokument im Suchnetzwerk dar.

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [NetworkFoundDocument()](#NetworkFoundDocument--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getFoundDocument()](#getFoundDocument--) | Liefert das gefundene Dokument. |
|
|  | [getShardIndex()](#getShardIndex--) | Ermittelt den Shard-Index. |
|
### NetworkFoundDocument() {#NetworkFoundDocument--}
```
public NetworkFoundDocument()
```


### getFoundDocument() {#getFoundDocument--}
```
public abstract FoundDocument getFoundDocument()
```


Liefert das gefundene Dokument.


**Returns:**
[FoundDocument](../../com.groupdocs.search.results/founddocument) - The found document.

### getShardIndex() {#getShardIndex--}
```
public abstract int getShardIndex()
```


Ermittelt den Shard-Index.


**Returns:**
int - Der Shard-Index.

