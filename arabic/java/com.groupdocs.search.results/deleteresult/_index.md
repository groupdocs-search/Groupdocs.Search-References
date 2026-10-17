---
title: "DeleteResult"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يمثل نتيجة العملية لحذف الملفات أو المجلدات المفهرسة من الفهرس."
type: docs
weight: 10
url: /ar/java/com.groupdocs.search.results/deleteresult/
---
**Inheritance:**
java.lang.Object
```
public class DeleteResult
```

يمثل نتيجة العملية لحذف الملفات أو المجلدات المفهرسة من الفهرس.


**Learn more**

* [Delete indexed paths](../https://docs.groupdocs.com/display/searchjava/Delete+indexed+paths)

## طرق

| طريقة | الوصف |
| --- | --- |
|  | [getItemResults()](#getItemResults--) | يعيد نتائج حذف كل مسار. |
|
|  | [getTotalCount()](#getTotalCount--) | يعيد العدد الإجمالي للمسارات التي سيتم حذفها. |
|
|  | [getSuccessCount()](#getSuccessCount--) | يعيد عدد المسارات التي تم حذفها بنجاح. |
|
|  | [getFailedCount()](#getFailedCount--) | يعيد عدد المسارات التي لم تُحذف بسبب الأخطاء. |
|
|  | [getErrors()](#getErrors--) | يعيد أوصاف أخطاء الحذف. |
|
### getItemResults() {#getItemResults--}
```
public final PathDeleteResult[] getItemResults()
```


يعيد نتائج حذف كل مسار.


**Returns:**
com.groupdocs.search.results.PathDeleteResult[] - نتائج حذف كل مسار.

### getTotalCount() {#getTotalCount--}
```
public final int getTotalCount()
```


يعيد العدد الإجمالي للمسارات التي سيتم حذفها.


**Returns:**
int - العدد الإجمالي للمسارات التي سيتم حذفها.

### getSuccessCount() {#getSuccessCount--}
```
public final int getSuccessCount()
```


يعيد عدد المسارات التي تم حذفها بنجاح.


**Returns:**
int - عدد المسارات التي تم حذفها بنجاح.

### getFailedCount() {#getFailedCount--}
```
public final int getFailedCount()
```


يعيد عدد المسارات التي لم تُحذف بسبب الأخطاء.


**Returns:**
int - عدد المسارات التي لم تُحذف بسبب الأخطاء.

### getErrors() {#getErrors--}
```
public final String[] getErrors()
```


يعيد أوصاف أخطاء الحذف.


**Returns:**
java.lang.String[] - أوصاف أخطاء الحذف.

