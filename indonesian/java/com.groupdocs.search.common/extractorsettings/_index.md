---
title: "ExtractorSettings"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Berisi pengaturan untuk ekstraktor data dokumen."
type: docs
weight: 19
url: /id/java/com.groupdocs.search.common/extractorsettings/
---
**Inheritance:**
java.lang.Object
```
public abstract class ExtractorSettings
```

Berisi pengaturan untuk ekstraktor data dokumen.

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [ExtractorSettings()](#ExtractorSettings--) |  |
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getIndexType()](#getIndexType--) | Mendapatkan tipe indeks yang digunakan oleh extractor. |
|
|  | [setIndexType(IndexType value)](#setIndexType-com.groupdocs.search.options.IndexType-) | Mengatur tipe indeks yang digunakan oleh extractor. |
|
### ExtractorSettings() {#ExtractorSettings--}
```
public ExtractorSettings()
```


### getIndexType() {#getIndexType--}
```
public abstract IndexType getIndexType()
```


Mendapatkan tipe indeks yang digunakan oleh extractor. Nilai defaultnya adalah GroupDocs.Search.Options.IndexType.NormalIndex .


**Returns:**
[IndexType](../../com.groupdocs.search.options/indextype) - The index type the extractor is used for.

### setIndexType(IndexType value) {#setIndexType-com.groupdocs.search.options.IndexType-}
```
public abstract void setIndexType(IndexType value)
```


Mengatur tipe indeks yang digunakan oleh extractor. Nilai defaultnya adalah GroupDocs.Search.Options.IndexType.NormalIndex .


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | value | [IndexType](../../com.groupdocs.search.options/indextype) | Tipe indeks yang digunakan oleh extractor. |
|

