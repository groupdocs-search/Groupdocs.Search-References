---
title: "VersionUpdateResult"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Mewakili hasil operasi pembaruan versi indeks."
type: docs
weight: 42
url: /id/java/com.groupdocs.search.common/versionupdateresult/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum VersionUpdateResult extends Enum<VersionUpdateResult>
```

Mewakili hasil operasi pembaruan versi indeks.

## Fields

| Field | Deskripsi |
| --- | --- |
|  | [Updated](#Updated) | Versi indeks diperbarui. |
|
|  | [AlreadyUpToDate](#AlreadyUpToDate) | Versi indeks sudah terbaru. |
|
|  | [Unsupported](#Unsupported) | Versi indeks tidak didukung atau direktori tidak berisi data indeks yang valid. |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Updated {#Updated}
```
public static final VersionUpdateResult Updated
```


Versi indeks diperbarui.


### AlreadyUpToDate {#AlreadyUpToDate}
```
public static final VersionUpdateResult AlreadyUpToDate
```


Versi indeks sudah terbaru.


### Unsupported {#Unsupported}
```
public static final VersionUpdateResult Unsupported
```


Versi indeks tidak didukung atau direktori tidak berisi data indeks yang valid.


### values() {#values--}
```
public static VersionUpdateResult[] values()
```




**Returns:**
com.groupdocs.search.common.VersionUpdateResult[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static VersionUpdateResult valueOf(String name)
```




**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nama | java.lang.String |  |

**Returns:**
[VersionUpdateResult](../../com.groupdocs.search.common/versionupdateresult)
