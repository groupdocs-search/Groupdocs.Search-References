---
title: "IndexType"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Menentukan tipe indeks."
type: docs
weight: 49
url: /id/java/com.groupdocs.search.options/indextype/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum IndexType extends Enum<IndexType>
```

Menentukan tipe indeks.


**Learn more**

* [Search index settings](../https://docs.groupdocs.com/display/searchjava/Search+index+settings)

## Fields

| Field | Deskripsi |
| --- | --- |
|  | [NormalIndex](#NormalIndex) | Indeks normal dengan metadata dokumen dan konten dokumen yang mendukung semua fitur pencarian. |
|
|  | [MetadataIndex](#MetadataIndex) | Indeks yang hanya berisi metadata dokumen, tanpa konten. |
|
|  | [CompactIndex](#CompactIndex) | Jenis indeks yang memakan ruang disk jauh lebih sedikit tetapi tidak mendukung pencarian frasa dan pencarian rentang tanggal. |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### NormalIndex {#NormalIndex}
```
public static final IndexType NormalIndex
```


Indeks normal dengan metadata dokumen dan konten dokumen yang mendukung semua fitur pencarian.


### MetadataIndex {#MetadataIndex}
```
public static final IndexType MetadataIndex
```


Indeks yang hanya berisi metadata dokumen, tanpa konten.


### CompactIndex {#CompactIndex}
```
public static final IndexType CompactIndex
```


Jenis indeks yang memakan ruang disk jauh lebih sedikit tetapi tidak mendukung pencarian frasa dan pencarian rentang tanggal.


### values() {#values--}
```
public static IndexType[] values()
```




**Returns:**
com.groupdocs.search.options.IndexType[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static IndexType valueOf(String name)
```




**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nama | java.lang.String |  |

**Returns:**
[IndexType](../../com.groupdocs.search.options/indextype)
