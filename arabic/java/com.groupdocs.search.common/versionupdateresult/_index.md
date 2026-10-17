---
title: "VersionUpdateResult"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يمثل نتيجة عملية تحديث نسخة الفهرس."
type: docs
weight: 42
url: /ar/java/com.groupdocs.search.common/versionupdateresult/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum VersionUpdateResult extends Enum<VersionUpdateResult>
```

يمثل نتيجة عملية تحديث نسخة الفهرس.

## الحقول

| حقل | الوصف |
| --- | --- |
|  | [Updated](#Updated) | تم تحديث إصدار الفهرس. |
|
|  | [AlreadyUpToDate](#AlreadyUpToDate) | إصدار الفهرس محدث بالفعل. |
|
|  | [Unsupported](#Unsupported) | إصدار الفهرس غير مدعوم أو الدليل لا يحتوي على بيانات فهرس صالحة. |
|
## طرق

| طريقة | الوصف |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Updated {#Updated}
```
public static final VersionUpdateResult Updated
```


تم تحديث إصدار الفهرس.


### AlreadyUpToDate {#AlreadyUpToDate}
```
public static final VersionUpdateResult AlreadyUpToDate
```


إصدار الفهرس محدث بالفعل.


### Unsupported {#Unsupported}
```
public static final VersionUpdateResult Unsupported
```


إصدار الفهرس غير مدعوم أو الدليل لا يحتوي على بيانات فهرس صالحة.


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
| معامل | نوع | الوصف |
| --- | --- | --- |
| الاسم | java.lang.String |  |

**Returns:**
[VersionUpdateResult](../../com.groupdocs.search.common/versionupdateresult)
