---
title: "NetworkSearchResult"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Representa un resultado de búsqueda que coincide con una consulta de búsqueda."
type: docs
weight: 14
url: /es/java/com.groupdocs.search.scaling.results/networksearchresult/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public abstract class NetworkSearchResult implements Iterable<NetworkFoundDocument>
```

Representa un resultado de búsqueda que coincide con una consulta de búsqueda.

## Constructores

| Constructor | Descripción |
| --- | --- |
| [NetworkSearchResult()](#NetworkSearchResult--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getDocumentCount()](#getDocumentCount--) | Obtiene el número de documentos encontrados. |
|
|  | [getOccurrenceCount()](#getOccurrenceCount--) | Obtiene el número total de ocurrencias encontradas. |
|
|  | [getTruncated()](#getTruncated--) | Obtiene un valor que indica que el resultado está truncado. |
|
|  | [getWarnings()](#getWarnings--) | Obtiene una advertencia que describe el resultado. |
|
|  | [getStartTime()](#getStartTime--) | Obtiene la hora de inicio de la búsqueda. |
|
|  | [getEndTime()](#getEndTime--) | Obtiene la hora de finalización de la búsqueda. |
|
|  | [getSearchDuration()](#getSearchDuration--) | Obtiene la duración de la búsqueda en segundos. |
|
|  | [getFoundDocument(int index)](#getFoundDocument-int-) | Obtiene el documento encontrado por índice. |
|
|  | [iterator()](#iterator--) | Devuelve un iterador que recorre la colección de los documentos encontrados. |
|
|  | [getNextChunkSearchToken()](#getNextChunkSearchToken--) | Obtiene un token de búsqueda de fragmento para buscar el siguiente fragmento. |
|
|  | [getNodeIndex()](#getNodeIndex--) | Obtiene el índice del nodo del que se recibió el resultado. |
|
### NetworkSearchResult() {#NetworkSearchResult--}
```
public NetworkSearchResult()
```


### getDocumentCount() {#getDocumentCount--}
```
public abstract int getDocumentCount()
```


Obtiene el número de documentos encontrados.


**Returns:**
int - El número de documentos encontrados.

### getOccurrenceCount() {#getOccurrenceCount--}
```
public abstract int getOccurrenceCount()
```


Obtiene el número total de ocurrencias encontradas.


**Returns:**
int - El número total de ocurrencias encontradas.

### getTruncated() {#getTruncated--}
```
public abstract boolean getTruncated()
```


Obtiene un valor que indica que el resultado está truncado.


**Returns:**
boolean - Un valor que indica que el resultado está truncado.

### getWarnings() {#getWarnings--}
```
public abstract String getWarnings()
```


Obtiene una advertencia que describe el resultado.


**Returns:**
java.lang.String - Una advertencia que describe el resultado.

### getStartTime() {#getStartTime--}
```
public abstract Date getStartTime()
```


Obtiene la hora de inicio de la búsqueda.


**Returns:**
java.util.Date - La hora de inicio de la búsqueda.

### getEndTime() {#getEndTime--}
```
public abstract Date getEndTime()
```


Obtiene la hora de finalización de la búsqueda.


**Returns:**
java.util.Date - La hora de finalización de la búsqueda.

### getSearchDuration() {#getSearchDuration--}
```
public abstract double getSearchDuration()
```


Obtiene la duración de la búsqueda en segundos.


**Returns:**
double - La duración de la búsqueda en segundos.

### getFoundDocument(int index) {#getFoundDocument-int-}
```
public abstract NetworkFoundDocument getFoundDocument(int index)
```


Obtiene el documento encontrado por índice.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | índice | int | El índice de un documento encontrado. |
|

**Returns:**
[NetworkFoundDocument](../../com.groupdocs.search.scaling.results/networkfounddocument) - The found document.

### iterator() {#iterator--}
```
public abstract Iterator<NetworkFoundDocument> iterator()
```


Devuelve un iterador que recorre la colección de los documentos encontrados.


**Returns:**
java.util.Iterator<com.groupdocs.search.scaling.results.NetworkFoundDocument> - Un iterador que puede usarse para recorrer la colección de los documentos encontrados.

### getNextChunkSearchToken() {#getNextChunkSearchToken--}
```
public abstract NetworkSearchToken getNextChunkSearchToken()
```


Obtiene un token de búsqueda de fragmento para buscar el siguiente fragmento.


**Returns:**
[NetworkSearchToken](../../com.groupdocs.search.scaling.results/networksearchtoken) - A chunk search token for searching the next chunk.

### getNodeIndex() {#getNodeIndex--}
```
public abstract int getNodeIndex()
```


Obtiene el índice del nodo del que se recibió el resultado.


**Returns:**
int - El índice del nodo del que se recibió el resultado.

