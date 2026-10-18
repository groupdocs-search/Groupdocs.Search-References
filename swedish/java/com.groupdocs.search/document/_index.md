---
title: "Dokument"
second_title: "GroupDocs.Search för Java API-referens"
description: "Representerar basklassen för dokument som läggs till i ett index från filsystemström eller struktur."
type: docs
weight: 13
url: /sv/java/com.groupdocs.search/document/
---
**Inheritance:**
java.lang.Object
```
public abstract class Document
```

Representerar basklassen för dokument som läggs till i ett index från filsystem, ström eller struktur. Innehåller statiska metoder för att skapa dokument från olika typer av källor.


**Learn more**

* [Indexing from different sources](../https://docs.groupdocs.com/search/java/indexing-from-different-sources/)

## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getDocumentSourceKind()](#getDocumentSourceKind--) | Hämtar dokumentkällans typ. |
|
|  | [getDocumentKey()](#getDocumentKey--) | Hämtar dokumentnyckeln som används för att identifiera dokumentet i ett index. |
|
|  | [isLazy()](#isLazy--) | Hämtar ett värde som indikerar om dokumentet laddas vid behov eller inte. |
|
|  | [getModificationDate()](#getModificationDate--) | Hämtar dokumentets senaste ändringsdatum. |
|
|  | [getExtension()](#getExtension--) | Hämtar filändelsen som används för denna dokumenttyp. |
|
|  | [getAdditionalFields()](#getAdditionalFields--) | Hämtar de ytterligare fälten för dokumentet. |
|
|  | [setAdditionalFields(DocumentField[] value)](#setAdditionalFields-com.groupdocs.search.common.DocumentField---) | Ställer in de ytterligare fälten för dokumentet. |
|
|  | [getAttributes()](#getAttributes--) | Hämtar dokumentets attribut. |
|
|  | [setAttributes(String[] value)](#setAttributes-java.lang.String---) | Ställer in dokumentets attribut. |
|
|  | [createFromFile(String filePath)](#createFromFile-java.lang.String-) | Skapar ett dokument från en fil. |
|
|  | [createFromStream(String documentKey, Date modificationDate, String extension, InputStream stream)](#createFromStream-java.lang.String-java.util.Date-java.lang.String-java.io.InputStream-) | Skapar ett dokument från en ström. |
|
|  | [createFromStructure(String documentKey, Date modificationDate, DocumentField[] fields)](#createFromStructure-java.lang.String-java.util.Date-com.groupdocs.search.common.DocumentField---) | Skapar ett dokument från en struktur som är en array av textfält. |
|
|  | [createLazy(DocumentSourceKind documentSourceKind, String documentKey, IDocumentLoader documentLoader)](#createLazy-com.groupdocs.search.common.DocumentSourceKind-java.lang.String-com.groupdocs.search.common.IDocumentLoader-) | Skapar ett fördröjt laddat dokument. |
|
|  | [toString()](#toString--) | Returnerar en  java.lang.String  som representerar det aktuella  Dokumentet . |
|
### getDocumentSourceKind() {#getDocumentSourceKind--}
```
public abstract DocumentSourceKind getDocumentSourceKind()
```


Hämtar dokumentkällans typ.


**Returns:**
[DocumentSourceKind](../../com.groupdocs.search.common/documentsourcekind) - The document source kind.

### getDocumentKey() {#getDocumentKey--}
```
public abstract String getDocumentKey()
```


Hämtar dokumentnyckeln som används för att identifiera dokumentet i ett index.


**Returns:**
java.lang.String - Dokumentnyckeln som används för att identifiera dokumentet i ett index.

### isLazy() {#isLazy--}
```
public abstract boolean isLazy()
```


Hämtar ett värde som indikerar om dokumentet laddas vid behov eller inte.


**Returns:**
boolean - Ett värde som indikerar om dokumentet laddas vid behov eller inte.

### getModificationDate() {#getModificationDate--}
```
public abstract Date getModificationDate()
```


Hämtar dokumentets senaste ändringsdatum.


**Returns:**
java.util.Date - Dokumentets senaste ändringsdatum.

### getExtension() {#getExtension--}
```
public abstract String getExtension()
```


Hämtar filändelsen som används för denna dokumenttyp.


**Returns:**
java.lang.String - Filändelsen som används för denna dokumenttyp.

### getAdditionalFields() {#getAdditionalFields--}
```
public DocumentField[] getAdditionalFields()
```


Hämtar de ytterligare fälten för dokumentet.


**Returns:**
com.groupdocs.search.common.DocumentField[] - De ytterligare fälten för dokumentet.

### setAdditionalFields(DocumentField[] value) {#setAdditionalFields-com.groupdocs.search.common.DocumentField---}
```
public void setAdditionalFields(DocumentField[] value)
```


Ställer in de ytterligare fälten för dokumentet.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | value | [DocumentField\[\]](../../com.groupdocs.search.common/documentfield) | De ytterligare fälten för dokumentet. |
|

### getAttributes() {#getAttributes--}
```
public String[] getAttributes()
```


Hämtar dokumentets attribut.


**Returns:**
java.lang.String[] - Dokumentets attribut.

### setAttributes(String[] value) {#setAttributes-java.lang.String---}
```
public void setAttributes(String[] value)
```


Ställer in dokumentets attribut.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | värde | java.lang.String[] | Dokumentets attribut. |
|

### createFromFile(String filePath) {#createFromFile-java.lang.String-}
```
public static Document createFromFile(String filePath)
```


Skapar ett dokument från en fil.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | filePath | java.lang.String | Dokumentets filsökväg. |
|

**Returns:**
[Document](../../com.groupdocs.search/document) - The created document.

### createFromStream(String documentKey, Date modificationDate, String extension, InputStream stream) {#createFromStream-java.lang.String-java.util.Date-java.lang.String-java.io.InputStream-}
```
public static Document createFromStream(String documentKey, Date modificationDate, String extension, InputStream stream)
```


Skapar ett dokument från en ström.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | documentKey | java.lang.String | Dokumentnyckeln. |
|
|  | modificationDate | java.util.Date | Dokumentets ändringsdatum. |
|
|  | filändelse | java.lang.String | Dokumentets filändelse. |
|
|  | ström | java.io.InputStream | Dokumentströmmen. |
|

**Returns:**
[Document](../../com.groupdocs.search/document) - The created document.

### createFromStructure(String documentKey, Date modificationDate, DocumentField[] fields) {#createFromStructure-java.lang.String-java.util.Date-com.groupdocs.search.common.DocumentField---}
```
public static Document createFromStructure(String documentKey, Date modificationDate, DocumentField[] fields)
```


Skapar ett dokument från en struktur som är en array av textfält.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | documentKey | java.lang.String | Dokumentnyckeln. |
|
|  | modificationDate | java.util.Date | Dokumentets ändringsdatum. |
|
|  | fields | [DocumentField\[\]](../../com.groupdocs.search.common/documentfield) | Dokumentfält. |
|

**Returns:**
[Document](../../com.groupdocs.search/document) - The created document.

### createLazy(DocumentSourceKind documentSourceKind, String documentKey, IDocumentLoader documentLoader) {#createLazy-com.groupdocs.search.common.DocumentSourceKind-java.lang.String-com.groupdocs.search.common.IDocumentLoader-}
```
public static Document createLazy(DocumentSourceKind documentSourceKind, String documentKey, IDocumentLoader documentLoader)
```


Skapar ett fördröjt laddat dokument.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | documentSourceKind | [DocumentSourceKind](../../com.groupdocs.search.common/documentsourcekind) | Dokumentets källtyp. Detta värde måste matcha typen av det inlästa dokumentet. |
|
|  | documentKey | java.lang.String | Dokumentnyckeln. Detta värde måste matcha nyckeln för det inlästa dokumentet. |
|
|  | documentLoader | [IDocumentLoader](../../com.groupdocs.search.common/idocumentloader) | Dokumentladdaren. |
|

**Returns:**
[Document](../../com.groupdocs.search/document) - The created document.

### toString() {#toString--}
```
public String toString()
```


Returnerar en  java.lang.String  som representerar det aktuella  Dokumentet .


**Returns:**
java.lang.String - En  java.lang.String  som representerar det aktuella  Dokumentet .

