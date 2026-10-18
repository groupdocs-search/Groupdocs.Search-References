---
title: "NetworkSearchResult"
second_title: "GroupDocs.Search för Java API-referens"
description: "Representerar ett sökresultat som matchar en sökfråga."
type: docs
weight: 14
url: /sv/java/com.groupdocs.search.scaling.results/networksearchresult/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public abstract class NetworkSearchResult implements Iterable<NetworkFoundDocument>
```

Representerar ett sökresultat som matchar en sökfråga.

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [NetworkSearchResult()](#NetworkSearchResult--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getDocumentCount()](#getDocumentCount--) | Hämtar antalet hittade dokument. |
|
|  | [getOccurrenceCount()](#getOccurrenceCount--) | Hämtar det totala antalet hittade förekomster. |
|
|  | [getTruncated()](#getTruncated--) | Hämtar ett värde som indikerar att resultatet är avkortat. |
|
|  | [getWarnings()](#getWarnings--) | Hämtar en varning som beskriver resultatet. |
|
|  | [getStartTime()](#getStartTime--) | Hämtar starttiden för sökningen. |
|
|  | [getEndTime()](#getEndTime--) | Hämtar sluttiden för sökningen. |
|
|  | [getSearchDuration()](#getSearchDuration--) | Hämtar sökvaraktigheten i sekunder. |
|
|  | [getFoundDocument(int index)](#getFoundDocument-int-) | Hämtar det hittade dokumentet efter index. |
|
|  | [iterator()](#iterator--) | Returnerar en iterator som itererar genom samlingen av de hittade dokumenten. |
|
|  | [getNextChunkSearchToken()](#getNextChunkSearchToken--) | Hämtar en token för segment-sökning för att söka nästa segment. |
|
|  | [getNodeIndex()](#getNodeIndex--) | Hämtar indexet för noden som resultatet mottogs från. |
|
### NetworkSearchResult() {#NetworkSearchResult--}
```
public NetworkSearchResult()
```


### getDocumentCount() {#getDocumentCount--}
```
public abstract int getDocumentCount()
```


Hämtar antalet hittade dokument.


**Returns:**
int - Antalet hittade dokument.

### getOccurrenceCount() {#getOccurrenceCount--}
```
public abstract int getOccurrenceCount()
```


Hämtar det totala antalet hittade förekomster.


**Returns:**
int - Det totala antalet hittade förekomster.

### getTruncated() {#getTruncated--}
```
public abstract boolean getTruncated()
```


Hämtar ett värde som indikerar att resultatet är avkortat.


**Returns:**
boolean - Ett värde som indikerar att resultatet är avkortat.

### getWarnings() {#getWarnings--}
```
public abstract String getWarnings()
```


Hämtar en varning som beskriver resultatet.


**Returns:**
java.lang.String - En varning som beskriver resultatet.

### getStartTime() {#getStartTime--}
```
public abstract Date getStartTime()
```


Hämtar starttiden för sökningen.


**Returns:**
java.util.Date - Starttiden för sökningen.

### getEndTime() {#getEndTime--}
```
public abstract Date getEndTime()
```


Hämtar sluttiden för sökningen.


**Returns:**
java.util.Date - Sluttiden för sökningen.

### getSearchDuration() {#getSearchDuration--}
```
public abstract double getSearchDuration()
```


Hämtar sökvaraktigheten i sekunder.


**Returns:**
double - Sökvaraktigheten i sekunder.

### getFoundDocument(int index) {#getFoundDocument-int-}
```
public abstract NetworkFoundDocument getFoundDocument(int index)
```


Hämtar det hittade dokumentet efter index.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | index | int | Indexet för ett hittat dokument. |
|

**Returns:**
[NetworkFoundDocument](../../com.groupdocs.search.scaling.results/networkfounddocument) - The found document.

### iterator() {#iterator--}
```
public abstract Iterator<NetworkFoundDocument> iterator()
```


Returnerar en iterator som itererar genom samlingen av de hittade dokumenten.


**Returns:**
java.util.Iterator<com.groupdocs.search.scaling.results.NetworkFoundDocument> - En iterator som kan användas för att iterera genom samlingen av de hittade dokumenten.

### getNextChunkSearchToken() {#getNextChunkSearchToken--}
```
public abstract NetworkSearchToken getNextChunkSearchToken()
```


Hämtar en token för segment-sökning för att söka nästa segment.


**Returns:**
[NetworkSearchToken](../../com.groupdocs.search.scaling.results/networksearchtoken) - A chunk search token for searching the next chunk.

### getNodeIndex() {#getNodeIndex--}
```
public abstract int getNodeIndex()
```


Hämtar indexet för noden som resultatet mottogs från.


**Returns:**
int - Indexet för noden som resultatet mottogs från.

