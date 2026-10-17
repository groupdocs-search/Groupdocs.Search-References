---
title: "MergeOptions"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يوفر خيارات لعملية الدمج."
type: docs
weight: 28
url: /ar/java/com.groupdocs.search.options/mergeoptions/
---
**Inheritance:**
java.lang.Object
```
public class MergeOptions
```

يوفر خيارات لعملية الدمج.


**Learn more**

* [Merge indexes](../https://docs.groupdocs.com/display/searchjava/Merge+indexes)
* [Optimize index](../https://docs.groupdocs.com/display/searchjava/Optimize+index)

## المنشئات

| منشئ | الوصف |
| --- | --- |
|  | [MergeOptions()](#MergeOptions--) | يُنشئ مثيلاً جديدًا من الفئة MergeOptions. |
|
## طرق

| طريقة | الوصف |
| --- | --- |
|  | [isAsync()](#isAsync--) | يحصل على علم تنفيذ العملية بشكل غير متزامن. |
|
|  | [setAsync(boolean value)](#setAsync-boolean-) | يضبط علم تنفيذ العملية بشكل غير متزامن. |
|
|  | [getCancellation()](#getCancellation--) | يحصل على كائن إلغاء العملية. |
|
|  | [setCancellation(Cancellation value)](#setCancellation-com.groupdocs.search.common.Cancellation-) | يضبط كائن إلغاء العملية. |
|
### MergeOptions() {#MergeOptions--}
```
public MergeOptions()
```


يُنشئ مثيلاً جديدًا من الفئة MergeOptions.


### isAsync() {#isAsync--}
```
public final boolean isAsync()
```


يحصل على علامة التنفيذ غير المتزامن للعملية. القيمة الافتراضية هي false.


**Returns:**
boolean - علامة التنفيذ غير المتزامن للعملية.

### setAsync(boolean value) {#setAsync-boolean-}
```
public final void setAsync(boolean value)
```


يضبط علامة التنفيذ غير المتزامن للعملية. القيمة الافتراضية هي false.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | قيمة | boolean | علامة التنفيذ غير المتزامن للعملية. |
|

### getCancellation() {#getCancellation--}
```
public final Cancellation getCancellation()
```


يحصل على كائن إلغاء العملية. القيمة الافتراضية هي null.


**Returns:**
[Cancellation](../../com.groupdocs.search.common/cancellation) - The operation cancellation object.

### setCancellation(Cancellation value) {#setCancellation-com.groupdocs.search.common.Cancellation-}
```
public final void setCancellation(Cancellation value)
```


يضبط كائن إلغاء العملية. القيمة الافتراضية هي null.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | value | [Cancellation](../../com.groupdocs.search.common/cancellation) | كائن إلغاء العملية. |
|

