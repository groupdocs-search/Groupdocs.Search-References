---
title: "Dokument"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Stellt die Basisklasse für Dokumente dar, die einem Index aus Dateisystem-Stream oder Struktur hinzugefügt werden."
type: docs
weight: 13
url: /de/java/com.groupdocs.search/document/
---
**Inheritance:**
java.lang.Object
```
public abstract class Document
```

Stellt die Basisklasse für Dokumente dar, die einem Index aus Dateisystem, Stream oder Struktur hinzugefügt werden. Enthält statische Methoden zum Erstellen von Dokumenten aus verschiedenen Quelltypen.


**Learn more**

* [Indexing from different sources](../https://docs.groupdocs.com/search/java/indexing-from-different-sources/)

## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getDocumentSourceKind()](#getDocumentSourceKind--) | Liefert die Art der Dokumentquelle. |
|
|  | [getDocumentKey()](#getDocumentKey--) | Liefert den Dokumentenschlüssel, der verwendet wird, um das Dokument innerhalb eines Index zu identifizieren. |
|
|  | [isLazy()](#isLazy--) | Liefert einen Wert, der angibt, ob das Dokument bei Bedarf geladen wird oder nicht. |
|
|  | [getModificationDate()](#getModificationDate--) | Liefert das letzte Änderungsdatum des Dokuments. |
|
|  | [getExtension()](#getExtension--) | Liefert die für diesen Dokumenttyp verwendete Erweiterung. |
|
|  | [getAdditionalFields()](#getAdditionalFields--) | Liefert die zusätzlichen Felder für das Dokument. |
|
|  | [setAdditionalFields(DocumentField[] value)](#setAdditionalFields-com.groupdocs.search.common.DocumentField---) | Setzt die zusätzlichen Felder für das Dokument. |
|
|  | [getAttributes()](#getAttributes--) | Liefert die Attribute des Dokuments. |
|
|  | [setAttributes(String[] value)](#setAttributes-java.lang.String---) | Setzt die Attribute des Dokuments. |
|
|  | [createFromFile(String filePath)](#createFromFile-java.lang.String-) | Erstellt ein Dokument aus einer Datei. |
|
|  | [createFromStream(String documentKey, Date modificationDate, String extension, InputStream stream)](#createFromStream-java.lang.String-java.util.Date-java.lang.String-java.io.InputStream-) | Erstellt ein Dokument aus einem Stream. |
|
|  | [createFromStructure(String documentKey, Date modificationDate, DocumentField[] fields)](#createFromStructure-java.lang.String-java.util.Date-com.groupdocs.search.common.DocumentField---) | Erstellt ein Dokument aus einer Struktur, die ein Array von Textfeldern ist. |
|
|  | [createLazy(DocumentSourceKind documentSourceKind, String documentKey, IDocumentLoader documentLoader)](#createLazy-com.groupdocs.search.common.DocumentSourceKind-java.lang.String-com.groupdocs.search.common.IDocumentLoader-) | Erstellt ein lazy-loaded Dokument. |
|
|  | [toString()](#toString--) | Gibt einen  java.lang.String  zurück, der das aktuelle  Document  darstellt. |
|
### getDocumentSourceKind() {#getDocumentSourceKind--}
```
public abstract DocumentSourceKind getDocumentSourceKind()
```


Liefert die Art der Dokumentquelle.


**Returns:**
[DocumentSourceKind](../../com.groupdocs.search.common/documentsourcekind) - The document source kind.

### getDocumentKey() {#getDocumentKey--}
```
public abstract String getDocumentKey()
```


Liefert den Dokumentenschlüssel, der verwendet wird, um das Dokument innerhalb eines Index zu identifizieren.


**Returns:**
java.lang.String - Der Dokumentenschlüssel, der verwendet wird, um das Dokument innerhalb eines Index zu identifizieren.

### isLazy() {#isLazy--}
```
public abstract boolean isLazy()
```


Liefert einen Wert, der angibt, ob das Dokument bei Bedarf geladen wird oder nicht.


**Returns:**
boolean - Ein Wert, der angibt, ob das Dokument bei Bedarf geladen wird oder nicht.

### getModificationDate() {#getModificationDate--}
```
public abstract Date getModificationDate()
```


Liefert das letzte Änderungsdatum des Dokuments.


**Returns:**
java.util.Date - Das letzte Änderungsdatum des Dokuments.

### getExtension() {#getExtension--}
```
public abstract String getExtension()
```


Liefert die für diesen Dokumenttyp verwendete Erweiterung.


**Returns:**
java.lang.String - Die für diesen Dokumenttyp verwendete Erweiterung.

### getAdditionalFields() {#getAdditionalFields--}
```
public DocumentField[] getAdditionalFields()
```


Liefert die zusätzlichen Felder für das Dokument.


**Returns:**
com.groupdocs.search.common.DocumentField[] - Die zusätzlichen Felder für das Dokument.

### setAdditionalFields(DocumentField[] value) {#setAdditionalFields-com.groupdocs.search.common.DocumentField---}
```
public void setAdditionalFields(DocumentField[] value)
```


Setzt die zusätzlichen Felder für das Dokument.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | value | [DocumentField\[\]](../../com.groupdocs.search.common/documentfield) | Die zusätzlichen Felder für das Dokument. |
|

### getAttributes() {#getAttributes--}
```
public String[] getAttributes()
```


Liefert die Attribute des Dokuments.


**Returns:**
java.lang.String[] - Die Attribute des Dokuments.

### setAttributes(String[] value) {#setAttributes-java.lang.String---}
```
public void setAttributes(String[] value)
```


Setzt die Attribute des Dokuments.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | java.lang.String[] | Die Attribute des Dokuments. |
|

### createFromFile(String filePath) {#createFromFile-java.lang.String-}
```
public static Document createFromFile(String filePath)
```


Erstellt ein Dokument aus einer Datei.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | filePath | java.lang.String | Der Dateipfad des Dokuments. |
|

**Returns:**
[Document](../../com.groupdocs.search/document) - The created document.

### createFromStream(String documentKey, Date modificationDate, String extension, InputStream stream) {#createFromStream-java.lang.String-java.util.Date-java.lang.String-java.io.InputStream-}
```
public static Document createFromStream(String documentKey, Date modificationDate, String extension, InputStream stream)
```


Erstellt ein Dokument aus einem Stream.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | documentKey | java.lang.String | Der Dokumentenschlüssel. |
|
|  | modificationDate | java.util.Date | Das Änderungsdatum des Dokuments. |
|
|  | extension | java.lang.String | Die Dokumenterweiterung. |
|
|  | stream | java.io.InputStream | Der Dokumenten-Stream. |
|

**Returns:**
[Document](../../com.groupdocs.search/document) - The created document.

### createFromStructure(String documentKey, Date modificationDate, DocumentField[] fields) {#createFromStructure-java.lang.String-java.util.Date-com.groupdocs.search.common.DocumentField---}
```
public static Document createFromStructure(String documentKey, Date modificationDate, DocumentField[] fields)
```


Erstellt ein Dokument aus einer Struktur, die ein Array von Textfeldern ist.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | documentKey | java.lang.String | Der Dokumentenschlüssel. |
|
|  | modificationDate | java.util.Date | Das Änderungsdatum des Dokuments. |
|
|  | fields | [DocumentField\[\]](../../com.groupdocs.search.common/documentfield) | Die Dokumentfelder. |
|

**Returns:**
[Document](../../com.groupdocs.search/document) - The created document.

### createLazy(DocumentSourceKind documentSourceKind, String documentKey, IDocumentLoader documentLoader) {#createLazy-com.groupdocs.search.common.DocumentSourceKind-java.lang.String-com.groupdocs.search.common.IDocumentLoader-}
```
public static Document createLazy(DocumentSourceKind documentSourceKind, String documentKey, IDocumentLoader documentLoader)
```


Erstellt ein lazy-loaded Dokument.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | documentSourceKind | [DocumentSourceKind](../../com.groupdocs.search.common/documentsourcekind) | Die Quellart des Dokuments. Dieser Wert muss mit der Art des geladenen Dokuments übereinstimmen. |
|
|  | documentKey | java.lang.String | Der Dokumentenschlüssel. Dieser Wert muss mit dem Schlüssel des geladenen Dokuments übereinstimmen. |
|
|  | documentLoader | [IDocumentLoader](../../com.groupdocs.search.common/idocumentloader) | Der Dokumenten-Loader. |
|

**Returns:**
[Document](../../com.groupdocs.search/document) - The created document.

### toString() {#toString--}
```
public String toString()
```


Gibt einen  java.lang.String  zurück, der das aktuelle  Document  darstellt.


**Returns:**
java.lang.String - Ein  java.lang.String  der das aktuelle  Document  darstellt.

