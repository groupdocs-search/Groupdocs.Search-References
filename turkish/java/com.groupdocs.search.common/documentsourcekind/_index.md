---
title: "DocumentSourceKind"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Belge kaynaklarının türlerini tanımlar."
type: docs
weight: 39
url: /tr/java/com.groupdocs.search.common/documentsourcekind/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum DocumentSourceKind extends Enum<DocumentSourceKind>
```

Belge kaynaklarının türlerini tanımlar.

## Alanlar

| Alan | Açıklama |
| --- | --- |
|  | [File](#File) | Dosya belge kaynağı. |
|
|  | [Stream](#Stream) | Akış belge kaynağı. |
|
|  | [Structure](#Structure) | Yapı belge kaynağı. |
|
|  | [ExtractedData](#ExtractedData) | Daha önce çıkarılmış verilerin belge kaynağı. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### File {#File}
```
public static final DocumentSourceKind File
```


Dosya belge kaynağı.


### Stream {#Stream}
```
public static final DocumentSourceKind Stream
```


Akış belge kaynağı.


### Structure {#Structure}
```
public static final DocumentSourceKind Structure
```


Yapı belge kaynağı.


### ExtractedData {#ExtractedData}
```
public static final DocumentSourceKind ExtractedData
```


Daha önce çıkarılmış verilerin belge kaynağı.


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
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ad | java.lang.String |  |

**Returns:**
[DocumentSourceKind](../../com.groupdocs.search.common/documentsourcekind)
