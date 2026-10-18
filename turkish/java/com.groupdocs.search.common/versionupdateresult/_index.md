---
title: "VersionUpdateResult"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Bir dizin sürüm güncelleme işleminin sonucunu temsil eder."
type: docs
weight: 42
url: /tr/java/com.groupdocs.search.common/versionupdateresult/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum VersionUpdateResult extends Enum<VersionUpdateResult>
```

Bir dizin sürüm güncelleme işleminin sonucunu temsil eder.

## Alanlar

| Alan | Açıklama |
| --- | --- |
|  | [Updated](#Updated) | Dizin sürümü güncellendi. |
|
|  | [AlreadyUpToDate](#AlreadyUpToDate) | Dizin sürümü zaten güncel. |
|
|  | [Unsupported](#Unsupported) | Dizin sürümü desteklenmiyor veya dizin geçerli indeks verileri içermiyor. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Updated {#Updated}
```
public static final VersionUpdateResult Updated
```


Dizin sürümü güncellendi.


### AlreadyUpToDate {#AlreadyUpToDate}
```
public static final VersionUpdateResult AlreadyUpToDate
```


Dizin sürümü zaten güncel.


### Unsupported {#Unsupported}
```
public static final VersionUpdateResult Unsupported
```


Dizin sürümü desteklenmiyor veya dizin geçerli indeks verileri içermiyor.


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
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ad | java.lang.String |  |

**Returns:**
[VersionUpdateResult](../../com.groupdocs.search.common/versionupdateresult)
