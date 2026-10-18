---
title: "DocumentInfo"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Mewakili deskripsi untuk dokumen terindeks."
type: docs
weight: 11
url: /id/java/com.groupdocs.search.results/documentinfo/
---
**Inheritance:**
java.lang.Object
```
public abstract class DocumentInfo
```

Mewakili deskripsi untuk dokumen terindeks.


**Learn more**

* [Search results](../https://docs.groupdocs.com/display/searchjava/Search+results)
* [Getting indexed documents](../https://docs.groupdocs.com/display/searchjava/Getting+indexed+documents)

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [DocumentInfo()](#DocumentInfo--) |  |
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [toString()](#toString--) | Mengembalikan sebuah  System.String  yang mewakili  DocumentInfo  saat ini. |
|
|  | [getFilePath()](#getFilePath--) | Mendapatkan jalur file untuk diindeks dari file atau kunci dokumen untuk diindeks dari aliran atau struktur. |
|
|  | [getFileType()](#getFileType--) | Mendapatkan tipe file. |
|
|  | [getFormatFamily()](#getFormatFamily--) | Mendapatkan keluarga format dokumen. |
|
|  | [getInnerPath()](#getInnerPath--) | Mendapatkan jalur dalam untuk item dokumen kontainer. |
|
|  | [getInnerPathParts()](#getInnerPathParts--) | Mendapatkan bagian jalur dalam untuk item dokumen kontainer. |
|
|  | [getDocumentSourceKind()](#getDocumentSourceKind--) | Mendapatkan jenis sumber dokumen. |
|
|  | [getIndexedWithError()](#getIndexedWithError--) | Mendapatkan indikator kesalahan pengindeksan. |
|
|  | [serialize()](#serialize--) | Menyerialkan instance saat ini ke dalam array byte. |
|
|  | [deserialize(byte[] array)](#deserialize-byte---) | Mendeserialkan sebuah instance dari array byte. |
|
### DocumentInfo() {#DocumentInfo--}
```
public DocumentInfo()
```


### toString() {#toString--}
```
public abstract String toString()
```


Mengembalikan sebuah  System.String  yang mewakili  DocumentInfo  saat ini.


**Returns:**
java.lang.String - Sebuah  System.String  yang mewakili  DocumentInfo  saat ini.

### getFilePath() {#getFilePath--}
```
public abstract String getFilePath()
```


Mendapatkan jalur file untuk diindeks dari file atau kunci dokumen untuk diindeks dari aliran atau struktur.


**Returns:**
java.lang.String - Jalur file atau kunci dokumen.

### getFileType() {#getFileType--}
```
public abstract FileType getFileType()
```


Mendapatkan tipe file.


**Returns:**
[FileType](../../com.groupdocs.search.results/filetype) - The file type.

### getFormatFamily() {#getFormatFamily--}
```
public abstract FormatFamily getFormatFamily()
```


Mendapatkan keluarga format dokumen.


**Returns:**
[FormatFamily](../../com.groupdocs.search.results/formatfamily) - The document format family.

### getInnerPath() {#getInnerPath--}
```
public abstract String getInnerPath()
```


Mendapatkan jalur dalam untuk item dokumen kontainer.


**Returns:**
java.lang.String - Jalur dalam.

### getInnerPathParts() {#getInnerPathParts--}
```
public abstract String[] getInnerPathParts()
```


Mendapatkan bagian jalur dalam untuk item dokumen kontainer.


**Returns:**
java.lang.String[] - Bagian jalur dalam.

### getDocumentSourceKind() {#getDocumentSourceKind--}
```
public abstract DocumentSourceKind getDocumentSourceKind()
```


Mendapatkan jenis sumber dokumen.


**Returns:**
[DocumentSourceKind](../../com.groupdocs.search.common/documentsourcekind) - The document source kind.

### getIndexedWithError() {#getIndexedWithError--}
```
public abstract boolean getIndexedWithError()
```


Mendapatkan indikator kesalahan pengindeksan.


**Returns:**
boolean - Indikator kesalahan pengindeksan.

### serialize() {#serialize--}
```
public abstract byte[] serialize()
```


Menyerialkan instance saat ini ke dalam array byte.


**Returns:**
byte[] - Array byte yang mewakili instance saat ini.

### deserialize(byte[] array) {#deserialize-byte---}
```
public static DocumentInfo deserialize(byte[] array)
```


Mendeserialkan sebuah instance dari array byte.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | array | byte[] | Array byte untuk dideserialkan. |
|

**Returns:**
[DocumentInfo](../../com.groupdocs.search.results/documentinfo) - An instance deserialized from a byte array.

