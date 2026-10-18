---
title: "SearchImage"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Representa una imagen para buscar."
type: docs
weight: 29
url: /es/java/com.groupdocs.search.common/searchimage/
---
**Inheritance:**
java.lang.Object
```
public abstract class SearchImage
```

Representa una imagen para buscar.

## Constructores

| Constructor | Descripción |
| --- | --- |
| [SearchImage()](#SearchImage--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
|  | [create(String filePath)](#create-java.lang.String-) | Crea una imagen a partir de un archivo para buscar. |
|
|  | [create(String filePath, int imageIndex)](#create-java.lang.String-int-) | Crea una imagen a partir de un archivo para buscar. |
|
|  | [create(InputStream stream)](#create-java.io.InputStream-) | Crea una imagen a partir de un flujo para buscar. |
|
|  | [create(InputStream stream, int imageIndex)](#create-java.io.InputStream-int-) | Crea una imagen a partir de un flujo para buscar. |
|
### SearchImage() {#SearchImage--}
```
public SearchImage()
```


### create(String filePath) {#create-java.lang.String-}
```
public static SearchImage create(String filePath)
```


Crea una imagen a partir de un archivo para buscar.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | filePath | java.lang.String | La ruta del archivo de imagen. |
|

**Returns:**
[SearchImage](../../com.groupdocs.search.common/searchimage) - An image to search.

### create(String filePath, int imageIndex) {#create-java.lang.String-int-}
```
public static SearchImage create(String filePath, int imageIndex)
```


Crea una imagen a partir de un archivo para buscar.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | filePath | java.lang.String | La ruta del archivo de imagen. |
|
|  | imageIndex | int | El índice de la imagen en imágenes multipágina. |
|

**Returns:**
[SearchImage](../../com.groupdocs.search.common/searchimage) - An image to search.

### create(InputStream stream) {#create-java.io.InputStream-}
```
public static SearchImage create(InputStream stream)
```


Crea una imagen a partir de un flujo para buscar.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | stream | java.io.InputStream | El flujo de la imagen. |
|

**Returns:**
[SearchImage](../../com.groupdocs.search.common/searchimage) - An image to search.

### create(InputStream stream, int imageIndex) {#create-java.io.InputStream-int-}
```
public static SearchImage create(InputStream stream, int imageIndex)
```


Crea una imagen a partir de un flujo para buscar.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | stream | java.io.InputStream | El flujo de la imagen. |
|
|  | imageIndex | int | El índice de la imagen en imágenes multipágina. |
|

**Returns:**
[SearchImage](../../com.groupdocs.search.common/searchimage) - An image to search.

