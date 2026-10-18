---
title: "NetworkImageSearchResult"
second_title: "GroupDocs.Search för Java API-referens"
description: "Representerar ett bildsökresultat som matchar en sökbild."
type: docs
weight: 12
url: /sv/java/com.groupdocs.search.scaling.results/networkimagesearchresult/
---
**Inheritance:**
java.lang.Object
```
public abstract class NetworkImageSearchResult
```

Representerar ett bildsökresultat som matchar en sökbild.

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [NetworkImageSearchResult()](#NetworkImageSearchResult--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getImageCount()](#getImageCount--) | Hämtar antalet hittade bilder. |
|
|  | [getFoundImage(int index)](#getFoundImage-int-) | Hämtar den hittade bilden efter index. |
|
|  | [getNetworkImageSearchToken()](#getNetworkImageSearchToken--) | Hämtar en token för bildsökning i segment för att söka nästa segment. |
|
|  | [getNodeIndex()](#getNodeIndex--) | Hämtar indexet för noden som resultatet mottogs från. |
|
|  | [getShardIndex()](#getShardIndex--) | Hämtar indexet för sharden som resultatet mottogs från. |
|
### NetworkImageSearchResult() {#NetworkImageSearchResult--}
```
public NetworkImageSearchResult()
```


### getImageCount() {#getImageCount--}
```
public abstract int getImageCount()
```


Hämtar antalet hittade bilder.


**Returns:**
int - Antalet hittade bilder.

### getFoundImage(int index) {#getFoundImage-int-}
```
public abstract FoundImageFrame getFoundImage(int index)
```


Hämtar den hittade bilden efter index.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | index | int | Indexet för en hittad bild. |
|

**Returns:**
[FoundImageFrame](../../com.groupdocs.search.results/foundimageframe) - The found image.

### getNetworkImageSearchToken() {#getNetworkImageSearchToken--}
```
public abstract NetworkImageSearchToken getNetworkImageSearchToken()
```


Hämtar en token för bildsökning i segment för att söka nästa segment.


**Returns:**
[NetworkImageSearchToken](../../com.groupdocs.search.scaling.results/networkimagesearchtoken) - A chunk image search token for searching the next chunk.

### getNodeIndex() {#getNodeIndex--}
```
public abstract int getNodeIndex()
```


Hämtar indexet för noden som resultatet mottogs från.


**Returns:**
int - Indexet för noden som resultatet mottogs från.

### getShardIndex() {#getShardIndex--}
```
public abstract int getShardIndex()
```


Hämtar indexet för sharden som resultatet mottogs från.


**Returns:**
int - Indexet för sharden som resultatet mottogs från.

