---
title: "NetworkSearchResult"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Stellt ein Suchergebnis dar, das zu einer Suchanfrage passt."
type: docs
weight: 14
url: /de/java/com.groupdocs.search.scaling.results/networksearchresult/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public abstract class NetworkSearchResult implements Iterable<NetworkFoundDocument>
```

Stellt ein Suchergebnis dar, das zu einer Suchanfrage passt.

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [NetworkSearchResult()](#NetworkSearchResult--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getDocumentCount()](#getDocumentCount--) | Ermittelt die Anzahl gefundener Dokumente. |
|
|  | [getOccurrenceCount()](#getOccurrenceCount--) | Ermittelt die Gesamtzahl gefundener Vorkommen. |
|
|  | [getTruncated()](#getTruncated--) | Gibt einen Wert zurück, der anzeigt, dass das Ergebnis abgeschnitten ist. |
|
|  | [getWarnings()](#getWarnings--) | Gibt eine Warnung zurück, die das Ergebnis beschreibt. |
|
|  | [getStartTime()](#getStartTime--) | Ermittelt die Startzeit der Suche. |
|
|  | [getEndTime()](#getEndTime--) | Ermittelt die Endzeit der Suche. |
|
|  | [getSearchDuration()](#getSearchDuration--) | Ermittelt die Suchdauer in Sekunden. |
|
|  | [getFoundDocument(int index)](#getFoundDocument-int-) | Gibt das gefundene Dokument nach Index zurück. |
|
|  | [iterator()](#iterator--) | Gibt einen Iterator zurück, der durch die Sammlung der gefundenen Dokumente iteriert. |
|
|  | [getNextChunkSearchToken()](#getNextChunkSearchToken--) | Gibt ein Chunk-Such-Token für die Suche nach dem nächsten Chunk zurück. |
|
|  | [getNodeIndex()](#getNodeIndex--) | Gibt den Index des Knotens zurück, von dem das Ergebnis empfangen wurde. |
|
### NetworkSearchResult() {#NetworkSearchResult--}
```
public NetworkSearchResult()
```


### getDocumentCount() {#getDocumentCount--}
```
public abstract int getDocumentCount()
```


Ermittelt die Anzahl gefundener Dokumente.


**Returns:**
int - Die Anzahl gefundener Dokumente.

### getOccurrenceCount() {#getOccurrenceCount--}
```
public abstract int getOccurrenceCount()
```


Ermittelt die Gesamtzahl gefundener Vorkommen.


**Returns:**
int - Die Gesamtzahl gefundener Vorkommen.

### getTruncated() {#getTruncated--}
```
public abstract boolean getTruncated()
```


Gibt einen Wert zurück, der anzeigt, dass das Ergebnis abgeschnitten ist.


**Returns:**
boolean - Ein Wert, der anzeigt, dass das Ergebnis abgeschnitten ist.

### getWarnings() {#getWarnings--}
```
public abstract String getWarnings()
```


Gibt eine Warnung zurück, die das Ergebnis beschreibt.


**Returns:**
java.lang.String - Eine Warnung, die das Ergebnis beschreibt.

### getStartTime() {#getStartTime--}
```
public abstract Date getStartTime()
```


Ermittelt die Startzeit der Suche.


**Returns:**
java.util.Date - Die Startzeit der Suche.

### getEndTime() {#getEndTime--}
```
public abstract Date getEndTime()
```


Ermittelt die Endzeit der Suche.


**Returns:**
java.util.Date - Die Endzeit der Suche.

### getSearchDuration() {#getSearchDuration--}
```
public abstract double getSearchDuration()
```


Ermittelt die Suchdauer in Sekunden.


**Returns:**
double - Die Suchdauer in Sekunden.

### getFoundDocument(int index) {#getFoundDocument-int-}
```
public abstract NetworkFoundDocument getFoundDocument(int index)
```


Gibt das gefundene Dokument nach Index zurück.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Index | int | Der Index eines gefundenen Dokuments. |
|

**Returns:**
[NetworkFoundDocument](../../com.groupdocs.search.scaling.results/networkfounddocument) - The found document.

### iterator() {#iterator--}
```
public abstract Iterator<NetworkFoundDocument> iterator()
```


Gibt einen Iterator zurück, der durch die Sammlung der gefundenen Dokumente iteriert.


**Returns:**
java.util.Iterator<com.groupdocs.search.scaling.results.NetworkFoundDocument> - Ein Iterator, der verwendet werden kann, um durch die Sammlung der gefundenen Dokumente zu iterieren.

### getNextChunkSearchToken() {#getNextChunkSearchToken--}
```
public abstract NetworkSearchToken getNextChunkSearchToken()
```


Gibt ein Chunk-Such-Token für die Suche nach dem nächsten Chunk zurück.


**Returns:**
[NetworkSearchToken](../../com.groupdocs.search.scaling.results/networksearchtoken) - A chunk search token for searching the next chunk.

### getNodeIndex() {#getNodeIndex--}
```
public abstract int getNodeIndex()
```


Gibt den Index des Knotens zurück, von dem das Ergebnis empfangen wurde.


**Returns:**
int - Der Index des Knotens, von dem das Ergebnis empfangen wurde.

