---
title: "NetworkSearchResult"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Stelt een zoekresultaat voor dat overeenkomt met een zoekopdracht."
type: docs
weight: 14
url: /nl/java/com.groupdocs.search.scaling.results/networksearchresult/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public abstract class NetworkSearchResult implements Iterable<NetworkFoundDocument>
```

Stelt een zoekresultaat voor dat overeenkomt met een zoekopdracht.

## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [NetworkSearchResult()](#NetworkSearchResult--) |  |
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getDocumentCount()](#getDocumentCount--) | Haalt het aantal gevonden documenten op. |
|
|  | [getOccurrenceCount()](#getOccurrenceCount--) | Haalt het totale aantal gevonden voorkomens op. |
|
|  | [getTruncated()](#getTruncated--) | Haalt een waarde op die aangeeft dat het resultaat is afgekapt. |
|
|  | [getWarnings()](#getWarnings--) | Haalt een waarschuwing op die het resultaat beschrijft. |
|
|  | [getStartTime()](#getStartTime--) | Haalt de starttijd van de zoekopdracht op. |
|
|  | [getEndTime()](#getEndTime--) | Haalt de eindtijd van de zoekopdracht op. |
|
|  | [getSearchDuration()](#getSearchDuration--) | Haalt de zoekduur in seconden op. |
|
|  | [getFoundDocument(int index)](#getFoundDocument-int-) | Haalt het gevonden document op via index. |
|
|  | [iterator()](#iterator--) | Retourneert een iterator die door de verzameling van de gevonden documenten iterereert. |
|
|  | [getNextChunkSearchToken()](#getNextChunkSearchToken--) | Haalt een chunk-zoektoken op voor het zoeken naar de volgende chunk. |
|
|  | [getNodeIndex()](#getNodeIndex--) | Haalt de index van de node op waarvan het resultaat werd ontvangen. |
|
### NetworkSearchResult() {#NetworkSearchResult--}
```
public NetworkSearchResult()
```


### getDocumentCount() {#getDocumentCount--}
```
public abstract int getDocumentCount()
```


Haalt het aantal gevonden documenten op.


**Returns:**
int - Het aantal gevonden documenten.

### getOccurrenceCount() {#getOccurrenceCount--}
```
public abstract int getOccurrenceCount()
```


Haalt het totale aantal gevonden voorkomens op.


**Returns:**
int - Het totale aantal gevonden voorkomens.

### getTruncated() {#getTruncated--}
```
public abstract boolean getTruncated()
```


Haalt een waarde op die aangeeft dat het resultaat is afgekapt.


**Returns:**
boolean - Een waarde die aangeeft dat het resultaat is afgekapt.

### getWarnings() {#getWarnings--}
```
public abstract String getWarnings()
```


Haalt een waarschuwing op die het resultaat beschrijft.


**Returns:**
java.lang.String - Een waarschuwing die het resultaat beschrijft.

### getStartTime() {#getStartTime--}
```
public abstract Date getStartTime()
```


Haalt de starttijd van de zoekopdracht op.


**Returns:**
java.util.Date - De starttijd van de zoekopdracht.

### getEndTime() {#getEndTime--}
```
public abstract Date getEndTime()
```


Haalt de eindtijd van de zoekopdracht op.


**Returns:**
java.util.Date - De eindtijd van de zoekopdracht.

### getSearchDuration() {#getSearchDuration--}
```
public abstract double getSearchDuration()
```


Haalt de zoekduur in seconden op.


**Returns:**
double - De zoekduur in seconden.

### getFoundDocument(int index) {#getFoundDocument-int-}
```
public abstract NetworkFoundDocument getFoundDocument(int index)
```


Haalt het gevonden document op via index.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | index | int | De index van een gevonden document. |
|

**Returns:**
[NetworkFoundDocument](../../com.groupdocs.search.scaling.results/networkfounddocument) - The found document.

### iterator() {#iterator--}
```
public abstract Iterator<NetworkFoundDocument> iterator()
```


Retourneert een iterator die door de verzameling van de gevonden documenten iterereert.


**Returns:**
java.util.Iterator<com.groupdocs.search.scaling.results.NetworkFoundDocument> - Een iterator die kan worden gebruikt om door de verzameling van de gevonden documenten te itereren.

### getNextChunkSearchToken() {#getNextChunkSearchToken--}
```
public abstract NetworkSearchToken getNextChunkSearchToken()
```


Haalt een chunk-zoektoken op voor het zoeken naar de volgende chunk.


**Returns:**
[NetworkSearchToken](../../com.groupdocs.search.scaling.results/networksearchtoken) - A chunk search token for searching the next chunk.

### getNodeIndex() {#getNodeIndex--}
```
public abstract int getNodeIndex()
```


Haalt de index van de node op waarvan het resultaat werd ontvangen.


**Returns:**
int - De index van de node waarvan het resultaat werd ontvangen.

