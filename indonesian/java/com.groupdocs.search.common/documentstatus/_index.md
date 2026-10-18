---
title: "DocumentStatus"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Mewakili status pemrosesan dokumen."
type: docs
weight: 40
url: /id/java/com.groupdocs.search.common/documentstatus/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum DocumentStatus extends Enum<DocumentStatus>
```

Mewakili status pemrosesan dokumen.

## Fields

| Field | Deskripsi |
| --- | --- |
|  | [SuccessfullyProcessed](#SuccessfullyProcessed) | Dokumen berhasil diindeks. |
|
|  | [Skipped](#Skipped) | Dokumen dilewati. |
|
|  | [ProcessedWithError](#ProcessedWithError) | Terjadi kesalahan selama pengindeksan dokumen. |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### SuccessfullyProcessed {#SuccessfullyProcessed}
```
public static final DocumentStatus SuccessfullyProcessed
```


Dokumen berhasil diindeks.


### Skipped {#Skipped}
```
public static final DocumentStatus Skipped
```


Dokumen dilewati.


### ProcessedWithError {#ProcessedWithError}
```
public static final DocumentStatus ProcessedWithError
```


Terjadi kesalahan selama pengindeksan dokumen.


### values() {#values--}
```
public static DocumentStatus[] values()
```




**Returns:**
com.groupdocs.search.common.DocumentStatus[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static DocumentStatus valueOf(String name)
```




**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nama | java.lang.String |  |

**Returns:**
[DocumentStatus](../../com.groupdocs.search.common/documentstatus)
