---
title: "FileIndexingEventArgs"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Representa los argumentos del evento de inicio del indexado de un documento."
type: docs
weight: 14
url: /es/java/com.groupdocs.search.events/fileindexingeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class FileIndexingEventArgs extends BaseIndexEventArgs
```

Representa los argumentos del evento de inicio del indexado de un documento.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Métodos

| Método | Descripción |
| --- | --- |
|  | [getDocument()](#getDocument--) | Obtiene el documento. |
|
|  | [getDocumentFullPath()](#getDocumentFullPath--) | Obtiene la ruta completa del documento. |
|
|  | [getDocumentKey()](#getDocumentKey--) | Obtiene la clave del documento. |
|
|  | [getSkipIndexing()](#getSkipIndexing--) | Obtiene un valor que indica que la indexación del documento debe omitirse. |
|
|  | [setSkipIndexing(boolean value)](#setSkipIndexing-boolean-) | Establece un valor que indica que la indexación del documento debe omitirse. |
|
|  | [getEncoding()](#getEncoding--) | Obtiene la codificación del documento. |
|
|  | [setEncoding(String value)](#setEncoding-java.lang.String-) | Establece la codificación del documento. |
|
|  | [getCustomExtractor()](#getCustomExtractor--) | Obtiene el extractor de texto personalizado. |
|
|  | [setCustomExtractor(IFieldExtractor value)](#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-) | Establece el extractor de texto personalizado. |
|
|  | [getAdditionalFields()](#getAdditionalFields--) | Obtiene los campos adicionales del documento. |
|
|  | [setAdditionalFields(DocumentField[] value)](#setAdditionalFields-com.groupdocs.search.common.DocumentField---) | Establece los campos adicionales del documento. |
|
|  | [getAttributes()](#getAttributes--) | Obtiene los atributos del documento. |
|
|  | [setAttributes(String[] value)](#setAttributes-java.lang.String---) | Establece los atributos del documento. |
|
### getDocument() {#getDocument--}
```
public final Document getDocument()
```


Obtiene el documento.


**Returns:**
[Document](../../com.groupdocs.search/document) - The document.

### getDocumentFullPath() {#getDocumentFullPath--}
```
public final String getDocumentFullPath()
```


Obtiene la ruta completa del documento.


**Returns:**
java.lang.String - La ruta completa del documento.

### getDocumentKey() {#getDocumentKey--}
```
public final String getDocumentKey()
```


Obtiene la clave del documento.


**Returns:**
java.lang.String - La clave del documento.

### getSkipIndexing() {#getSkipIndexing--}
```
public final boolean getSkipIndexing()
```


Obtiene un valor que indica que la indexación del documento debe omitirse.


**Returns:**
boolean - Un valor que indica que la indexación del documento debe omitirse.

### setSkipIndexing(boolean value) {#setSkipIndexing-boolean-}
```
public final void setSkipIndexing(boolean value)
```


Establece un valor que indica que la indexación del documento debe omitirse.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | boolean | Un valor que indica que la indexación del documento debe omitirse. |
|

### getEncoding() {#getEncoding--}
```
public final String getEncoding()
```


Obtiene la codificación del documento.


**Returns:**
java.lang.String - La codificación del documento.

### setEncoding(String value) {#setEncoding-java.lang.String-}
```
public final void setEncoding(String value)
```


Establece la codificación del documento.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | java.lang.String | La codificación del documento. |
|

### getCustomExtractor() {#getCustomExtractor--}
```
public final IFieldExtractor getCustomExtractor()
```


Obtiene el extractor de texto personalizado.


**Returns:**
[IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) - The custom text extractor.

### setCustomExtractor(IFieldExtractor value) {#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-}
```
public final void setCustomExtractor(IFieldExtractor value)
```


Establece el extractor de texto personalizado.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | value | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | El extractor de texto personalizado. |
|

### getAdditionalFields() {#getAdditionalFields--}
```
public final DocumentField[] getAdditionalFields()
```


Obtiene los campos adicionales del documento.


**Returns:**
com.groupdocs.search.common.DocumentField[] - Los campos adicionales del documento.

### setAdditionalFields(DocumentField[] value) {#setAdditionalFields-com.groupdocs.search.common.DocumentField---}
```
public final void setAdditionalFields(DocumentField[] value)
```


Establece los campos adicionales del documento.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | value | [DocumentField\[\]](../../com.groupdocs.search.common/documentfield) | Los campos adicionales para el documento. |
|

### getAttributes() {#getAttributes--}
```
public final String[] getAttributes()
```


Obtiene los atributos del documento.


**Returns:**
java.lang.String[] - Los atributos del documento.

### setAttributes(String[] value) {#setAttributes-java.lang.String---}
```
public final void setAttributes(String[] value)
```


Establece los atributos del documento.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | java.lang.String[] | Los atributos del documento. |
|

