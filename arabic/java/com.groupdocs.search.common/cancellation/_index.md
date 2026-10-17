---
title: "الإلغاء"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يمثل كائنًا لطلب إلغاء عملية."
type: docs
weight: 11
url: /ar/java/com.groupdocs.search.common/cancellation/
---
**Inheritance:**
java.lang.Object
```
public class Cancellation
```

يمثل كائنًا لطلب إلغاء عملية.


**Learn more**

* [Indexing options](../https://docs.groupdocs.com/display/searchjava/Indexing+options)
* [Search options](../https://docs.groupdocs.com/display/searchjava/Search+options)

## المنشئات

| منشئ | الوصف |
| --- | --- |
|  | [Cancellation()](#Cancellation--) | يُنشئ مثيلاً جديدًا لـ |
الإلغاء
الفئة.
|
## طرق

| طريقة | الوصف |
| --- | --- |
|  | [isCancelled()](#isCancelled--) | يحصل على قيمة تشير إلى أن الإلغاء قد تم طلبه. |
|
|  | [cancel()](#cancel--) | يقوم بطلب الإلغاء. |
|
|  | [cancelAfter(int milliseconds)](#cancelAfter-int-) | يقوم بطلب الإلغاء بعد انتهاء عدد محدد من المللي ثانية. |
|
### Cancellation() {#Cancellation--}
```
public Cancellation()
```


يُنشئ مثيلاً جديدًا لـ
الإلغاء
الفئة.


### isCancelled() {#isCancelled--}
```
public final boolean isCancelled()
```


يحصل على قيمة تشير إلى أن الإلغاء قد تم طلبه.


**Returns:**
منطقي - قيمة تشير إلى أن الإلغاء قد تم طلبه.

### cancel() {#cancel--}
```
public final void cancel()
```


يقوم بطلب الإلغاء.


### cancelAfter(int milliseconds) {#cancelAfter-int-}
```
public final void cancelAfter(int milliseconds)
```


يقوم بطلب الإلغاء بعد انتهاء عدد محدد من المللي ثانية.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | مللي ثانية | int | عدد المللي ثانية التي بعده سيتم إلغاء العملية. |
|

