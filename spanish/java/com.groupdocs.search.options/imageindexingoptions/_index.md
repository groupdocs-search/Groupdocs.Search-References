---
title: "ImageIndexingOptions"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Proporciona opciones de indexación de imágenes para la búsqueda inversa de imágenes."
type: docs
weight: 23
url: /es/java/com.groupdocs.search.options/imageindexingoptions/
---
**Inheritance:**
java.lang.Object
```
public abstract class ImageIndexingOptions
```

Proporciona opciones de indexación de imágenes para la búsqueda inversa de imágenes.

## Constructores

| Constructor | Descripción |
| --- | --- |
| [ImageIndexingOptions()](#ImageIndexingOptions--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getEnabledForSeparateImages()](#getEnabledForSeparateImages--) | Obtiene un valor que indica si indexar archivos de imagen separados. |
|
|  | [setEnabledForSeparateImages(boolean value)](#setEnabledForSeparateImages-boolean-) | Establece un valor que indica si indexar archivos de imagen separados. |
|
|  | [getEnabledForContainerItemImages()](#getEnabledForContainerItemImages--) | Obtiene un valor que indica si indexar imágenes que son elementos en un contenedor (por ejemplo, imágenes en un archivo ZIP). |
|
|  | [setEnabledForContainerItemImages(boolean value)](#setEnabledForContainerItemImages-boolean-) | Establece un valor que indica si indexar imágenes que son elementos en un contenedor (por ejemplo, imágenes en un archivo ZIP). |
|
|  | [getEnabledForEmbeddedImages()](#getEnabledForEmbeddedImages--) | Obtiene un valor que indica si indexar imágenes incrustadas (por ejemplo, imágenes en un documento DOCX). |
|
|  | [setEnabledForEmbeddedImages(boolean value)](#setEnabledForEmbeddedImages-boolean-) | Establece un valor que indica si indexar imágenes incrustadas (por ejemplo, imágenes en un documento DOCX). |
|
### ImageIndexingOptions() {#ImageIndexingOptions--}
```
public ImageIndexingOptions()
```


### getEnabledForSeparateImages() {#getEnabledForSeparateImages--}
```
public abstract boolean getEnabledForSeparateImages()
```


Obtiene un valor que indica si indexar archivos de imagen separados. El valor predeterminado es  false .


**Returns:**
boolean - Un valor que indica si indexar archivos de imagen separados.

### setEnabledForSeparateImages(boolean value) {#setEnabledForSeparateImages-boolean-}
```
public abstract void setEnabledForSeparateImages(boolean value)
```


Establece un valor que indica si indexar archivos de imagen separados. El valor predeterminado es  false .


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | boolean | Un valor que indica si indexar archivos de imagen separados. |
|

### getEnabledForContainerItemImages() {#getEnabledForContainerItemImages--}
```
public abstract boolean getEnabledForContainerItemImages()
```


Obtiene un valor que indica si indexar imágenes que son elementos en un contenedor (por ejemplo, imágenes en un archivo ZIP). El valor predeterminado es  false .


**Returns:**
boolean - Un valor que indica si se deben indexar imágenes que son elementos en un contenedor.

### setEnabledForContainerItemImages(boolean value) {#setEnabledForContainerItemImages-boolean-}
```
public abstract void setEnabledForContainerItemImages(boolean value)
```


Establece un valor que indica si se deben indexar imágenes que son elementos en un contenedor (por ejemplo, imágenes en un archivo ZIP). El valor predeterminado es false.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | boolean | Un valor que indica si se deben indexar imágenes que son elementos en un contenedor. |
|

### getEnabledForEmbeddedImages() {#getEnabledForEmbeddedImages--}
```
public abstract boolean getEnabledForEmbeddedImages()
```


Obtiene un valor que indica si se deben indexar imágenes incrustadas (por ejemplo, imágenes en un documento DOCX). El valor predeterminado es false.


**Returns:**
boolean - Un valor que indica si se deben indexar imágenes incrustadas.

### setEnabledForEmbeddedImages(boolean value) {#setEnabledForEmbeddedImages-boolean-}
```
public abstract void setEnabledForEmbeddedImages(boolean value)
```


Establece un valor que indica si se deben indexar imágenes incrustadas (por ejemplo, imágenes en un documento DOCX). El valor predeterminado es false.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | boolean | Un valor que indica si se deben indexar imágenes incrustadas. |
|

