---
title: "ExtractedItemInfo"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Mewakili informasi item wadah."
type: docs
weight: 18
url: /id/java/com.groupdocs.search.common/extractediteminfo/
---
**Inheritance:**
java.lang.Object
```
public class ExtractedItemInfo
```

Mewakili informasi item wadah.


**Learn more**

* [Custom text extractors](../https://docs.groupdocs.com/display/searchjava/Custom+text+extractors)

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [ExtractedItemInfo(FormatFamily formatFamily, DocumentField[] fields, String itemInfo, String innerPath)](#ExtractedItemInfo-com.groupdocs.search.results.FormatFamily-com.groupdocs.search.common.DocumentField---java.lang.String-java.lang.String-) | Menginisialisasi instance baru dari kelas ExtractedItemInfo. |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getFormatFamily()](#getFormatFamily--) | Mengambil tipe dokumen. |
|
|  | [getFields()](#getFields--) | Mengambil bidang yang diekstrak. |
|
|  | [getItemInfo()](#getItemInfo--) | Mendapatkan informasi item. |
|
|  | [getInnerPath()](#getInnerPath--) | Mendapatkan jalur dalam. |
|
### ExtractedItemInfo(FormatFamily formatFamily, DocumentField[] fields, String itemInfo, String innerPath) {#ExtractedItemInfo-com.groupdocs.search.results.FormatFamily-com.groupdocs.search.common.DocumentField---java.lang.String-java.lang.String-}
```
public ExtractedItemInfo(FormatFamily formatFamily, DocumentField[] fields, String itemInfo, String innerPath)
```


Menginisialisasi instance baru dari kelas ExtractedItemInfo.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | formatFamily | [FormatFamily](../../com.groupdocs.search.results/formatfamily) | Keluarga format dokumen. |
|
|  | fields | [DocumentField\[\]](../../com.groupdocs.search.common/documentfield) | Bidang yang diekstrak. |
|
|  | itemInfo | java.lang.String | Informasi item. |
|
|  | innerPath | java.lang.String | Jalur ke item dalam kontainer. |
|

### getFormatFamily() {#getFormatFamily--}
```
public final FormatFamily getFormatFamily()
```


Mengambil tipe dokumen.


**Returns:**
[FormatFamily](../../com.groupdocs.search.results/formatfamily) - The document type.

### getFields() {#getFields--}
```
public final DocumentField[] getFields()
```


Mengambil bidang yang diekstrak.


**Returns:**
com.groupdocs.search.common.DocumentField[] - Bidang yang diekstrak.

### getItemInfo() {#getItemInfo--}
```
public final String getItemInfo()
```


Mendapatkan informasi item.


**Returns:**
java.lang.String - Informasi item.

### getInnerPath() {#getInnerPath--}
```
public final String getInnerPath()
```


Mendapatkan jalur dalam.


**Returns:**
java.lang.String - Jalur dalam.

