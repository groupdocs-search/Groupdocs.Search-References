---
title: "IndexInfo"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Berisi informasi dasar tentang Indeks."
type: docs
weight: 24
url: /id/java/com.groupdocs.search.common/indexinfo/
---
**Inheritance:**
java.lang.Object
```
public abstract class IndexInfo
```

Berisi informasi dasar tentang Indeks.

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [IndexInfo()](#IndexInfo--) |  |
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getIndexId()](#getIndexId--) | Mendapatkan pengidentifikasi unik indeks. |
|
|  | [getIndexFolder()](#getIndexFolder--) | Mendapatkan nama folder lengkap tempat indeks berada. |
|
|  | [getIndexStatus()](#getIndexStatus--) | Mendapatkan status indeks. |
|
|  | [getVersion()](#getVersion--) | Mendapatkan versi indeks. |
|
|  | [getSegmentCount()](#getSegmentCount--) | Mendapatkan jumlah segmen indeks. |
|
|  | [getTermCount()](#getTermCount--) | Mendapatkan jumlah kata dalam indeks. |
|
### IndexInfo() {#IndexInfo--}
```
public IndexInfo()
```


### getIndexId() {#getIndexId--}
```
public abstract UUID getIndexId()
```


Mendapatkan pengidentifikasi unik indeks.


**Returns:**
java.util.UUID - Pengidentifikasi unik indeks.

### getIndexFolder() {#getIndexFolder--}
```
public abstract String getIndexFolder()
```


Mendapatkan nama folder lengkap tempat indeks berada.


**Returns:**
java.lang.String - Nama folder lengkap tempat indeks berada.

### getIndexStatus() {#getIndexStatus--}
```
public abstract IndexStatus getIndexStatus()
```


Mendapatkan status indeks.


**Returns:**
[IndexStatus](../../com.groupdocs.search.common/indexstatus) - The index status.

### getVersion() {#getVersion--}
```
public abstract String getVersion()
```


Mendapatkan versi indeks.


**Returns:**
java.lang.String - Versi indeks.

### getSegmentCount() {#getSegmentCount--}
```
public abstract int getSegmentCount()
```


Mendapatkan jumlah segmen indeks.


**Returns:**
int - Jumlah segmen indeks.

### getTermCount() {#getTermCount--}
```
public abstract int getTermCount()
```


Mendapatkan jumlah kata dalam indeks.


**Returns:**
int - Jumlah kata dalam indeks.

