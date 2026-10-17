---
title: "PathDeleteResult"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يمثل نتيجة العملية لحذف ملف أو مجلد مفهرس من الفهرس."
type: docs
weight: 18
url: /ar/java/com.groupdocs.search.results/pathdeleteresult/
---
**Inheritance:**
java.lang.Object
```
public class PathDeleteResult
```

يمثل نتيجة العملية لحذف ملف أو مجلد مفهرس من الفهرس.


**Learn more**

* [Delete indexed paths](../https://docs.groupdocs.com/display/searchjava/Delete+indexed+paths)

## طرق

| طريقة | الوصف |
| --- | --- |
|  | [isSuccess()](#isSuccess--) | يرجع مؤشر نجاح عملية الحذف. |
|
|  | [getError()](#getError--) | يرجع وصفًا لخطأ الحذف. |
|
|  | [getPath()](#getPath--) | يرجع المسار إلى الملف أو المجلد المراد حذفه. |
|
### isSuccess() {#isSuccess--}
```
public final boolean isSuccess()
```


يرجع مؤشر نجاح عملية الحذف.


**Returns:**
boolean -  true  إذا كانت عملية الحذف ناجحة؛ وإلا، يرجع  false .

### getError() {#getError--}
```
public final String getError()
```


يرجع وصفًا لخطأ الحذف.


**Returns:**
java.lang.String - وصف لخطأ الحذف.

### getPath() {#getPath--}
```
public final String getPath()
```


يرجع المسار إلى الملف أو المجلد المراد حذفه.


**Returns:**
java.lang.String - المسار إلى الملف أو المجلد المراد حذفه.

