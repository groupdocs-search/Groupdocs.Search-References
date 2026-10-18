---
title: "DocumentFilter"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Representa la clase base para filtros de documentos."
type: docs
weight: 14
url: /es/java/com.groupdocs.search/documentfilter/
---
**Inheritance:**
java.lang.Object
```
public abstract class DocumentFilter
```

Representa la clase base para filtros de documentos. Contiene métodos para la creación de instancias de filtros de documentos.


**Learn more**

* [Document filtering during indexing](../https://docs.groupdocs.com/display/searchjava/Document+filtering+during+indexing)

## Constructores

| Constructor | Descripción |
| --- | --- |
| [DocumentFilter()](#DocumentFilter--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
|  | [toString()](#toString--) | Devuelve la representación en cadena de un filtro de documentos. |
|
|  | [createCreationTimeLowerBound(Date lowerBound)](#createCreationTimeLowerBound-java.util.Date-) | Crea un filtro para omitir documentos con fecha de creación anterior al límite inferior. |
|
|  | [createCreationTimeUpperBound(Date upperBound)](#createCreationTimeUpperBound-java.util.Date-) | Crea un filtro para omitir documentos con fecha de creación posterior al límite superior. |
|
|  | [createCreationTimeRange(Date lowerBound, Date upperBound)](#createCreationTimeRange-java.util.Date-java.util.Date-) | Crea un filtro para omitir documentos con fecha de creación fuera del rango especificado. |
|
|  | [createModificationTimeLowerBound(Date lowerBound)](#createModificationTimeLowerBound-java.util.Date-) | Crea un filtro para omitir documentos con fecha de modificación anterior al límite inferior. |
|
|  | [createModificationTimeUpperBound(Date upperBound)](#createModificationTimeUpperBound-java.util.Date-) | Crea un filtro para omitir documentos con fecha de modificación posterior al límite superior. |
|
|  | [createModificationTimeRange(Date lowerBound, Date upperBound)](#createModificationTimeRange-java.util.Date-java.util.Date-) | Crea un filtro para omitir documentos con fecha de modificación fuera del rango especificado. |
|
|  | [createFilePathRegularExpression(String pattern)](#createFilePathRegularExpression-java.lang.String-) | Crea un filtro para omitir documentos que no coinciden con una expresión regular. |
|
|  | [createFilePathRegularExpression(String pattern, int options)](#createFilePathRegularExpression-java.lang.String-int-) | Crea un filtro para omitir documentos que no coinciden con una expresión regular. |
|
|  | [createFileLengthLowerBound(long lowerBound)](#createFileLengthLowerBound-long-) | Crea un filtro para omitir documentos con una longitud menor al límite inferior. |
|
|  | [createFileLengthUpperBound(long upperBound)](#createFileLengthUpperBound-long-) | Crea un filtro para omitir documentos con una longitud mayor al límite superior. |
|
|  | [createFileLengthRange(long lowerBound, long upperBound)](#createFileLengthRange-long-long-) | Crea un filtro para omitir documentos fuera del rango de longitud de documento especificado. |
|
|  | [createFileExtension(String[] extensions)](#createFileExtension-java.lang.String...-) | Crea un filtro para omitir documentos que no tienen una extensión permitida. |
|
|  | [createNot(DocumentFilter innerFilter)](#createNot-com.groupdocs.search.DocumentFilter-) | Crea un filtro que tiene lógica inversa en relación con el filtro interno especificado. |
|
|  | [createAnd(DocumentFilter[] filters)](#createAnd-com.groupdocs.search.DocumentFilter...-) | Crea una conjunción lógica de los filtros especificados. |
|
|  | [createOr(DocumentFilter[] filters)](#createOr-com.groupdocs.search.DocumentFilter...-) | Crea una disyunción lógica de los filtros especificados. |
|
### DocumentFilter() {#DocumentFilter--}
```
public DocumentFilter()
```


### toString() {#toString--}
```
public abstract String toString()
```


Devuelve la representación en cadena de un filtro de documentos.


**Returns:**
java.lang.String - Representación en cadena de un filtro de documentos.

### createCreationTimeLowerBound(Date lowerBound) {#createCreationTimeLowerBound-java.util.Date-}
```
public static DocumentFilter createCreationTimeLowerBound(Date lowerBound)
```


Crea un filtro para omitir documentos con fecha de creación anterior al límite inferior.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | lowerBound | java.util.Date | El límite inferior del tiempo de creación del documento. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document creation time.

### createCreationTimeUpperBound(Date upperBound) {#createCreationTimeUpperBound-java.util.Date-}
```
public static DocumentFilter createCreationTimeUpperBound(Date upperBound)
```


Crea un filtro para omitir documentos con fecha de creación posterior al límite superior.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | upperBound | java.util.Date | El límite superior del tiempo de creación del documento. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document creation time.

### createCreationTimeRange(Date lowerBound, Date upperBound) {#createCreationTimeRange-java.util.Date-java.util.Date-}
```
public static DocumentFilter createCreationTimeRange(Date lowerBound, Date upperBound)
```


Crea un filtro para omitir documentos con fecha de creación fuera del rango especificado.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | lowerBound | java.util.Date | El límite inferior del tiempo de creación del documento. |
|
|  | upperBound | java.util.Date | El límite superior del tiempo de creación del documento. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document creation time.

### createModificationTimeLowerBound(Date lowerBound) {#createModificationTimeLowerBound-java.util.Date-}
```
public static DocumentFilter createModificationTimeLowerBound(Date lowerBound)
```


Crea un filtro para omitir documentos con fecha de modificación anterior al límite inferior.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | lowerBound | java.util.Date | El límite inferior del tiempo de modificación del documento. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document modification time.

### createModificationTimeUpperBound(Date upperBound) {#createModificationTimeUpperBound-java.util.Date-}
```
public static DocumentFilter createModificationTimeUpperBound(Date upperBound)
```


Crea un filtro para omitir documentos con fecha de modificación posterior al límite superior.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | upperBound | java.util.Date | El límite superior del tiempo de modificación del documento. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document modification time.

### createModificationTimeRange(Date lowerBound, Date upperBound) {#createModificationTimeRange-java.util.Date-java.util.Date-}
```
public static DocumentFilter createModificationTimeRange(Date lowerBound, Date upperBound)
```


Crea un filtro para omitir documentos con fecha de modificación fuera del rango especificado.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | lowerBound | java.util.Date | El límite inferior del tiempo de modificación del documento. |
|
|  | upperBound | java.util.Date | El límite superior del tiempo de modificación del documento. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document modification time.

### createFilePathRegularExpression(String pattern) {#createFilePathRegularExpression-java.lang.String-}
```
public static DocumentFilter createFilePathRegularExpression(String pattern)
```


Crea un filtro para omitir documentos que no coinciden con una expresión regular. La expresión regular se aplica a la ruta completa de un documento.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | pattern | java.lang.String | El patrón de expresión regular. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by file name.

### createFilePathRegularExpression(String pattern, int options) {#createFilePathRegularExpression-java.lang.String-int-}
```
public static DocumentFilter createFilePathRegularExpression(String pattern, int options)
```


Crea un filtro para omitir documentos que no coinciden con una expresión regular. La expresión regular se aplica a la ruta completa de un documento.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | pattern | java.lang.String | El patrón de expresión regular. |
|
|  | options | int | Las opciones de expresión regular. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by file name.

### createFileLengthLowerBound(long lowerBound) {#createFileLengthLowerBound-long-}
```
public static DocumentFilter createFileLengthLowerBound(long lowerBound)
```


Crea un filtro para omitir documentos con una longitud menor al límite inferior.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | lowerBound | long | El límite inferior de la longitud del documento. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document length.

### createFileLengthUpperBound(long upperBound) {#createFileLengthUpperBound-long-}
```
public static DocumentFilter createFileLengthUpperBound(long upperBound)
```


Crea un filtro para omitir documentos con una longitud mayor al límite superior.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | upperBound | long | El límite superior de la longitud del documento. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document length.

### createFileLengthRange(long lowerBound, long upperBound) {#createFileLengthRange-long-long-}
```
public static DocumentFilter createFileLengthRange(long lowerBound, long upperBound)
```


Crea un filtro para omitir documentos fuera del rango de longitud de documento especificado.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | lowerBound | long | El límite inferior de la longitud del documento. |
|
|  | upperBound | long | El límite superior de la longitud del documento. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document length.

### createFileExtension(String[] extensions) {#createFileExtension-java.lang.String...-}
```
public static DocumentFilter createFileExtension(String[] extensions)
```


Crea un filtro para omitir documentos que no tienen una extensión permitida.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | extensions | java.lang.String[] | La lista de extensiones permitidas. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document extension.

### createNot(DocumentFilter innerFilter) {#createNot-com.groupdocs.search.DocumentFilter-}
```
public static DocumentFilter createNot(DocumentFilter innerFilter)
```


Crea un filtro que tiene lógica inversa en relación con el filtro interno especificado.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | innerFilter | [DocumentFilter](../../com.groupdocs.search/documentfilter) | El filtro interno del documento. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - An inverted document filter.

### createAnd(DocumentFilter[] filters) {#createAnd-com.groupdocs.search.DocumentFilter...-}
```
public static DocumentFilter createAnd(DocumentFilter[] filters)
```


Crea una conjunción lógica de los filtros especificados.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | filters | [DocumentFilter\[\]](../../com.groupdocs.search/documentfilter) | Los filtros del documento. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter that represents result of conjunction of the specified filters.

### createOr(DocumentFilter[] filters) {#createOr-com.groupdocs.search.DocumentFilter...-}
```
public static DocumentFilter createOr(DocumentFilter[] filters)
```


Crea una disyunción lógica de los filtros especificados.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | filters | [DocumentFilter\[\]](../../com.groupdocs.search/documentfilter) | Los filtros del documento. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter that represents result of disjunction of the specified filters.

