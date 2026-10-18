---
title: "PathDeleteResult"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Mewakili hasil operasi menghapus file atau folder terindeks dari indeks."
type: docs
weight: 18
url: /id/java/com.groupdocs.search.results/pathdeleteresult/
---
**Inheritance:**
java.lang.Object
```
public class PathDeleteResult
```

Mewakili hasil operasi menghapus file atau folder terindeks dari indeks.


**Learn more**

* [Delete indexed paths](../https://docs.groupdocs.com/display/searchjava/Delete+indexed+paths)

## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [isSuccess()](#isSuccess--) | Mengembalikan indikator keberhasilan operasi penghapusan. |
|
|  | [getError()](#getError--) | Mengembalikan deskripsi kesalahan penghapusan. |
|
|  | [getPath()](#getPath--) | Mengembalikan jalur ke file atau folder yang akan dihapus. |
|
### isSuccess() {#isSuccess--}
```
public final boolean isSuccess()
```


Mengembalikan indikator keberhasilan operasi penghapusan.


**Returns:**
boolean -  true  jika operasi penghapusan berhasil; jika tidak, mengembalikan  false .

### getError() {#getError--}
```
public final String getError()
```


Mengembalikan deskripsi kesalahan penghapusan.


**Returns:**
java.lang.String - Deskripsi kesalahan penghapusan.

### getPath() {#getPath--}
```
public final String getPath()
```


Mengembalikan jalur ke file atau folder yang akan dihapus.


**Returns:**
java.lang.String - Jalur ke file atau folder yang akan dihapus.

