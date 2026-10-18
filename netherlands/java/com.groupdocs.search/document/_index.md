---
title: "Document"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Stelt de basisklasse voor documenten voor die aan een index worden toegevoegd vanuit een bestandssysteemstream of structuur."
type: docs
weight: 13
url: /nl/java/com.groupdocs.search/document/
---
**Inheritance:**
java.lang.Object
```
public abstract class Document
```

Stelt de basisklasse voor documenten voor die aan een index worden toegevoegd vanuit een bestandssysteem, stream of structuur. Bevat statische methoden voor het maken van documenten uit verschillende soorten bronnen.


**Learn more**

* [Indexing from different sources](../https://docs.groupdocs.com/search/java/indexing-from-different-sources/)

## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getDocumentSourceKind()](#getDocumentSourceKind--) | Haalt het type documentbron op. |
|
|  | [getDocumentKey()](#getDocumentKey--) | Haalt de documentsleutel op die wordt gebruikt om het document binnen een index te identificeren. |
|
|  | [isLazy()](#isLazy--) | Haalt een waarde op die aangeeft of het document al dan niet naar behoefte wordt geladen. |
|
|  | [getModificationDate()](#getModificationDate--) | Haalt de laatste wijzigingsdatum van het document op. |
|
|  | [getExtension()](#getExtension--) | Haalt de extensie op die voor dit documenttype wordt gebruikt. |
|
|  | [getAdditionalFields()](#getAdditionalFields--) | Haalt de extra velden voor het document op. |
|
|  | [setAdditionalFields(DocumentField[] value)](#setAdditionalFields-com.groupdocs.search.common.DocumentField---) | Stelt de extra velden voor het document in. |
|
|  | [getAttributes()](#getAttributes--) | Haalt de attributen van het document op. |
|
|  | [setAttributes(String[] value)](#setAttributes-java.lang.String---) | Stelt de attributen van het document in. |
|
|  | [createFromFile(String filePath)](#createFromFile-java.lang.String-) | Maakt een document aan vanuit een bestand. |
|
|  | [createFromStream(String documentKey, Date modificationDate, String extension, InputStream stream)](#createFromStream-java.lang.String-java.util.Date-java.lang.String-java.io.InputStream-) | Maakt een document aan vanuit een stream. |
|
|  | [createFromStructure(String documentKey, Date modificationDate, DocumentField[] fields)](#createFromStructure-java.lang.String-java.util.Date-com.groupdocs.search.common.DocumentField---) | Maakt een document aan vanuit een structuur die een array van tekstvelden is. |
|
|  | [createLazy(DocumentSourceKind documentSourceKind, String documentKey, IDocumentLoader documentLoader)](#createLazy-com.groupdocs.search.common.DocumentSourceKind-java.lang.String-com.groupdocs.search.common.IDocumentLoader-) | Maakt een lui geladen document aan. |
|
|  | [toString()](#toString--) | Retourneert een  java.lang.String  die de huidige  Document  weergeeft. |
|
### getDocumentSourceKind() {#getDocumentSourceKind--}
```
public abstract DocumentSourceKind getDocumentSourceKind()
```


Haalt het type documentbron op.


**Returns:**
[DocumentSourceKind](../../com.groupdocs.search.common/documentsourcekind) - The document source kind.

### getDocumentKey() {#getDocumentKey--}
```
public abstract String getDocumentKey()
```


Haalt de documentsleutel op die wordt gebruikt om het document binnen een index te identificeren.


**Returns:**
java.lang.String - De documentsleutel die wordt gebruikt om het document binnen een index te identificeren.

### isLazy() {#isLazy--}
```
public abstract boolean isLazy()
```


Haalt een waarde op die aangeeft of het document al dan niet naar behoefte wordt geladen.


**Returns:**
boolean - Een waarde die aangeeft of het document al dan niet naar behoefte wordt geladen.

### getModificationDate() {#getModificationDate--}
```
public abstract Date getModificationDate()
```


Haalt de laatste wijzigingsdatum van het document op.


**Returns:**
java.util.Date - De laatste wijzigingsdatum van het document.

### getExtension() {#getExtension--}
```
public abstract String getExtension()
```


Haalt de extensie op die voor dit documenttype wordt gebruikt.


**Returns:**
java.lang.String - De extensie die voor dit documenttype wordt gebruikt.

### getAdditionalFields() {#getAdditionalFields--}
```
public DocumentField[] getAdditionalFields()
```


Haalt de extra velden voor het document op.


**Returns:**
com.groupdocs.search.common.DocumentField[] - De extra velden voor het document.

### setAdditionalFields(DocumentField[] value) {#setAdditionalFields-com.groupdocs.search.common.DocumentField---}
```
public void setAdditionalFields(DocumentField[] value)
```


Stelt de extra velden voor het document in.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | value | [DocumentField\[\]](../../com.groupdocs.search.common/documentfield) | De extra velden voor het document. |
|

### getAttributes() {#getAttributes--}
```
public String[] getAttributes()
```


Haalt de attributen van het document op.


**Returns:**
java.lang.String[] - De attributen van het document.

### setAttributes(String[] value) {#setAttributes-java.lang.String---}
```
public void setAttributes(String[] value)
```


Stelt de attributen van het document in.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | waarde | java.lang.String[] | De attributen van het document. |
|

### createFromFile(String filePath) {#createFromFile-java.lang.String-}
```
public static Document createFromFile(String filePath)
```


Maakt een document aan vanuit een bestand.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | filePath | java.lang.String | Het bestandspad van het document. |
|

**Returns:**
[Document](../../com.groupdocs.search/document) - The created document.

### createFromStream(String documentKey, Date modificationDate, String extension, InputStream stream) {#createFromStream-java.lang.String-java.util.Date-java.lang.String-java.io.InputStream-}
```
public static Document createFromStream(String documentKey, Date modificationDate, String extension, InputStream stream)
```


Maakt een document aan vanuit een stream.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | documentKey | java.lang.String | De documentsleutel. |
|
|  | modificationDate | java.util.Date | De wijzigingsdatum van het document. |
|
|  | extension | java.lang.String | De extensie van het document. |
|
|  | stream | java.io.InputStream | De documentstroom. |
|

**Returns:**
[Document](../../com.groupdocs.search/document) - The created document.

### createFromStructure(String documentKey, Date modificationDate, DocumentField[] fields) {#createFromStructure-java.lang.String-java.util.Date-com.groupdocs.search.common.DocumentField---}
```
public static Document createFromStructure(String documentKey, Date modificationDate, DocumentField[] fields)
```


Maakt een document aan vanuit een structuur die een array van tekstvelden is.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | documentKey | java.lang.String | De documentsleutel. |
|
|  | modificationDate | java.util.Date | De wijzigingsdatum van het document. |
|
|  | fields | [DocumentField\[\]](../../com.groupdocs.search.common/documentfield) | De documentvelden. |
|

**Returns:**
[Document](../../com.groupdocs.search/document) - The created document.

### createLazy(DocumentSourceKind documentSourceKind, String documentKey, IDocumentLoader documentLoader) {#createLazy-com.groupdocs.search.common.DocumentSourceKind-java.lang.String-com.groupdocs.search.common.IDocumentLoader-}
```
public static Document createLazy(DocumentSourceKind documentSourceKind, String documentKey, IDocumentLoader documentLoader)
```


Maakt een lui geladen document aan.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | documentSourceKind | [DocumentSourceKind](../../com.groupdocs.search.common/documentsourcekind) | Het type documentbron. Deze waarde moet overeenkomen met het type van het geladen document. |
|
|  | documentKey | java.lang.String | De documentsleutel. Deze waarde moet overeenkomen met de sleutel van het geladen document. |
|
|  | documentLoader | [IDocumentLoader](../../com.groupdocs.search.common/idocumentloader) | De documentlader. |
|

**Returns:**
[Document](../../com.groupdocs.search/document) - The created document.

### toString() {#toString--}
```
public String toString()
```


Retourneert een  java.lang.String  die de huidige  Document  weergeeft.


**Returns:**
java.lang.String - Een  java.lang.String  die de huidige  Document  vertegenwoordigt.

