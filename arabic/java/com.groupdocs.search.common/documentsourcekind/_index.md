---
title: "DocumentSourceKind"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يعرف أنواع مصادر المستندات."
type: docs
weight: 39
url: /ar/java/com.groupdocs.search.common/documentsourcekind/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum DocumentSourceKind extends Enum<DocumentSourceKind>
```

يعرف أنواع مصادر المستندات.

## الحقول

| حقل | الوصف |
| --- | --- |
|  | [File](#File) | مصدر المستند من الملف. |
|
|  | [Stream](#Stream) | مصدر المستند من التدفق. |
|
|  | [Structure](#Structure) | مصدر المستند الهيكلي. |
|
|  | [ExtractedData](#ExtractedData) | مصدر المستند للبيانات المستخرجة مسبقًا. |
|
## طرق

| طريقة | الوصف |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### File {#File}
```
public static final DocumentSourceKind File
```


مصدر المستند من الملف.


### Stream {#Stream}
```
public static final DocumentSourceKind Stream
```


مصدر المستند من التدفق.


### Structure {#Structure}
```
public static final DocumentSourceKind Structure
```


مصدر المستند الهيكلي.


### ExtractedData {#ExtractedData}
```
public static final DocumentSourceKind ExtractedData
```


مصدر المستند للبيانات المستخرجة مسبقًا.


### values() {#values--}
```
public static DocumentSourceKind[] values()
```




**Returns:**
com.groupdocs.search.common.DocumentSourceKind[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static DocumentSourceKind valueOf(String name)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الاسم | java.lang.String |  |

**Returns:**
[DocumentSourceKind](../../com.groupdocs.search.common/documentsourcekind)
