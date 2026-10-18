---
title: "DocumentFilter"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Rappresenta la classe base per i filtri dei documenti."
type: docs
weight: 14
url: /it/java/com.groupdocs.search/documentfilter/
---
**Inheritance:**
java.lang.Object
```
public abstract class DocumentFilter
```

Rappresenta la classe base per i filtri di documento. Contiene metodi per la creazione di istanze di filtri di documento.


**Learn more**

* [Document filtering during indexing](../https://docs.groupdocs.com/display/searchjava/Document+filtering+during+indexing)

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [DocumentFilter()](#DocumentFilter--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [toString()](#toString--) | Restituisce la rappresentazione stringa di un filtro di documento. |
|
|  | [createCreationTimeLowerBound(Date lowerBound)](#createCreationTimeLowerBound-java.util.Date-) | Crea un filtro per saltare i documenti con data di creazione precedente al limite inferiore. |
|
|  | [createCreationTimeUpperBound(Date upperBound)](#createCreationTimeUpperBound-java.util.Date-) | Crea un filtro per saltare i documenti con data di creazione successiva al limite superiore. |
|
|  | [createCreationTimeRange(Date lowerBound, Date upperBound)](#createCreationTimeRange-java.util.Date-java.util.Date-) | Crea un filtro per saltare i documenti con data di creazione fuori dall'intervallo specificato. |
|
|  | [createModificationTimeLowerBound(Date lowerBound)](#createModificationTimeLowerBound-java.util.Date-) | Crea un filtro per saltare i documenti con data di modifica precedente al limite inferiore. |
|
|  | [createModificationTimeUpperBound(Date upperBound)](#createModificationTimeUpperBound-java.util.Date-) | Crea un filtro per saltare i documenti con data di modifica successiva al limite superiore. |
|
|  | [createModificationTimeRange(Date lowerBound, Date upperBound)](#createModificationTimeRange-java.util.Date-java.util.Date-) | Crea un filtro per saltare i documenti con data di modifica fuori dall'intervallo specificato. |
|
|  | [createFilePathRegularExpression(String pattern)](#createFilePathRegularExpression-java.lang.String-) | Crea un filtro per saltare i documenti che non corrispondono a un'espressione regolare. |
|
|  | [createFilePathRegularExpression(String pattern, int options)](#createFilePathRegularExpression-java.lang.String-int-) | Crea un filtro per saltare i documenti che non corrispondono a un'espressione regolare. |
|
|  | [createFileLengthLowerBound(long lowerBound)](#createFileLengthLowerBound-long-) | Crea un filtro per saltare i documenti con lunghezza inferiore al limite inferiore. |
|
|  | [createFileLengthUpperBound(long upperBound)](#createFileLengthUpperBound-long-) | Crea un filtro per saltare i documenti con lunghezza superiore al limite superiore. |
|
|  | [createFileLengthRange(long lowerBound, long upperBound)](#createFileLengthRange-long-long-) | Crea un filtro per saltare i documenti fuori dall'intervallo di lunghezza specificato. |
|
|  | [createFileExtension(String[] extensions)](#createFileExtension-java.lang.String...-) | Crea un filtro per saltare i documenti che non hanno un'estensione consentita. |
|
|  | [createNot(DocumentFilter innerFilter)](#createNot-com.groupdocs.search.DocumentFilter-) | Crea un filtro che ha una logica inversa rispetto al filtro interno specificato. |
|
|  | [createAnd(DocumentFilter[] filters)](#createAnd-com.groupdocs.search.DocumentFilter...-) | Crea una congiunzione logica dei filtri specificati. |
|
|  | [createOr(DocumentFilter[] filters)](#createOr-com.groupdocs.search.DocumentFilter...-) | Crea una disgiunzione logica dei filtri specificati. |
|
### DocumentFilter() {#DocumentFilter--}
```
public DocumentFilter()
```


### toString() {#toString--}
```
public abstract String toString()
```


Restituisce la rappresentazione stringa di un filtro di documento.


**Returns:**
java.lang.String - Rappresentazione stringa di un filtro di documento.

### createCreationTimeLowerBound(Date lowerBound) {#createCreationTimeLowerBound-java.util.Date-}
```
public static DocumentFilter createCreationTimeLowerBound(Date lowerBound)
```


Crea un filtro per saltare i documenti con data di creazione precedente al limite inferiore.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | lowerBound | java.util.Date | Il limite inferiore del tempo di creazione del documento. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document creation time.

### createCreationTimeUpperBound(Date upperBound) {#createCreationTimeUpperBound-java.util.Date-}
```
public static DocumentFilter createCreationTimeUpperBound(Date upperBound)
```


Crea un filtro per saltare i documenti con data di creazione successiva al limite superiore.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | upperBound | java.util.Date | Il limite superiore del tempo di creazione del documento. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document creation time.

### createCreationTimeRange(Date lowerBound, Date upperBound) {#createCreationTimeRange-java.util.Date-java.util.Date-}
```
public static DocumentFilter createCreationTimeRange(Date lowerBound, Date upperBound)
```


Crea un filtro per saltare i documenti con data di creazione fuori dall'intervallo specificato.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | lowerBound | java.util.Date | Il limite inferiore del tempo di creazione del documento. |
|
|  | upperBound | java.util.Date | Il limite superiore del tempo di creazione del documento. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document creation time.

### createModificationTimeLowerBound(Date lowerBound) {#createModificationTimeLowerBound-java.util.Date-}
```
public static DocumentFilter createModificationTimeLowerBound(Date lowerBound)
```


Crea un filtro per saltare i documenti con data di modifica precedente al limite inferiore.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | lowerBound | java.util.Date | Il limite inferiore del tempo di modifica del documento. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document modification time.

### createModificationTimeUpperBound(Date upperBound) {#createModificationTimeUpperBound-java.util.Date-}
```
public static DocumentFilter createModificationTimeUpperBound(Date upperBound)
```


Crea un filtro per saltare i documenti con data di modifica successiva al limite superiore.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | upperBound | java.util.Date | Il limite superiore del tempo di modifica del documento. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document modification time.

### createModificationTimeRange(Date lowerBound, Date upperBound) {#createModificationTimeRange-java.util.Date-java.util.Date-}
```
public static DocumentFilter createModificationTimeRange(Date lowerBound, Date upperBound)
```


Crea un filtro per saltare i documenti con data di modifica fuori dall'intervallo specificato.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | lowerBound | java.util.Date | Il limite inferiore del tempo di modifica del documento. |
|
|  | upperBound | java.util.Date | Il limite superiore del tempo di modifica del documento. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document modification time.

### createFilePathRegularExpression(String pattern) {#createFilePathRegularExpression-java.lang.String-}
```
public static DocumentFilter createFilePathRegularExpression(String pattern)
```


Crea un filtro per saltare i documenti che non corrispondono a un'espressione regolare. L'espressione regolare è applicata al percorso completo di un documento.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | pattern | java.lang.String | Il pattern dell'espressione regolare. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by file name.

### createFilePathRegularExpression(String pattern, int options) {#createFilePathRegularExpression-java.lang.String-int-}
```
public static DocumentFilter createFilePathRegularExpression(String pattern, int options)
```


Crea un filtro per saltare i documenti che non corrispondono a un'espressione regolare. L'espressione regolare è applicata al percorso completo di un documento.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | pattern | java.lang.String | Il pattern dell'espressione regolare. |
|
|  | options | int | Le opzioni dell'espressione regolare. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by file name.

### createFileLengthLowerBound(long lowerBound) {#createFileLengthLowerBound-long-}
```
public static DocumentFilter createFileLengthLowerBound(long lowerBound)
```


Crea un filtro per saltare i documenti con lunghezza inferiore al limite inferiore.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | lowerBound | long | Il limite inferiore della lunghezza del documento. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document length.

### createFileLengthUpperBound(long upperBound) {#createFileLengthUpperBound-long-}
```
public static DocumentFilter createFileLengthUpperBound(long upperBound)
```


Crea un filtro per saltare i documenti con lunghezza superiore al limite superiore.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | upperBound | long | Il limite superiore della lunghezza del documento. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document length.

### createFileLengthRange(long lowerBound, long upperBound) {#createFileLengthRange-long-long-}
```
public static DocumentFilter createFileLengthRange(long lowerBound, long upperBound)
```


Crea un filtro per saltare i documenti fuori dall'intervallo di lunghezza specificato.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | lowerBound | long | Il limite inferiore della lunghezza del documento. |
|
|  | upperBound | long | Il limite superiore della lunghezza del documento. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document length.

### createFileExtension(String[] extensions) {#createFileExtension-java.lang.String...-}
```
public static DocumentFilter createFileExtension(String[] extensions)
```


Crea un filtro per saltare i documenti che non hanno un'estensione consentita.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | extensions | java.lang.String[] | L'elenco delle estensioni consentite. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document extension.

### createNot(DocumentFilter innerFilter) {#createNot-com.groupdocs.search.DocumentFilter-}
```
public static DocumentFilter createNot(DocumentFilter innerFilter)
```


Crea un filtro che ha una logica inversa rispetto al filtro interno specificato.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | innerFilter | [DocumentFilter](../../com.groupdocs.search/documentfilter) | Il filtro interno del documento. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - An inverted document filter.

### createAnd(DocumentFilter[] filters) {#createAnd-com.groupdocs.search.DocumentFilter...-}
```
public static DocumentFilter createAnd(DocumentFilter[] filters)
```


Crea una congiunzione logica dei filtri specificati.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | filters | [DocumentFilter\[\]](../../com.groupdocs.search/documentfilter) | I filtri del documento. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter that represents result of conjunction of the specified filters.

### createOr(DocumentFilter[] filters) {#createOr-com.groupdocs.search.DocumentFilter...-}
```
public static DocumentFilter createOr(DocumentFilter[] filters)
```


Crea una disgiunzione logica dei filtri specificati.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | filters | [DocumentFilter\[\]](../../com.groupdocs.search/documentfilter) | I filtri del documento. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter that represents result of disjunction of the specified filters.

