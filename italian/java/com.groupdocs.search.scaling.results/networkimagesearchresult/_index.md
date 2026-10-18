---
title: "NetworkImageSearchResult"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Rappresenta un risultato di ricerca immagine corrispondente a un'immagine di ricerca."
type: docs
weight: 12
url: /it/java/com.groupdocs.search.scaling.results/networkimagesearchresult/
---
**Inheritance:**
java.lang.Object
```
public abstract class NetworkImageSearchResult
```

Rappresenta un risultato di ricerca immagine corrispondente a un'immagine di ricerca.

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [NetworkImageSearchResult()](#NetworkImageSearchResult--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getImageCount()](#getImageCount--) | Restituisce il numero di immagini trovate. |
|
|  | [getFoundImage(int index)](#getFoundImage-int-) | Restituisce l'immagine trovata per indice. |
|
|  | [getNetworkImageSearchToken()](#getNetworkImageSearchToken--) | Restituisce un token di ricerca immagine a blocchi per cercare il blocco successivo. |
|
|  | [getNodeIndex()](#getNodeIndex--) | Restituisce l'indice del nodo da cui è stato ricevuto il risultato. |
|
|  | [getShardIndex()](#getShardIndex--) | Restituisce l'indice dello shard da cui è stato ricevuto il risultato. |
|
### NetworkImageSearchResult() {#NetworkImageSearchResult--}
```
public NetworkImageSearchResult()
```


### getImageCount() {#getImageCount--}
```
public abstract int getImageCount()
```


Restituisce il numero di immagini trovate.


**Returns:**
int - Il numero di immagini trovate.

### getFoundImage(int index) {#getFoundImage-int-}
```
public abstract FoundImageFrame getFoundImage(int index)
```


Restituisce l'immagine trovata per indice.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | indice | int | L'indice di un'immagine trovata. |
|

**Returns:**
[FoundImageFrame](../../com.groupdocs.search.results/foundimageframe) - The found image.

### getNetworkImageSearchToken() {#getNetworkImageSearchToken--}
```
public abstract NetworkImageSearchToken getNetworkImageSearchToken()
```


Restituisce un token di ricerca immagine a blocchi per cercare il blocco successivo.


**Returns:**
[NetworkImageSearchToken](../../com.groupdocs.search.scaling.results/networkimagesearchtoken) - A chunk image search token for searching the next chunk.

### getNodeIndex() {#getNodeIndex--}
```
public abstract int getNodeIndex()
```


Restituisce l'indice del nodo da cui è stato ricevuto il risultato.


**Returns:**
int - L'indice del nodo da cui è stato ricevuto il risultato.

### getShardIndex() {#getShardIndex--}
```
public abstract int getShardIndex()
```


Restituisce l'indice dello shard da cui è stato ricevuto il risultato.


**Returns:**
int - L'indice dello shard da cui è stato ricevuto il risultato.

