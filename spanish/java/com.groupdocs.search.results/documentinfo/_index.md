---
title: "DocumentInfo"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Representa un descriptor para un documento indexado."
type: docs
weight: 11
url: /es/java/com.groupdocs.search.results/documentinfo/
---
**Inheritance:**
java.lang.Object
```
public abstract class DocumentInfo
```

Representa un descriptor para un documento indexado.


**Learn more**

* [Search results](../https://docs.groupdocs.com/display/searchjava/Search+results)
* [Getting indexed documents](../https://docs.groupdocs.com/display/searchjava/Getting+indexed+documents)

## Constructores

| Constructor | Descripción |
| --- | --- |
| [DocumentInfo()](#DocumentInfo--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
|  | [toString()](#toString--) | Devuelve una  System.String  que representa el actual  DocumentInfo . |
|
|  | [getFilePath()](#getFilePath--) | Obtiene la ruta del archivo indexado desde archivo o la clave del documento indexado desde flujo o estructura. |
|
|  | [getFileType()](#getFileType--) | Obtiene el tipo de archivo. |
|
|  | [getFormatFamily()](#getFormatFamily--) | Obtiene la familia de formatos del documento. |
|
|  | [getInnerPath()](#getInnerPath--) | Obtiene la ruta interna para el elemento del documento contenedor. |
|
|  | [getInnerPathParts()](#getInnerPathParts--) | Obtiene las partes de la ruta interna para el elemento del documento contenedor. |
|
|  | [getDocumentSourceKind()](#getDocumentSourceKind--) | Obtiene el tipo de origen del documento. |
|
|  | [getIndexedWithError()](#getIndexedWithError--) | Obtiene el indicador de error de indexación. |
|
|  | [serialize()](#serialize--) | Serializa la instancia actual a una matriz de bytes. |
|
|  | [deserialize(byte[] array)](#deserialize-byte---) | Deserializa una instancia a partir de una matriz de bytes. |
|
### DocumentInfo() {#DocumentInfo--}
```
public DocumentInfo()
```


### toString() {#toString--}
```
public abstract String toString()
```


Devuelve una  System.String  que representa el actual  DocumentInfo .


**Returns:**
java.lang.String - Una  System.String  que representa el actual  DocumentInfo .

### getFilePath() {#getFilePath--}
```
public abstract String getFilePath()
```


Obtiene la ruta del archivo indexado desde archivo o la clave del documento indexado desde flujo o estructura.


**Returns:**
java.lang.String - La ruta del archivo o la clave del documento.

### getFileType() {#getFileType--}
```
public abstract FileType getFileType()
```


Obtiene el tipo de archivo.


**Returns:**
[FileType](../../com.groupdocs.search.results/filetype) - The file type.

### getFormatFamily() {#getFormatFamily--}
```
public abstract FormatFamily getFormatFamily()
```


Obtiene la familia de formatos del documento.


**Returns:**
[FormatFamily](../../com.groupdocs.search.results/formatfamily) - The document format family.

### getInnerPath() {#getInnerPath--}
```
public abstract String getInnerPath()
```


Obtiene la ruta interna para el elemento del documento contenedor.


**Returns:**
java.lang.String - La ruta interna.

### getInnerPathParts() {#getInnerPathParts--}
```
public abstract String[] getInnerPathParts()
```


Obtiene las partes de la ruta interna para el elemento del documento contenedor.


**Returns:**
java.lang.String[] - Las partes de la ruta interna.

### getDocumentSourceKind() {#getDocumentSourceKind--}
```
public abstract DocumentSourceKind getDocumentSourceKind()
```


Obtiene el tipo de origen del documento.


**Returns:**
[DocumentSourceKind](../../com.groupdocs.search.common/documentsourcekind) - The document source kind.

### getIndexedWithError() {#getIndexedWithError--}
```
public abstract boolean getIndexedWithError()
```


Obtiene el indicador de error de indexación.


**Returns:**
boolean - El indicador de error de indexación.

### serialize() {#serialize--}
```
public abstract byte[] serialize()
```


Serializa la instancia actual a una matriz de bytes.


**Returns:**
byte[] - Una matriz de bytes que representa la instancia actual.

### deserialize(byte[] array) {#deserialize-byte---}
```
public static DocumentInfo deserialize(byte[] array)
```


Deserializa una instancia a partir de una matriz de bytes.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | matriz | byte[] | Una matriz de bytes desde la cual deserializar. |
|

**Returns:**
[DocumentInfo](../../com.groupdocs.search.results/documentinfo) - An instance deserialized from a byte array.

