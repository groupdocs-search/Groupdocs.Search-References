---
title: "IndexStatus"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Bir dizin durumunu belirtir."
type: docs
weight: 41
url: /tr/java/com.groupdocs.search.common/indexstatus/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum IndexStatus extends Enum<IndexStatus>
```

Bir dizin durumunu belirtir.

## Alanlar

| Alan | Açıklama |
| --- | --- |
|  | [Ready](#Ready) | Dizin serbest ve değişiklik yapmaya hazır. |
|
|  | [Failed](#Failed) | Bir hata nedeniyle dizinin yeniden yüklenmesi gerekiyor. |
|
|  | [Indexing](#Indexing) | Dizin bir indeksleme işlemi gerçekleştirir. |
|
|  | [Updating](#Updating) | Dizin bir güncelleme işlemi gerçekleştirir. |
|
|  | [Merging](#Merging) | Dizin bir birleştirme işlemi gerçekleştirir. |
|
|  | [Optimizing](#Optimizing) | Dizin bir optimizasyon işlemi gerçekleştirir. |
|
|  | [Deleting](#Deleting) | Dizin bir silme işlemi gerçekleştirir. |
|
|  | [Renaming](#Renaming) | Dizin bir yeniden adlandırma işlemi gerçekleştirir. |
|
|  | [ChangingAttributes](#ChangingAttributes) | Dizin öznitelikleri değiştirir. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Ready {#Ready}
```
public static final IndexStatus Ready
```


Dizin serbest ve değişiklik yapmaya hazır.


### Failed {#Failed}
```
public static final IndexStatus Failed
```


Bir hata nedeniyle dizinin yeniden yüklenmesi gerekiyor.


### Indexing {#Indexing}
```
public static final IndexStatus Indexing
```


Dizin bir indeksleme işlemi gerçekleştirir.


### Updating {#Updating}
```
public static final IndexStatus Updating
```


Dizin bir güncelleme işlemi gerçekleştirir.


### Merging {#Merging}
```
public static final IndexStatus Merging
```


Dizin bir birleştirme işlemi gerçekleştirir.


### Optimizing {#Optimizing}
```
public static final IndexStatus Optimizing
```


Dizin bir optimizasyon işlemi gerçekleştirir.


### Deleting {#Deleting}
```
public static final IndexStatus Deleting
```


Dizin bir silme işlemi gerçekleştirir.


### Renaming {#Renaming}
```
public static final IndexStatus Renaming
```


Dizin bir yeniden adlandırma işlemi gerçekleştirir.


### ChangingAttributes {#ChangingAttributes}
```
public static final IndexStatus ChangingAttributes
```


Dizin öznitelikleri değiştirir.


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
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ad | java.lang.String |  |

**Returns:**
[IndexStatus](../../com.groupdocs.search.common/indexstatus)
