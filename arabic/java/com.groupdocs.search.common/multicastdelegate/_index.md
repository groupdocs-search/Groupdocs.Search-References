---
title: "MulticastDelegate"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يمثل مفوضًا يشير إلى مثيلات الفئة التي لديها طريقة لتُستدعى."
type: docs
weight: 26
url: /ar/java/com.groupdocs.search.common/multicastdelegate/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.Delegate](../../com.groupdocs.search.common/delegate)
```
public abstract class MulticastDelegate extends Delegate
```

يمثل مندوبًا يشير إلى نسخ من الفئات التي لديها طريقة لتُستدعى.

## المنشئات

| منشئ | الوصف |
| --- | --- |
| [MulticastDelegate()](#MulticastDelegate--) |  |
## طرق

| طريقة | الوصف |
| --- | --- |
|  | [getInvocationList()](#getInvocationList--) | يعيد قائمة الاستدعاءات. |
|
|  | [getDelegateId()](#getDelegateId--) | يرجع معرف المفوض. |
|
|  | [op_Equality(MulticastDelegate d1, MulticastDelegate d2)](#op-Equality-com.groupdocs.search.common.MulticastDelegate-com.groupdocs.search.common.MulticastDelegate-) | يفحص مساواة مفوضين. |
|
|  | [op_Inequality(MulticastDelegate d1, MulticastDelegate d2)](#op-Inequality-com.groupdocs.search.common.MulticastDelegate-com.groupdocs.search.common.MulticastDelegate-) | يفحص عدم مساواة مفوضين. |
|
### MulticastDelegate() {#MulticastDelegate--}
```
public MulticastDelegate()
```


### getInvocationList() {#getInvocationList--}
```
public final Delegate[] getInvocationList()
```


يعيد قائمة الاستدعاءات.


**Returns:**
com.groupdocs.search.common.Delegate[] - قائمة استدعاءات.

### getDelegateId() {#getDelegateId--}
```
public String getDelegateId()
```


يرجع معرف المفوض.


**Returns:**
java.lang.String - معرف المفوض.

### op_Equality(MulticastDelegate d1, MulticastDelegate d2) {#op-Equality-com.groupdocs.search.common.MulticastDelegate-com.groupdocs.search.common.MulticastDelegate-}
```
public static boolean op_Equality(MulticastDelegate d1, MulticastDelegate d2)
```


يفحص مساواة مفوضين.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | d1 | [MulticastDelegate](../../com.groupdocs.search.common/multicastdelegate) | المفوض الأول. |
|
|  | d2 | [MulticastDelegate](../../com.groupdocs.search.common/multicastdelegate) | المفوض الثاني. |
|

**Returns:**
boolean - نتيجة فحص مساواة مفوضين.

### op_Inequality(MulticastDelegate d1, MulticastDelegate d2) {#op-Inequality-com.groupdocs.search.common.MulticastDelegate-com.groupdocs.search.common.MulticastDelegate-}
```
public static boolean op_Inequality(MulticastDelegate d1, MulticastDelegate d2)
```


يفحص عدم مساواة مفوضين.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | d1 | [MulticastDelegate](../../com.groupdocs.search.common/multicastdelegate) | المفوض الأول. |
|
|  | d2 | [MulticastDelegate](../../com.groupdocs.search.common/multicastdelegate) | المفوض الثاني. |
|

**Returns:**
boolean - نتيجة فحص مندوبين للتحقق من عدم المساواة.

