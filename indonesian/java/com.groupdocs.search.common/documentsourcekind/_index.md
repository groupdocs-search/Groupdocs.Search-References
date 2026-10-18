---
title: "DocumentSourceKind"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Mendefinisikan jenis-jenis sumber dokumen."
type: docs
weight: 39
url: /id/java/com.groupdocs.search.common/documentsourcekind/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum DocumentSourceKind extends Enum<DocumentSourceKind>
```

Mendefinisikan jenis-jenis sumber dokumen.

## Fields

| Field | Deskripsi |
| --- | --- |
|  | [File](#File) | Sumber dokumen file. |
|
|  | [Stream](#Stream) | Sumber dokumen aliran. |
|
|  | [Structure](#Structure) | Sumber dokumen struktur. |
|
|  | [ExtractedData](#ExtractedData) | Sumber dokumen dari data yang sebelumnya diekstrak. |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### File {#File}
```
public static final DocumentSourceKind File
```


Sumber dokumen file.


### Stream {#Stream}
```
public static final DocumentSourceKind Stream
```


Sumber dokumen aliran.


### Structure {#Structure}
```
public static final DocumentSourceKind Structure
```


Sumber dokumen struktur.


### ExtractedData {#ExtractedData}
```
public static final DocumentSourceKind ExtractedData
```


Sumber dokumen dari data yang sebelumnya diekstrak.


### values() {#values--}
```
public static DocumentSourceKind[] values()
```




**Returns:**
com.groupdocs.search.common.DocumentSourceKind[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static DocumentSourceKind valueOf(String name)
```




**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nama | java.lang.String |  |

**Returns:**
[DocumentSourceKind](../../com.groupdocs.search.common/documentsourcekind)
