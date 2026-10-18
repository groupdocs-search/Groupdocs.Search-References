---
title: "NetworkSearchResult"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Rappresenta un risultato di ricerca corrispondente a una query di ricerca."
type: docs
weight: 14
url: /it/java/com.groupdocs.search.scaling.results/networksearchresult/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public abstract class NetworkSearchResult implements Iterable<NetworkFoundDocument>
```

Rappresenta un risultato di ricerca corrispondente a una query di ricerca.

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [NetworkSearchResult()](#NetworkSearchResult--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getDocumentCount()](#getDocumentCount--) | Ottiene il numero di documenti trovati. |
|
|  | [getOccurrenceCount()](#getOccurrenceCount--) | Ottiene il numero totale di occorrenze trovate. |
|
|  | [getTruncated()](#getTruncated--) | Restituisce un valore che indica che il risultato è troncato. |
|
|  | [getWarnings()](#getWarnings--) | Restituisce avvisi che descrivono il risultato. |
|
|  | [getStartTime()](#getStartTime--) | Ottiene l'ora di inizio della ricerca. |
|
|  | [getEndTime()](#getEndTime--) | Ottiene l'ora di fine della ricerca. |
|
|  | [getSearchDuration()](#getSearchDuration--) | Ottiene la durata della ricerca in secondi. |
|
|  | [getFoundDocument(int index)](#getFoundDocument-int-) | Restituisce il documento trovato per indice. |
|
|  | [iterator()](#iterator--) | Restituisce un iteratore che scorre la collezione dei documenti trovati. |
|
|  | [getNextChunkSearchToken()](#getNextChunkSearchToken--) | Restituisce un token di ricerca a blocchi per cercare il blocco successivo. |
|
|  | [getNodeIndex()](#getNodeIndex--) | Restituisce l'indice del nodo da cui è stato ricevuto il risultato. |
|
### NetworkSearchResult() {#NetworkSearchResult--}
```
public NetworkSearchResult()
```


### getDocumentCount() {#getDocumentCount--}
```
public abstract int getDocumentCount()
```


Ottiene il numero di documenti trovati.


**Returns:**
int - Il numero di documenti trovati.

### getOccurrenceCount() {#getOccurrenceCount--}
```
public abstract int getOccurrenceCount()
```


Ottiene il numero totale di occorrenze trovate.


**Returns:**
int - Il numero totale di occorrenze trovate.

### getTruncated() {#getTruncated--}
```
public abstract boolean getTruncated()
```


Restituisce un valore che indica che il risultato è troncato.


**Returns:**
boolean - Un valore che indica che il risultato è troncato.

### getWarnings() {#getWarnings--}
```
public abstract String getWarnings()
```


Restituisce avvisi che descrivono il risultato.


**Returns:**
java.lang.String - Avvisi che descrivono il risultato.

### getStartTime() {#getStartTime--}
```
public abstract Date getStartTime()
```


Ottiene l'ora di inizio della ricerca.


**Returns:**
java.util.Date - L'ora di inizio della ricerca.

### getEndTime() {#getEndTime--}
```
public abstract Date getEndTime()
```


Ottiene l'ora di fine della ricerca.


**Returns:**
java.util.Date - L'ora di fine della ricerca.

### getSearchDuration() {#getSearchDuration--}
```
public abstract double getSearchDuration()
```


Ottiene la durata della ricerca in secondi.


**Returns:**
double - La durata della ricerca in secondi.

### getFoundDocument(int index) {#getFoundDocument-int-}
```
public abstract NetworkFoundDocument getFoundDocument(int index)
```


Restituisce il documento trovato per indice.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | indice | int | L'indice di un documento trovato. |
|

**Returns:**
[NetworkFoundDocument](../../com.groupdocs.search.scaling.results/networkfounddocument) - The found document.

### iterator() {#iterator--}
```
public abstract Iterator<NetworkFoundDocument> iterator()
```


Restituisce un iteratore che scorre la collezione dei documenti trovati.


**Returns:**
java.util.Iterator<com.groupdocs.search.scaling.results.NetworkFoundDocument> - Un iteratore che può essere usato per scorrere la collezione dei documenti trovati.

### getNextChunkSearchToken() {#getNextChunkSearchToken--}
```
public abstract NetworkSearchToken getNextChunkSearchToken()
```


Restituisce un token di ricerca a blocchi per cercare il blocco successivo.


**Returns:**
[NetworkSearchToken](../../com.groupdocs.search.scaling.results/networksearchtoken) - A chunk search token for searching the next chunk.

### getNodeIndex() {#getNodeIndex--}
```
public abstract int getNodeIndex()
```


Restituisce l'indice del nodo da cui è stato ricevuto il risultato.


**Returns:**
int - L'indice del nodo da cui è stato ricevuto il risultato.

