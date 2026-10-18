---
title: "OperationType"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Bir indeks işlemi türünü temsil eder."
type: docs
weight: 23
url: /tr/java/com.groupdocs.search.events/operationtype/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum OperationType extends Enum<OperationType>
```

Bir indeks işlemi türünü temsil eder.

## Alanlar

| Alan | Açıklama |
| --- | --- |
|  | [Indexing](#Indexing) | Bir indekse belgeler ekleniyor. |
|
|  | [Updating](#Updating) | Bir indekste belgeler güncelleniyor. |
|
|  | [Merging](#Merging) | İndeksler birleştiriliyor. |
|
|  | [Optimizing](#Optimizing) | Bir indeks optimize ediliyor. |
|
|  | [Deleting](#Deleting) | Bir indeksten yollar siliniyor. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Indexing {#Indexing}
```
public static final OperationType Indexing
```


Bir indekse belgeler ekleniyor.


### Updating {#Updating}
```
public static final OperationType Updating
```


Bir indekste belgeler güncelleniyor.


### Merging {#Merging}
```
public static final OperationType Merging
```


İndeksler birleştiriliyor.


### Optimizing {#Optimizing}
```
public static final OperationType Optimizing
```


Bir indeks optimize ediliyor.


### Deleting {#Deleting}
```
public static final OperationType Deleting
```


Bir indeksten yollar siliniyor.


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
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ad | java.lang.String |  |

**Returns:**
[OperationType](../../com.groupdocs.search.events/operationtype)
