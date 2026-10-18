---
title: "DocumentInfo"
second_title: "GroupDocs.Search för Java API-referens"
description: "Representerar en beskrivning för ett indexerat dokument."
type: docs
weight: 11
url: /sv/java/com.groupdocs.search.results/documentinfo/
---
**Inheritance:**
java.lang.Object
```
public abstract class DocumentInfo
```

Representerar en beskrivning för ett indexerat dokument.


**Learn more**

* [Search results](../https://docs.groupdocs.com/display/searchjava/Search+results)
* [Getting indexed documents](../https://docs.groupdocs.com/display/searchjava/Getting+indexed+documents)

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [DocumentInfo()](#DocumentInfo--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [toString()](#toString--) | Returnerar en  System.String  som representerar den aktuella  DocumentInfo . |
|
|  | [getFilePath()](#getFilePath--) | Hämtar filsökvägen för indexerad från fil eller dokumentnyckeln för indexerad från ström eller struktur. |
|
|  | [getFileType()](#getFileType--) | Hämtar filtypen. |
|
|  | [getFormatFamily()](#getFormatFamily--) | Hämtar dokumentformatfamiljen. |
|
|  | [getInnerPath()](#getInnerPath--) | Hämtar den interna sökvägen för containerdokumentet. |
|
|  | [getInnerPathParts()](#getInnerPathParts--) | Hämtar de interna sökvägsdelarna för containerdokumentet. |
|
|  | [getDocumentSourceKind()](#getDocumentSourceKind--) | Hämtar dokumentkällans typ. |
|
|  | [getIndexedWithError()](#getIndexedWithError--) | Hämtar indikatorn för indexeringsfel. |
|
|  | [serialize()](#serialize--) | Serialiserar den aktuella instansen till en bytearray. |
|
|  | [deserialize(byte[] array)](#deserialize-byte---) | Deserialiserar en instans från en bytearray. |
|
### DocumentInfo() {#DocumentInfo--}
```
public DocumentInfo()
```


### toString() {#toString--}
```
public abstract String toString()
```


Returnerar en  System.String  som representerar den aktuella  DocumentInfo .


**Returns:**
java.lang.String - En  System.String  som representerar den aktuella  DocumentInfo .

### getFilePath() {#getFilePath--}
```
public abstract String getFilePath()
```


Hämtar filsökvägen för indexerad från fil eller dokumentnyckeln för indexerad från ström eller struktur.


**Returns:**
java.lang.String - Filsökvägen eller dokumentnyckeln.

### getFileType() {#getFileType--}
```
public abstract FileType getFileType()
```


Hämtar filtypen.


**Returns:**
[FileType](../../com.groupdocs.search.results/filetype) - The file type.

### getFormatFamily() {#getFormatFamily--}
```
public abstract FormatFamily getFormatFamily()
```


Hämtar dokumentformatfamiljen.


**Returns:**
[FormatFamily](../../com.groupdocs.search.results/formatfamily) - The document format family.

### getInnerPath() {#getInnerPath--}
```
public abstract String getInnerPath()
```


Hämtar den interna sökvägen för containerdokumentet.


**Returns:**
java.lang.String - Den interna sökvägen.

### getInnerPathParts() {#getInnerPathParts--}
```
public abstract String[] getInnerPathParts()
```


Hämtar de interna sökvägsdelarna för containerdokumentet.


**Returns:**
java.lang.String[] - De interna sökvägsdelarna.

### getDocumentSourceKind() {#getDocumentSourceKind--}
```
public abstract DocumentSourceKind getDocumentSourceKind()
```


Hämtar dokumentkällans typ.


**Returns:**
[DocumentSourceKind](../../com.groupdocs.search.common/documentsourcekind) - The document source kind.

### getIndexedWithError() {#getIndexedWithError--}
```
public abstract boolean getIndexedWithError()
```


Hämtar indikatorn för indexeringsfel.


**Returns:**
boolean - Indikatorn för indexeringsfel.

### serialize() {#serialize--}
```
public abstract byte[] serialize()
```


Serialiserar den aktuella instansen till en bytearray.


**Returns:**
byte[] - En bytearray som representerar den aktuella instansen.

### deserialize(byte[] array) {#deserialize-byte---}
```
public static DocumentInfo deserialize(byte[] array)
```


Deserialiserar en instans från en bytearray.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | array | byte[] | En bytearray att deserialisera från. |
|

**Returns:**
[DocumentInfo](../../com.groupdocs.search.results/documentinfo) - An instance deserialized from a byte array.

