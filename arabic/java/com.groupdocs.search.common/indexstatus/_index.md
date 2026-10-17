---
title: "IndexStatus"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يحدد حالة الفهرس."
type: docs
weight: 41
url: /ar/java/com.groupdocs.search.common/indexstatus/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum IndexStatus extends Enum<IndexStatus>
```

يحدد حالة الفهرس.

## الحقول

| حقل | الوصف |
| --- | --- |
|  | [Ready](#Ready) | الفهرس خالٍ وجاهز للتغيير. |
|
|  | [Failed](#Failed) | يحتاج الفهرس إلى إعادة تحميله بسبب خطأ. |
|
|  | [Indexing](#Indexing) | يقوم الفهرس بعملية فهرسة. |
|
|  | [Updating](#Updating) | يقوم الفهرس بعملية تحديث. |
|
|  | [Merging](#Merging) | يقوم الفهرس بعملية دمج. |
|
|  | [Optimizing](#Optimizing) | يقوم الفهرس بعملية تحسين. |
|
|  | [Deleting](#Deleting) | يقوم الفهرس بعملية حذف. |
|
|  | [Renaming](#Renaming) | يقوم الفهرس بعملية إعادة تسمية. |
|
|  | [ChangingAttributes](#ChangingAttributes) | يقوم الفهرس بتغيير السمات. |
|
## طرق

| طريقة | الوصف |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Ready {#Ready}
```
public static final IndexStatus Ready
```


الفهرس خالٍ وجاهز للتغيير.


### Failed {#Failed}
```
public static final IndexStatus Failed
```


يحتاج الفهرس إلى إعادة تحميله بسبب خطأ.


### Indexing {#Indexing}
```
public static final IndexStatus Indexing
```


يقوم الفهرس بعملية فهرسة.


### Updating {#Updating}
```
public static final IndexStatus Updating
```


يقوم الفهرس بعملية تحديث.


### Merging {#Merging}
```
public static final IndexStatus Merging
```


يقوم الفهرس بعملية دمج.


### Optimizing {#Optimizing}
```
public static final IndexStatus Optimizing
```


يقوم الفهرس بعملية تحسين.


### Deleting {#Deleting}
```
public static final IndexStatus Deleting
```


يقوم الفهرس بعملية حذف.


### Renaming {#Renaming}
```
public static final IndexStatus Renaming
```


يقوم الفهرس بعملية إعادة تسمية.


### ChangingAttributes {#ChangingAttributes}
```
public static final IndexStatus ChangingAttributes
```


يقوم الفهرس بتغيير السمات.


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
| معامل | نوع | الوصف |
| --- | --- | --- |
| الاسم | java.lang.String |  |

**Returns:**
[IndexStatus](../../com.groupdocs.search.common/indexstatus)
