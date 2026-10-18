---
title: "NetworkImageSearchResult"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Stelt een afbeeldingzoekresultaat voor dat overeenkomt met een zoekafbeelding."
type: docs
weight: 12
url: /nl/java/com.groupdocs.search.scaling.results/networkimagesearchresult/
---
**Inheritance:**
java.lang.Object
```
public abstract class NetworkImageSearchResult
```

Stelt een afbeeldingzoekresultaat voor dat overeenkomt met een zoekafbeelding.

## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [NetworkImageSearchResult()](#NetworkImageSearchResult--) |  |
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getImageCount()](#getImageCount--) | Haalt het aantal gevonden afbeeldingen op. |
|
|  | [getFoundImage(int index)](#getFoundImage-int-) | Haalt de gevonden afbeelding op via index. |
|
|  | [getNetworkImageSearchToken()](#getNetworkImageSearchToken--) | Haalt een chunk-afbeeldingszoektoken op voor het zoeken naar de volgende chunk. |
|
|  | [getNodeIndex()](#getNodeIndex--) | Haalt de index van de node op waarvan het resultaat werd ontvangen. |
|
|  | [getShardIndex()](#getShardIndex--) | Haalt de index van de shard op waarvan het resultaat werd ontvangen. |
|
### NetworkImageSearchResult() {#NetworkImageSearchResult--}
```
public NetworkImageSearchResult()
```


### getImageCount() {#getImageCount--}
```
public abstract int getImageCount()
```


Haalt het aantal gevonden afbeeldingen op.


**Returns:**
int - Het aantal gevonden afbeeldingen.

### getFoundImage(int index) {#getFoundImage-int-}
```
public abstract FoundImageFrame getFoundImage(int index)
```


Haalt de gevonden afbeelding op via index.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | index | int | De index van een gevonden afbeelding. |
|

**Returns:**
[FoundImageFrame](../../com.groupdocs.search.results/foundimageframe) - The found image.

### getNetworkImageSearchToken() {#getNetworkImageSearchToken--}
```
public abstract NetworkImageSearchToken getNetworkImageSearchToken()
```


Haalt een chunk-afbeeldingszoektoken op voor het zoeken naar de volgende chunk.


**Returns:**
[NetworkImageSearchToken](../../com.groupdocs.search.scaling.results/networkimagesearchtoken) - A chunk image search token for searching the next chunk.

### getNodeIndex() {#getNodeIndex--}
```
public abstract int getNodeIndex()
```


Haalt de index van de node op waarvan het resultaat werd ontvangen.


**Returns:**
int - De index van de node waarvan het resultaat werd ontvangen.

### getShardIndex() {#getShardIndex--}
```
public abstract int getShardIndex()
```


Haalt de index van de shard op waarvan het resultaat werd ontvangen.


**Returns:**
int - De index van de shard waarvan het resultaat werd ontvangen.

