---
title: "Delegate"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يمثل مفوضًا يشير إلى نسخة من الفئة التي تحتوي على طريقة يتم استدعاؤها."
type: docs
weight: 14
url: /ar/java/com.groupdocs.search.common/delegate/
---
**Inheritance:**
java.lang.Object
```
public abstract class Delegate
```

يمثل مندوبًا يشير إلى نسخة من فئة لديها طريقة لتُستدعى.

## المنشئات

| منشئ | الوصف |
| --- | --- |
| [Delegate()](#Delegate--) |  |
## طرق

| طريقة | الوصف |
| --- | --- |
|  | [getInvocationList()](#getInvocationList--) | يعيد قائمة الاستدعاءات. |
|
|  | [combine(Delegate a, Delegate b)](#combine-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-) | يجمع مفوضين في واحد. |
|
|  | [combine(Delegate[] delegates)](#combine-com.groupdocs.search.common.Delegate...-) | يجمع عدة مفوضين في واحد. |
|
|  | [remove(Delegate source, Delegate value)](#remove-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-) | يزيل مفوض القيمة من مفوض المصدر. |
|
|  | [removeAll(Delegate source, Delegate value)](#removeAll-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-) | يزيل مفوض القيمة من مفوض المصدر. |
|
|  | [op_Equality(Delegate d1, Delegate d2)](#op-Equality-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-) | يفحص مساواة مفوضين. |
|
|  | [op_Inequality(Delegate d1, Delegate d2)](#op-Inequality-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-) | يفحص عدم مساواة مفوضين. |
|
### Delegate() {#Delegate--}
```
public Delegate()
```


### getInvocationList() {#getInvocationList--}
```
public Delegate[] getInvocationList()
```


يعيد قائمة الاستدعاءات.


**Returns:**
com.groupdocs.search.common.Delegate[] - قائمة استدعاءات.

### combine(Delegate a, Delegate b) {#combine-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-}
```
public static Delegate combine(Delegate a, Delegate b)
```


يجمع مفوضين في واحد.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | a | [Delegate](../../com.groupdocs.search.common/delegate) | المفوض الأول للجمع. |
|
|  | b | [Delegate](../../com.groupdocs.search.common/delegate) | المفوض الثاني للجمع. |
|

**Returns:**
[Delegate](../../com.groupdocs.search.common/delegate) - A new combined delegate.

### combine(Delegate[] delegates) {#combine-com.groupdocs.search.common.Delegate...-}
```
public static Delegate combine(Delegate[] delegates)
```


يجمع عدة مفوضين في واحد.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | delegates | [Delegate\[\]](../../com.groupdocs.search.common/delegate) | المفوضون للجمع. |
|

**Returns:**
[Delegate](../../com.groupdocs.search.common/delegate) - A new combined delegate.

### remove(Delegate source, Delegate value) {#remove-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-}
```
public static Delegate remove(Delegate source, Delegate value)
```


يزيل مفوض القيمة من مفوض المصدر.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | source | [Delegate](../../com.groupdocs.search.common/delegate) | مفوض المصدر. |
|
|  | value | [Delegate](../../com.groupdocs.search.common/delegate) | مفوض القيمة. |
|

**Returns:**
[Delegate](../../com.groupdocs.search.common/delegate) - A new delegate that is a result of removing.

### removeAll(Delegate source, Delegate value) {#removeAll-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-}
```
public static Delegate removeAll(Delegate source, Delegate value)
```


يزيل مفوض القيمة من مفوض المصدر.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | source | [Delegate](../../com.groupdocs.search.common/delegate) | مفوض المصدر. |
|
|  | value | [Delegate](../../com.groupdocs.search.common/delegate) | مفوض القيمة. |
|

**Returns:**
[Delegate](../../com.groupdocs.search.common/delegate) - A new delegate that is a result of removing.

### op_Equality(Delegate d1, Delegate d2) {#op-Equality-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-}
```
public static boolean op_Equality(Delegate d1, Delegate d2)
```


يفحص مساواة مفوضين.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | d1 | [Delegate](../../com.groupdocs.search.common/delegate) | المفوض الأول. |
|
|  | d2 | [Delegate](../../com.groupdocs.search.common/delegate) | المفوض الثاني. |
|

**Returns:**
boolean - نتيجة فحص مساواة مفوضين.

### op_Inequality(Delegate d1, Delegate d2) {#op-Inequality-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-}
```
public static boolean op_Inequality(Delegate d1, Delegate d2)
```


يفحص عدم مساواة مفوضين.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | d1 | [Delegate](../../com.groupdocs.search.common/delegate) | المفوض الأول. |
|
|  | d2 | [Delegate](../../com.groupdocs.search.common/delegate) | المفوض الثاني. |
|

**Returns:**
boolean - نتيجة فحص مندوبين للتحقق من عدم المساواة.

