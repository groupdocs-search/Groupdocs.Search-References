---
title: "NetworkImageSearchResult"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Stellt ein Bildsuchergebnis dar, das zu einem Suchbild passt."
type: docs
weight: 12
url: /de/java/com.groupdocs.search.scaling.results/networkimagesearchresult/
---
**Inheritance:**
java.lang.Object
```
public abstract class NetworkImageSearchResult
```

Stellt ein Bildsuchergebnis dar, das zu einem Suchbild passt.

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [NetworkImageSearchResult()](#NetworkImageSearchResult--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getImageCount()](#getImageCount--) | Gibt die Anzahl gefundener Bilder zurück. |
|
|  | [getFoundImage(int index)](#getFoundImage-int-) | Gibt das gefundene Bild nach Index zurück. |
|
|  | [getNetworkImageSearchToken()](#getNetworkImageSearchToken--) | Gibt ein Chunk-Bild-Such-Token für die Suche nach dem nächsten Chunk zurück. |
|
|  | [getNodeIndex()](#getNodeIndex--) | Gibt den Index des Knotens zurück, von dem das Ergebnis empfangen wurde. |
|
|  | [getShardIndex()](#getShardIndex--) | Gibt den Index des Shards zurück, von dem das Ergebnis empfangen wurde. |
|
### NetworkImageSearchResult() {#NetworkImageSearchResult--}
```
public NetworkImageSearchResult()
```


### getImageCount() {#getImageCount--}
```
public abstract int getImageCount()
```


Gibt die Anzahl gefundener Bilder zurück.


**Returns:**
int - Die Anzahl gefundener Bilder.

### getFoundImage(int index) {#getFoundImage-int-}
```
public abstract FoundImageFrame getFoundImage(int index)
```


Gibt das gefundene Bild nach Index zurück.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Index | int | Der Index eines gefundenen Bildes. |
|

**Returns:**
[FoundImageFrame](../../com.groupdocs.search.results/foundimageframe) - The found image.

### getNetworkImageSearchToken() {#getNetworkImageSearchToken--}
```
public abstract NetworkImageSearchToken getNetworkImageSearchToken()
```


Gibt ein Chunk-Bild-Such-Token für die Suche nach dem nächsten Chunk zurück.


**Returns:**
[NetworkImageSearchToken](../../com.groupdocs.search.scaling.results/networkimagesearchtoken) - A chunk image search token for searching the next chunk.

### getNodeIndex() {#getNodeIndex--}
```
public abstract int getNodeIndex()
```


Gibt den Index des Knotens zurück, von dem das Ergebnis empfangen wurde.


**Returns:**
int - Der Index des Knotens, von dem das Ergebnis empfangen wurde.

### getShardIndex() {#getShardIndex--}
```
public abstract int getShardIndex()
```


Gibt den Index des Shards zurück, von dem das Ergebnis empfangen wurde.


**Returns:**
int - Der Index des Shards, von dem das Ergebnis empfangen wurde.

