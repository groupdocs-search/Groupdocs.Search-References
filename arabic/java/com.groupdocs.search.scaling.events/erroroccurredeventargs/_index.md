---
title: "ErrorOccurredEventArgs"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يمثل المعلمات لحدث حدوث خطأ في أحد عقد شبكة البحث."
type: docs
weight: 13
url: /ar/java/com.groupdocs.search.scaling.events/erroroccurredeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class ErrorOccurredEventArgs extends EventArgs
```

يمثل المعلمات لحدث حدوث خطأ في أحد عقد شبكة البحث.

## طرق

| طريقة | الوصف |
| --- | --- |
|  | [getNodeIndex()](#getNodeIndex--) | يحصل على فهرس عقدة شبكة البحث. |
|
|  | [getServiceIndex()](#getServiceIndex--) | يحصل على فهرس خدمة عقدة شبكة البحث. |
|
|  | [getMessage()](#getMessage--) | يحصل على رسالة الخطأ. |
|
### getNodeIndex() {#getNodeIndex--}
```
public final int getNodeIndex()
```


يحصل على فهرس عقدة شبكة البحث.


**Returns:**
int - فهرس عقدة شبكة البحث.

### getServiceIndex() {#getServiceIndex--}
```
public final int getServiceIndex()
```


يحصل على فهرس خدمة عقدة شبكة البحث.


**Returns:**
int - فهرس خدمة عقدة شبكة البحث.

### getMessage() {#getMessage--}
```
public final String getMessage()
```


يحصل على رسالة الخطأ.


**Returns:**
java.lang.String - رسالة الخطأ.

