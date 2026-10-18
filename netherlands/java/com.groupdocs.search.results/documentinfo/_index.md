---
title: "DocumentInfo"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Stelt een descriptor voor een geïndexeerd document voor."
type: docs
weight: 11
url: /nl/java/com.groupdocs.search.results/documentinfo/
---
**Inheritance:**
java.lang.Object
```
public abstract class DocumentInfo
```

Stelt een descriptor voor een geïndexeerd document voor.


**Learn more**

* [Search results](../https://docs.groupdocs.com/display/searchjava/Search+results)
* [Getting indexed documents](../https://docs.groupdocs.com/display/searchjava/Getting+indexed+documents)

## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [DocumentInfo()](#DocumentInfo--) |  |
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [toString()](#toString--) | Retourneert een  System.String  die de huidige  DocumentInfo  vertegenwoordigt. |
|
|  | [getFilePath()](#getFilePath--) | Haalt het bestandspad op voor geïndexeerd vanuit bestand of de documentensleutel voor geïndexeerd vanuit stream of structuur. |
|
|  | [getFileType()](#getFileType--) | Haalt het bestandstype op. |
|
|  | [getFormatFamily()](#getFormatFamily--) | Haalt de documentformaatfamilie op. |
|
|  | [getInnerPath()](#getInnerPath--) | Haalt het interne pad op voor het containerdocumentitem. |
|
|  | [getInnerPathParts()](#getInnerPathParts--) | Haalt de interne padonderdelen op voor het containerdocumentitem. |
|
|  | [getDocumentSourceKind()](#getDocumentSourceKind--) | Haalt het type documentbron op. |
|
|  | [getIndexedWithError()](#getIndexedWithError--) | Haalt de indicator van indexeringsfout op. |
|
|  | [serialize()](#serialize--) | Serialiseert de huidige instantie naar een byte-array. |
|
|  | [deserialize(byte[] array)](#deserialize-byte---) | Deserialiseert een instantie vanuit een byte-array. |
|
### DocumentInfo() {#DocumentInfo--}
```
public DocumentInfo()
```


### toString() {#toString--}
```
public abstract String toString()
```


Retourneert een  System.String  die de huidige  DocumentInfo  vertegenwoordigt.


**Returns:**
java.lang.String - Een  System.String  die de huidige  DocumentInfo  vertegenwoordigt.

### getFilePath() {#getFilePath--}
```
public abstract String getFilePath()
```


Haalt het bestandspad op voor geïndexeerd vanuit bestand of de documentensleutel voor geïndexeerd vanuit stream of structuur.


**Returns:**
java.lang.String - Het bestandspad of de documentensleutel.

### getFileType() {#getFileType--}
```
public abstract FileType getFileType()
```


Haalt het bestandstype op.


**Returns:**
[FileType](../../com.groupdocs.search.results/filetype) - The file type.

### getFormatFamily() {#getFormatFamily--}
```
public abstract FormatFamily getFormatFamily()
```


Haalt de documentformaatfamilie op.


**Returns:**
[FormatFamily](../../com.groupdocs.search.results/formatfamily) - The document format family.

### getInnerPath() {#getInnerPath--}
```
public abstract String getInnerPath()
```


Haalt het interne pad op voor het containerdocumentitem.


**Returns:**
java.lang.String - Het interne pad.

### getInnerPathParts() {#getInnerPathParts--}
```
public abstract String[] getInnerPathParts()
```


Haalt de interne padonderdelen op voor het containerdocumentitem.


**Returns:**
java.lang.String[] - De interne padonderdelen.

### getDocumentSourceKind() {#getDocumentSourceKind--}
```
public abstract DocumentSourceKind getDocumentSourceKind()
```


Haalt het type documentbron op.


**Returns:**
[DocumentSourceKind](../../com.groupdocs.search.common/documentsourcekind) - The document source kind.

### getIndexedWithError() {#getIndexedWithError--}
```
public abstract boolean getIndexedWithError()
```


Haalt de indicator van indexeringsfout op.


**Returns:**
boolean - De indicator van indexeringsfout.

### serialize() {#serialize--}
```
public abstract byte[] serialize()
```


Serialiseert de huidige instantie naar een byte-array.


**Returns:**
byte[] - Een byte-array die de huidige instantie vertegenwoordigt.

### deserialize(byte[] array) {#deserialize-byte---}
```
public static DocumentInfo deserialize(byte[] array)
```


Deserialiseert een instantie vanuit een byte-array.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | array | byte[] | Een byte-array om van te deserialiseren. |
|

**Returns:**
[DocumentInfo](../../com.groupdocs.search.results/documentinfo) - An instance deserialized from a byte array.

