---
title: "DocumentInfo"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Stellt einen Deskriptor für ein indiziertes Dokument dar."
type: docs
weight: 11
url: /de/java/com.groupdocs.search.results/documentinfo/
---
**Inheritance:**
java.lang.Object
```
public abstract class DocumentInfo
```

Stellt einen Deskriptor für ein indiziertes Dokument dar.


**Learn more**

* [Search results](../https://docs.groupdocs.com/display/searchjava/Search+results)
* [Getting indexed documents](../https://docs.groupdocs.com/display/searchjava/Getting+indexed+documents)

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [DocumentInfo()](#DocumentInfo--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [toString()](#toString--) | Gibt einen  System.String  zurück, der das aktuelle  DocumentInfo  darstellt. |
|
|  | [getFilePath()](#getFilePath--) | Ermittelt den Dateipfad für die Indizierung aus einer Datei oder den Dokumentenschlüssel für die Indizierung aus einem Stream oder einer Struktur. |
|
|  | [getFileType()](#getFileType--) | Ermittelt den Dateityp. |
|
|  | [getFormatFamily()](#getFormatFamily--) | Liefert die Dokumentformatfamilie. |
|
|  | [getInnerPath()](#getInnerPath--) | Ermittelt den inneren Pfad für das Container-Dokumenten-Element. |
|
|  | [getInnerPathParts()](#getInnerPathParts--) | Ermittelt die inneren Pfadteile für das Container-Dokumenten-Element. |
|
|  | [getDocumentSourceKind()](#getDocumentSourceKind--) | Liefert die Art der Dokumentquelle. |
|
|  | [getIndexedWithError()](#getIndexedWithError--) | Ermittelt den Indikator für einen Indexierungsfehler. |
|
|  | [serialize()](#serialize--) | Serialisiert die aktuelle Instanz in ein Byte-Array. |
|
|  | [deserialize(byte[] array)](#deserialize-byte---) | Deserialisiert eine Instanz aus einem Byte-Array. |
|
### DocumentInfo() {#DocumentInfo--}
```
public DocumentInfo()
```


### toString() {#toString--}
```
public abstract String toString()
```


Gibt einen  System.String  zurück, der das aktuelle  DocumentInfo  darstellt.


**Returns:**
java.lang.String - Ein  System.String  der das aktuelle  DocumentInfo  darstellt.

### getFilePath() {#getFilePath--}
```
public abstract String getFilePath()
```


Ermittelt den Dateipfad für die Indizierung aus einer Datei oder den Dokumentenschlüssel für die Indizierung aus einem Stream oder einer Struktur.


**Returns:**
java.lang.String - Der Dateipfad oder Dokumentenschlüssel.

### getFileType() {#getFileType--}
```
public abstract FileType getFileType()
```


Ermittelt den Dateityp.


**Returns:**
[FileType](../../com.groupdocs.search.results/filetype) - The file type.

### getFormatFamily() {#getFormatFamily--}
```
public abstract FormatFamily getFormatFamily()
```


Liefert die Dokumentformatfamilie.


**Returns:**
[FormatFamily](../../com.groupdocs.search.results/formatfamily) - The document format family.

### getInnerPath() {#getInnerPath--}
```
public abstract String getInnerPath()
```


Ermittelt den inneren Pfad für das Container-Dokumenten-Element.


**Returns:**
java.lang.String - Der innere Pfad.

### getInnerPathParts() {#getInnerPathParts--}
```
public abstract String[] getInnerPathParts()
```


Ermittelt die inneren Pfadteile für das Container-Dokumenten-Element.


**Returns:**
java.lang.String[] - Die inneren Pfadteile.

### getDocumentSourceKind() {#getDocumentSourceKind--}
```
public abstract DocumentSourceKind getDocumentSourceKind()
```


Liefert die Art der Dokumentquelle.


**Returns:**
[DocumentSourceKind](../../com.groupdocs.search.common/documentsourcekind) - The document source kind.

### getIndexedWithError() {#getIndexedWithError--}
```
public abstract boolean getIndexedWithError()
```


Ermittelt den Indikator für einen Indexierungsfehler.


**Returns:**
boolean - Der Indikator für einen Indexierungsfehler.

### serialize() {#serialize--}
```
public abstract byte[] serialize()
```


Serialisiert die aktuelle Instanz in ein Byte-Array.


**Returns:**
byte[] – Ein Byte-Array, das die aktuelle Instanz darstellt.

### deserialize(byte[] array) {#deserialize-byte---}
```
public static DocumentInfo deserialize(byte[] array)
```


Deserialisiert eine Instanz aus einem Byte-Array.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Array | byte[] | Ein Byte-Array, aus dem deserialisiert werden soll. |
|

**Returns:**
[DocumentInfo](../../com.groupdocs.search.results/documentinfo) - An instance deserialized from a byte array.

