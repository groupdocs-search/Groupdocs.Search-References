---
title: "OperationType"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يمثل نوع عملية الفهرسة."
type: docs
weight: 23
url: /ar/java/com.groupdocs.search.events/operationtype/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum OperationType extends Enum<OperationType>
```

يمثل نوع عملية الفهرسة.

## الحقول

| حقل | الوصف |
| --- | --- |
|  | [Indexing](#Indexing) | إضافة مستندات إلى فهرس. |
|
|  | [Updating](#Updating) | تحديث مستندات في فهرس. |
|
|  | [Merging](#Merging) | دمج الفهارس. |
|
|  | [Optimizing](#Optimizing) | تحسين فهرس. |
|
|  | [Deleting](#Deleting) | حذف المسارات من فهرس. |
|
## طرق

| طريقة | الوصف |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Indexing {#Indexing}
```
public static final OperationType Indexing
```


إضافة مستندات إلى فهرس.


### Updating {#Updating}
```
public static final OperationType Updating
```


تحديث مستندات في فهرس.


### Merging {#Merging}
```
public static final OperationType Merging
```


دمج الفهارس.


### Optimizing {#Optimizing}
```
public static final OperationType Optimizing
```


تحسين فهرس.


### Deleting {#Deleting}
```
public static final OperationType Deleting
```


حذف المسارات من فهرس.


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
| معامل | نوع | الوصف |
| --- | --- | --- |
| الاسم | java.lang.String |  |

**Returns:**
[OperationType](../../com.groupdocs.search.events/operationtype)
