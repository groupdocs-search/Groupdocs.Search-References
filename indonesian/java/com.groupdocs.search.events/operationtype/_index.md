---
title: "OperationType"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Mewakili tipe operasi indeks."
type: docs
weight: 23
url: /id/java/com.groupdocs.search.events/operationtype/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum OperationType extends Enum<OperationType>
```

Mewakili tipe operasi indeks.

## Fields

| Field | Deskripsi |
| --- | --- |
|  | [Indexing](#Indexing) | Menambahkan dokumen ke indeks. |
|
|  | [Updating](#Updating) | Memperbarui dokumen dalam indeks. |
|
|  | [Merging](#Merging) | Menggabungkan indeks. |
|
|  | [Optimizing](#Optimizing) | Mengoptimalkan indeks. |
|
|  | [Deleting](#Deleting) | Menghapus jalur dari indeks. |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Indexing {#Indexing}
```
public static final OperationType Indexing
```


Menambahkan dokumen ke indeks.


### Updating {#Updating}
```
public static final OperationType Updating
```


Memperbarui dokumen dalam indeks.


### Merging {#Merging}
```
public static final OperationType Merging
```


Menggabungkan indeks.


### Optimizing {#Optimizing}
```
public static final OperationType Optimizing
```


Mengoptimalkan indeks.


### Deleting {#Deleting}
```
public static final OperationType Deleting
```


Menghapus jalur dari indeks.


### values() {#values--}
```
public static OperationType[] values()
```




**Returns:**
com.groupdocs.search.events.OperationType[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static OperationType valueOf(String name)
```




**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nama | java.lang.String |  |

**Returns:**
[OperationType](../../com.groupdocs.search.events/operationtype)
