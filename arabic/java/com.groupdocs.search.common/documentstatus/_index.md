---
title: "DocumentStatus"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يمثل حالة معالجة المستند."
type: docs
weight: 40
url: /ar/java/com.groupdocs.search.common/documentstatus/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum DocumentStatus extends Enum<DocumentStatus>
```

يمثل حالة معالجة المستند.

## الحقول

| حقل | الوصف |
| --- | --- |
|  | [SuccessfullyProcessed](#SuccessfullyProcessed) | تم فهرسة المستند بنجاح. |
|
|  | [Skipped](#Skipped) | تم تخطي المستند. |
|
|  | [ProcessedWithError](#ProcessedWithError) | حدث خطأ أثناء فهرسة المستند. |
|
## طرق

| طريقة | الوصف |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### SuccessfullyProcessed {#SuccessfullyProcessed}
```
public static final DocumentStatus SuccessfullyProcessed
```


تم فهرسة المستند بنجاح.


### Skipped {#Skipped}
```
public static final DocumentStatus Skipped
```


تم تخطي المستند.


### ProcessedWithError {#ProcessedWithError}
```
public static final DocumentStatus ProcessedWithError
```


حدث خطأ أثناء فهرسة المستند.


### values() {#values--}
```
public static DocumentStatus[] values()
```




**Returns:**
com.groupdocs.search.common.DocumentStatus[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static DocumentStatus valueOf(String name)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الاسم | java.lang.String |  |

**Returns:**
[DocumentStatus](../../com.groupdocs.search.common/documentstatus)
