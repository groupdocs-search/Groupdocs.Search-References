---
title: "DeleteResult"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Mewakili hasil operasi penghapusan file atau folder terindeks dari indeks."
type: docs
weight: 10
url: /id/java/com.groupdocs.search.results/deleteresult/
---
**Inheritance:**
java.lang.Object
```
public class DeleteResult
```

Mewakili hasil operasi penghapusan file atau folder terindeks dari indeks.


**Learn more**

* [Delete indexed paths](../https://docs.groupdocs.com/display/searchjava/Delete+indexed+paths)

## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getItemResults()](#getItemResults--) | Mengembalikan hasil penghapusan setiap jalur. |
|
|  | [getTotalCount()](#getTotalCount--) | Mengembalikan total jumlah jalur yang akan dihapus. |
|
|  | [getSuccessCount()](#getSuccessCount--) | Mengembalikan jumlah jalur yang berhasil dihapus. |
|
|  | [getFailedCount()](#getFailedCount--) | Mengembalikan jumlah jalur yang tidak dihapus karena kesalahan. |
|
|  | [getErrors()](#getErrors--) | Mengembalikan deskripsi kesalahan penghapusan. |
|
### getItemResults() {#getItemResults--}
```
public final PathDeleteResult[] getItemResults()
```


Mengembalikan hasil penghapusan setiap jalur.


**Returns:**
com.groupdocs.search.results.PathDeleteResult[] - Hasil penghapusan setiap jalur.

### getTotalCount() {#getTotalCount--}
```
public final int getTotalCount()
```


Mengembalikan total jumlah jalur yang akan dihapus.


**Returns:**
int - Total jumlah jalur yang akan dihapus.

### getSuccessCount() {#getSuccessCount--}
```
public final int getSuccessCount()
```


Mengembalikan jumlah jalur yang berhasil dihapus.


**Returns:**
int - Jumlah jalur yang berhasil dihapus.

### getFailedCount() {#getFailedCount--}
```
public final int getFailedCount()
```


Mengembalikan jumlah jalur yang tidak dihapus karena kesalahan.


**Returns:**
int - Jumlah jalur yang tidak terhapus karena kesalahan.

### getErrors() {#getErrors--}
```
public final String[] getErrors()
```


Mengembalikan deskripsi kesalahan penghapusan.


**Returns:**
java.lang.String[] - Deskripsi kesalahan penghapusan.

