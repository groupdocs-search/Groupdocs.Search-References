---
title: "NetworkImageSearchResult"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Representa un resultado de búsqueda de imágenes que coincide con una imagen de búsqueda."
type: docs
weight: 12
url: /es/java/com.groupdocs.search.scaling.results/networkimagesearchresult/
---
**Inheritance:**
java.lang.Object
```
public abstract class NetworkImageSearchResult
```

Representa un resultado de búsqueda de imágenes que coincide con una imagen de búsqueda.

## Constructores

| Constructor | Descripción |
| --- | --- |
| [NetworkImageSearchResult()](#NetworkImageSearchResult--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getImageCount()](#getImageCount--) | Obtiene el número de imágenes encontradas. |
|
|  | [getFoundImage(int index)](#getFoundImage-int-) | Obtiene la imagen encontrada por índice. |
|
|  | [getNetworkImageSearchToken()](#getNetworkImageSearchToken--) | Obtiene un token de búsqueda de fragmento de imagen para buscar el siguiente fragmento. |
|
|  | [getNodeIndex()](#getNodeIndex--) | Obtiene el índice del nodo del que se recibió el resultado. |
|
|  | [getShardIndex()](#getShardIndex--) | Obtiene el índice del shard del que se recibió el resultado. |
|
### NetworkImageSearchResult() {#NetworkImageSearchResult--}
```
public NetworkImageSearchResult()
```


### getImageCount() {#getImageCount--}
```
public abstract int getImageCount()
```


Obtiene el número de imágenes encontradas.


**Returns:**
int - El número de imágenes encontradas.

### getFoundImage(int index) {#getFoundImage-int-}
```
public abstract FoundImageFrame getFoundImage(int index)
```


Obtiene la imagen encontrada por índice.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | índice | int | El índice de una imagen encontrada. |
|

**Returns:**
[FoundImageFrame](../../com.groupdocs.search.results/foundimageframe) - The found image.

### getNetworkImageSearchToken() {#getNetworkImageSearchToken--}
```
public abstract NetworkImageSearchToken getNetworkImageSearchToken()
```


Obtiene un token de búsqueda de fragmento de imagen para buscar el siguiente fragmento.


**Returns:**
[NetworkImageSearchToken](../../com.groupdocs.search.scaling.results/networkimagesearchtoken) - A chunk image search token for searching the next chunk.

### getNodeIndex() {#getNodeIndex--}
```
public abstract int getNodeIndex()
```


Obtiene el índice del nodo del que se recibió el resultado.


**Returns:**
int - El índice del nodo del que se recibió el resultado.

### getShardIndex() {#getShardIndex--}
```
public abstract int getShardIndex()
```


Obtiene el índice del shard del que se recibió el resultado.


**Returns:**
int - El índice del shard del que se recibió el resultado.

