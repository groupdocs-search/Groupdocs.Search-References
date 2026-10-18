---
title: "FoundImageFrame"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Representa un fotograma de imagen encontrado."
type: docs
weight: 16
url: /es/java/com.groupdocs.search.results/foundimageframe/
---
**Inheritance:**
java.lang.Object
```
public abstract class FoundImageFrame
```

Representa un fotograma de imagen encontrado.

## Constructores

| Constructor | Descripción |
| --- | --- |
| [FoundImageFrame()](#FoundImageFrame--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getDocumentInfo()](#getDocumentInfo--) | Obtiene la información del documento. |
|
|  | [getImageIndex()](#getImageIndex--) | Obtiene el número ordinal de la imagen en el documento. |
|
|  | [getFrameIndex()](#getFrameIndex--) | Obtiene el índice del fotograma en la imagen. |
|
|  | [getHashDifferences()](#getHashDifferences--) | Obtiene el número de bits no coincidentes en el hash de la imagen. |
|
|  | [toString()](#toString--) | Devuelve un  System.String  que representa el actual  FoundImageFrame . |
|
### FoundImageFrame() {#FoundImageFrame--}
```
public FoundImageFrame()
```


### getDocumentInfo() {#getDocumentInfo--}
```
public abstract DocumentInfo getDocumentInfo()
```


Obtiene la información del documento.


**Returns:**
[DocumentInfo](../../com.groupdocs.search.results/documentinfo) - The document info.

### getImageIndex() {#getImageIndex--}
```
public abstract int getImageIndex()
```


Obtiene el número ordinal de la imagen en el documento.


**Returns:**
int - El número ordinal de la imagen en el documento.

### getFrameIndex() {#getFrameIndex--}
```
public abstract int getFrameIndex()
```


Obtiene el índice del fotograma en la imagen.


**Returns:**
int - El índice del fotograma en la imagen.

### getHashDifferences() {#getHashDifferences--}
```
public abstract int getHashDifferences()
```


Obtiene el número de bits no coincidentes en el hash de la imagen.


**Returns:**
int - El número de bits no coincidentes en el hash de la imagen.

### toString() {#toString--}
```
public abstract String toString()
```


Devuelve un  System.String  que representa el actual  FoundImageFrame .


**Returns:**
java.lang.String - Un  System.String  que representa el actual  FoundImageFrame .

