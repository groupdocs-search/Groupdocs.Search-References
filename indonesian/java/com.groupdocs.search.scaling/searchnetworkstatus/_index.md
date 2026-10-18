---
title: "SearchNetworkStatus"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Menentukan status jaringan pencarian."
type: docs
weight: 13
url: /id/java/com.groupdocs.search.scaling/searchnetworkstatus/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum SearchNetworkStatus extends Enum<SearchNetworkStatus>
```

Menentukan status jaringan pencarian.

## Fields

| Field | Deskripsi |
| --- | --- |
|  | [Ready](#Ready) | Jaringan pencarian bebas dan siap untuk perubahan. |
|
|  | [Configuring](#Configuring) | Jaringan pencarian melakukan operasi konfigurasi. |
|
|  | [Indexing](#Indexing) | Jaringan pencarian melakukan operasi pengindeksan. |
|
|  | [Optimizing](#Optimizing) | Jaringan pencarian melakukan operasi optimasi. |
|
|  | [Deleting](#Deleting) | Jaringan pencarian melakukan operasi penghapusan. |
|
|  | [ChangingAttributes](#ChangingAttributes) | Jaringan pencarian mengubah atribut. |
|
|  | [Synchronizing](#Synchronizing) | Jaringan pencarian melakukan operasi sinkronisasi. |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Ready {#Ready}
```
public static final SearchNetworkStatus Ready
```


Jaringan pencarian bebas dan siap untuk perubahan.


### Configuring {#Configuring}
```
public static final SearchNetworkStatus Configuring
```


Jaringan pencarian melakukan operasi konfigurasi.


### Indexing {#Indexing}
```
public static final SearchNetworkStatus Indexing
```


Jaringan pencarian melakukan operasi pengindeksan.


### Optimizing {#Optimizing}
```
public static final SearchNetworkStatus Optimizing
```


Jaringan pencarian melakukan operasi optimasi.


### Deleting {#Deleting}
```
public static final SearchNetworkStatus Deleting
```


Jaringan pencarian melakukan operasi penghapusan.


### ChangingAttributes {#ChangingAttributes}
```
public static final SearchNetworkStatus ChangingAttributes
```


Jaringan pencarian mengubah atribut.


### Synchronizing {#Synchronizing}
```
public static final SearchNetworkStatus Synchronizing
```


Jaringan pencarian melakukan operasi sinkronisasi.


### values() {#values--}
```
public static SearchNetworkStatus[] values()
```




**Returns:**
com.groupdocs.search.scaling.SearchNetworkStatus[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static SearchNetworkStatus valueOf(String name)
```




**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nama | java.lang.String |  |

**Returns:**
[SearchNetworkStatus](../../com.groupdocs.search.scaling/searchnetworkstatus)
