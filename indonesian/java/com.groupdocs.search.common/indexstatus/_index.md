---
title: "IndexStatus"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Menentukan status indeks."
type: docs
weight: 41
url: /id/java/com.groupdocs.search.common/indexstatus/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum IndexStatus extends Enum<IndexStatus>
```

Menentukan status indeks.

## Fields

| Field | Deskripsi |
| --- | --- |
|  | [Ready](#Ready) | Indeks bebas dan siap diubah. |
|
|  | [Failed](#Failed) | Indeks perlu dimuat ulang karena ada kesalahan. |
|
|  | [Indexing](#Indexing) | Indeks melakukan operasi pengindeksan. |
|
|  | [Updating](#Updating) | Indeks melakukan operasi pembaruan. |
|
|  | [Merging](#Merging) | Indeks melakukan operasi penggabungan. |
|
|  | [Optimizing](#Optimizing) | Indeks melakukan operasi optimasi. |
|
|  | [Deleting](#Deleting) | Indeks melakukan operasi penghapusan. |
|
|  | [Renaming](#Renaming) | Indeks melakukan operasi penggantian nama. |
|
|  | [ChangingAttributes](#ChangingAttributes) | Indeks mengubah atribut. |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Ready {#Ready}
```
public static final IndexStatus Ready
```


Indeks bebas dan siap diubah.


### Failed {#Failed}
```
public static final IndexStatus Failed
```


Indeks perlu dimuat ulang karena ada kesalahan.


### Indexing {#Indexing}
```
public static final IndexStatus Indexing
```


Indeks melakukan operasi pengindeksan.


### Updating {#Updating}
```
public static final IndexStatus Updating
```


Indeks melakukan operasi pembaruan.


### Merging {#Merging}
```
public static final IndexStatus Merging
```


Indeks melakukan operasi penggabungan.


### Optimizing {#Optimizing}
```
public static final IndexStatus Optimizing
```


Indeks melakukan operasi optimasi.


### Deleting {#Deleting}
```
public static final IndexStatus Deleting
```


Indeks melakukan operasi penghapusan.


### Renaming {#Renaming}
```
public static final IndexStatus Renaming
```


Indeks melakukan operasi penggantian nama.


### ChangingAttributes {#ChangingAttributes}
```
public static final IndexStatus ChangingAttributes
```


Indeks mengubah atribut.


### values() {#values--}
```
public static IndexStatus[] values()
```




**Returns:**
com.groupdocs.search.common.IndexStatus[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static IndexStatus valueOf(String name)
```




**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nama | java.lang.String |  |

**Returns:**
[IndexStatus](../../com.groupdocs.search.common/indexstatus)
