---
title: "DocumentImage"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Representa datos de imagen de documento."
type: docs
weight: 16
url: /es/java/com.groupdocs.search.common/documentimage/
---
**Inheritance:**
java.lang.Object
```
public abstract class DocumentImage
```

Representa datos de imagen de documento.

## Constructores

| Constructor | Descripción |
| --- | --- |
| [DocumentImage()](#DocumentImage--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getImageIndex()](#getImageIndex--) | Obtiene el número ordinal de la imagen en el documento. |
|
|  | [getFields()](#getFields--) | Obtiene los campos extraídos. |
|
|  | [getFrames()](#getFrames--) | Obtiene los fotogramas de la imagen. |
|
### DocumentImage() {#DocumentImage--}
```
public DocumentImage()
```


### getImageIndex() {#getImageIndex--}
```
public abstract int getImageIndex()
```


Obtiene el número ordinal de la imagen en el documento.


**Returns:**
int - El número ordinal de la imagen en el documento.

### getFields() {#getFields--}
```
public abstract DocumentField[] getFields()
```


Obtiene los campos extraídos.


**Returns:**
com.groupdocs.search.common.DocumentField[] - Los campos extraídos.

### getFrames() {#getFrames--}
```
public abstract ImageFrame[] getFrames()
```


Obtiene los fotogramas de la imagen.


**Returns:**
com.groupdocs.search.common.ImageFrame[] - Los fotogramas de la imagen.

