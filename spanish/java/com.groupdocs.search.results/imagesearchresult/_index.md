---
title: "ImageSearchResult"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Representa el resultado de una búsqueda inversa de imágenes."
type: docs
weight: 17
url: /es/java/com.groupdocs.search.results/imagesearchresult/
---
**Inheritance:**
java.lang.Object
```
public abstract class ImageSearchResult
```

Representa el resultado de una búsqueda inversa de imágenes.

## Constructores

| Constructor | Descripción |
| --- | --- |
| [ImageSearchResult()](#ImageSearchResult--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getImageCount()](#getImageCount--) | Obtiene el número de imágenes encontradas. |
|
|  | [getFoundImage(int index)](#getFoundImage-int-) | Obtiene la imagen encontrada por índice. |
|
### ImageSearchResult() {#ImageSearchResult--}
```
public ImageSearchResult()
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

