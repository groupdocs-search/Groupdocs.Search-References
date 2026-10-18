---
title: "Documento"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Representa la clase base para los documentos añadidos a un índice desde una secuencia del sistema de archivos o una estructura."
type: docs
weight: 13
url: /es/java/com.groupdocs.search/document/
---
**Inheritance:**
java.lang.Object
```
public abstract class Document
```

Representa la clase base para los documentos añadidos a un índice desde el sistema de archivos, una secuencia o una estructura. Contiene métodos estáticos para crear documentos a partir de diferentes tipos de fuentes.


**Learn more**

* [Indexing from different sources](../https://docs.groupdocs.com/search/java/indexing-from-different-sources/)

## Métodos

| Método | Descripción |
| --- | --- |
|  | [getDocumentSourceKind()](#getDocumentSourceKind--) | Obtiene el tipo de origen del documento. |
|
|  | [getDocumentKey()](#getDocumentKey--) | Obtiene la clave del documento que se utiliza para identificar el documento dentro de un índice. |
|
|  | [isLazy()](#isLazy--) | Obtiene un valor que indica si el documento se carga bajo demanda o no. |
|
|  | [getModificationDate()](#getModificationDate--) | Obtiene la fecha de última modificación del documento. |
|
|  | [getExtension()](#getExtension--) | Obtiene la extensión utilizada para este tipo de documento. |
|
|  | [getAdditionalFields()](#getAdditionalFields--) | Obtiene los campos adicionales del documento. |
|
|  | [setAdditionalFields(DocumentField[] value)](#setAdditionalFields-com.groupdocs.search.common.DocumentField---) | Establece los campos adicionales del documento. |
|
|  | [getAttributes()](#getAttributes--) | Obtiene los atributos del documento. |
|
|  | [setAttributes(String[] value)](#setAttributes-java.lang.String---) | Establece los atributos del documento. |
|
|  | [createFromFile(String filePath)](#createFromFile-java.lang.String-) | Crea un documento a partir de un archivo. |
|
|  | [createFromStream(String documentKey, Date modificationDate, String extension, InputStream stream)](#createFromStream-java.lang.String-java.util.Date-java.lang.String-java.io.InputStream-) | Crea un documento a partir de una secuencia. |
|
|  | [createFromStructure(String documentKey, Date modificationDate, DocumentField[] fields)](#createFromStructure-java.lang.String-java.util.Date-com.groupdocs.search.common.DocumentField---) | Crea un documento a partir de una estructura que es una matriz de campos de texto. |
|
|  | [createLazy(DocumentSourceKind documentSourceKind, String documentKey, IDocumentLoader documentLoader)](#createLazy-com.groupdocs.search.common.DocumentSourceKind-java.lang.String-com.groupdocs.search.common.IDocumentLoader-) | Crea un documento cargado de forma diferida. |
|
|  | [toString()](#toString--) | Devuelve un  java.lang.String  que representa el  Document  actual. |
|
### getDocumentSourceKind() {#getDocumentSourceKind--}
```
public abstract DocumentSourceKind getDocumentSourceKind()
```


Obtiene el tipo de origen del documento.


**Returns:**
[DocumentSourceKind](../../com.groupdocs.search.common/documentsourcekind) - The document source kind.

### getDocumentKey() {#getDocumentKey--}
```
public abstract String getDocumentKey()
```


Obtiene la clave del documento que se utiliza para identificar el documento dentro de un índice.


**Returns:**
java.lang.String - La clave del documento que se utiliza para identificar el documento dentro de un índice.

### isLazy() {#isLazy--}
```
public abstract boolean isLazy()
```


Obtiene un valor que indica si el documento se carga bajo demanda o no.


**Returns:**
boolean - Un valor que indica si el documento se carga bajo demanda o no.

### getModificationDate() {#getModificationDate--}
```
public abstract Date getModificationDate()
```


Obtiene la fecha de última modificación del documento.


**Returns:**
java.util.Date - La fecha de última modificación del documento.

### getExtension() {#getExtension--}
```
public abstract String getExtension()
```


Obtiene la extensión utilizada para este tipo de documento.


**Returns:**
java.lang.String - La extensión utilizada para este tipo de documento.

### getAdditionalFields() {#getAdditionalFields--}
```
public DocumentField[] getAdditionalFields()
```


Obtiene los campos adicionales del documento.


**Returns:**
com.groupdocs.search.common.DocumentField[] - Los campos adicionales del documento.

### setAdditionalFields(DocumentField[] value) {#setAdditionalFields-com.groupdocs.search.common.DocumentField---}
```
public void setAdditionalFields(DocumentField[] value)
```


Establece los campos adicionales del documento.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | value | [DocumentField\[\]](../../com.groupdocs.search.common/documentfield) | Los campos adicionales para el documento. |
|

### getAttributes() {#getAttributes--}
```
public String[] getAttributes()
```


Obtiene los atributos del documento.


**Returns:**
java.lang.String[] - Los atributos del documento.

### setAttributes(String[] value) {#setAttributes-java.lang.String---}
```
public void setAttributes(String[] value)
```


Establece los atributos del documento.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | java.lang.String[] | Los atributos del documento. |
|

### createFromFile(String filePath) {#createFromFile-java.lang.String-}
```
public static Document createFromFile(String filePath)
```


Crea un documento a partir de un archivo.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | filePath | java.lang.String | La ruta del archivo del documento. |
|

**Returns:**
[Document](../../com.groupdocs.search/document) - The created document.

### createFromStream(String documentKey, Date modificationDate, String extension, InputStream stream) {#createFromStream-java.lang.String-java.util.Date-java.lang.String-java.io.InputStream-}
```
public static Document createFromStream(String documentKey, Date modificationDate, String extension, InputStream stream)
```


Crea un documento a partir de una secuencia.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | documentKey | java.lang.String | La clave del documento. |
|
|  | modificationDate | java.util.Date | La fecha de modificación del documento. |
|
|  | extension | java.lang.String | La extensión del documento. |
|
|  | stream | java.io.InputStream | El flujo del documento. |
|

**Returns:**
[Document](../../com.groupdocs.search/document) - The created document.

### createFromStructure(String documentKey, Date modificationDate, DocumentField[] fields) {#createFromStructure-java.lang.String-java.util.Date-com.groupdocs.search.common.DocumentField---}
```
public static Document createFromStructure(String documentKey, Date modificationDate, DocumentField[] fields)
```


Crea un documento a partir de una estructura que es una matriz de campos de texto.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | documentKey | java.lang.String | La clave del documento. |
|
|  | modificationDate | java.util.Date | La fecha de modificación del documento. |
|
|  | fields | [DocumentField\[\]](../../com.groupdocs.search.common/documentfield) | Los campos del documento. |
|

**Returns:**
[Document](../../com.groupdocs.search/document) - The created document.

### createLazy(DocumentSourceKind documentSourceKind, String documentKey, IDocumentLoader documentLoader) {#createLazy-com.groupdocs.search.common.DocumentSourceKind-java.lang.String-com.groupdocs.search.common.IDocumentLoader-}
```
public static Document createLazy(DocumentSourceKind documentSourceKind, String documentKey, IDocumentLoader documentLoader)
```


Crea un documento cargado de forma diferida.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | documentSourceKind | [DocumentSourceKind](../../com.groupdocs.search.common/documentsourcekind) | El tipo de origen del documento. Este valor debe coincidir con el tipo del documento cargado. |
|
|  | documentKey | java.lang.String | La clave del documento. Este valor debe coincidir con la clave del documento cargado. |
|
|  | documentLoader | [IDocumentLoader](../../com.groupdocs.search.common/idocumentloader) | El cargador del documento. |
|

**Returns:**
[Document](../../com.groupdocs.search/document) - The created document.

### toString() {#toString--}
```
public String toString()
```


Devuelve un  java.lang.String  que representa el  Document  actual.


**Returns:**
java.lang.String - Una  java.lang.String  que representa el actual  Documento .

