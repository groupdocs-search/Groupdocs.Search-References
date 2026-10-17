---
title: "HighlightOptions"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يوفر خيارات لتسليط الضوء على المصطلحات التي تم العثور عليها."
type: docs
weight: 22
url: /ar/java/com.groupdocs.search.options/highlightoptions/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.options.TextOptions](../../com.groupdocs.search.options/textoptions)

**All Implemented Interfaces:**
[com.groupdocs.search.options.IHighlightOptions](../../com.groupdocs.search.options/ihighlightoptions)
```
public class HighlightOptions extends TextOptions implements IHighlightOptions
```

يوفر خيارات لتسليط الضوء على المصطلحات التي تم العثور عليها.


**Learn more**

* [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)

## المنشئات

| منشئ | الوصف |
| --- | --- |
|  | [HighlightOptions()](#HighlightOptions--) | يُنشئ مثيلاً جديدًا لفئة  HighlightOptions . |
|
|  | [HighlightOptions(Object data)](#HighlightOptions-java.lang.Object-) | يُنشئ مثيلاً جديدًا لفئة  TextOptions . |
|
## طرق

| طريقة | الوصف |
| --- | --- |
|  | [getTermsBefore()](#getTermsBefore--) | يحصل على الحد الأقصى لعدد الكلمات في مقطع نصي قبل الكلمة المميزة. |
|
|  | [setTermsBefore(int value)](#setTermsBefore-int-) | يضبط الحد الأقصى لعدد الكلمات في مقطع نصي قبل الكلمة المميزة. |
|
|  | [getTermsAfter()](#getTermsAfter--) | يحصل على الحد الأقصى لعدد الكلمات في مقطع نصي بعد الكلمة المميزة. |
|
|  | [setTermsAfter(int value)](#setTermsAfter-int-) | يضبط الحد الأقصى لعدد الكلمات في مقطع نصي بعد الكلمة المميزة. |
|
|  | [getTermsTotal()](#getTermsTotal--) | يحصل على الحد الأقصى لعدد الكلمات في مقطع نصي. |
|
|  | [setTermsTotal(int value)](#setTermsTotal-int-) | يضبط الحد الأقصى لعدد الكلمات في مقطع نصي. |
|
|  | [getUseInlineStyles()](#getUseInlineStyles--) | يحصل على قيمة تشير إلى ما إذا كانت الأنماط المضمنة تُستخدم لتسليط الضوء على النتائج. |
|
|  | [setUseInlineStyles(boolean value)](#setUseInlineStyles-boolean-) | يضبط قيمة تشير إلى ما إذا كانت الأنماط المضمنة تُستخدم لتسليط الضوء على النتائج. |
|
|  | [getHighlightColor()](#getHighlightColor--) | يحصل على اللون المستخدم لتسليط الضوء على النتائج. |
|
|  | [setHighlightColor(Color value)](#setHighlightColor-com.groupdocs.search.options.Color-) | يضبط اللون المستخدم لتسليط الضوء على النتائج. |
|
|  | [getTermHighlightStartTag()](#getTermHighlightStartTag--) | يحصل على وسم البداية لتسليط الضوء على الكلمة المكتشفة. |
|
|  | [setTermHighlightStartTag(String value)](#setTermHighlightStartTag-java.lang.String-) | يضبط وسم البداية لتسليط الضوء على الكلمة المكتشفة. |
|
|  | [getTermHighlightEndTag()](#getTermHighlightEndTag--) | يحصل على وسم النهاية لتسليط الضوء على الكلمة المكتشفة. |
|
|  | [setTermHighlightEndTag(String value)](#setTermHighlightEndTag-java.lang.String-) | يضبط وسم النهاية لتسليط الضوء على الكلمة المكتشفة. |
|
### HighlightOptions() {#HighlightOptions--}
```
public HighlightOptions()
```


يُنشئ مثيلاً جديدًا لفئة  HighlightOptions .


### HighlightOptions(Object data) {#HighlightOptions-java.lang.Object-}
```
public HighlightOptions(Object data)
```


يُنشئ مثيلاً جديدًا لفئة  TextOptions .


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | البيانات | java.lang.Object | البيانات المتسلسلة. |
|

### getTermsBefore() {#getTermsBefore--}
```
public int getTermsBefore()
```


يحصل على الحد الأقصى لعدد الكلمات في مقطع نصي قبل الكلمة المميزة. يجب أن تكون القيمة في النطاق من 0 إلى 10000. القيمة الافتراضية هي 7.


**Returns:**
int - الحد الأقصى لعدد الكلمات في مقطع نصي قبل الكلمة المميزة.

### setTermsBefore(int value) {#setTermsBefore-int-}
```
public void setTermsBefore(int value)
```


يضبط الحد الأقصى لعدد الكلمات في مقطع نصي قبل الكلمة المميزة. يجب أن تكون القيمة في النطاق من 0 إلى 10000. القيمة الافتراضية هي 7.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | قيمة | int | الحد الأقصى لعدد الكلمات في مقطع نصي قبل الكلمة المميزة. |
|

### getTermsAfter() {#getTermsAfter--}
```
public int getTermsAfter()
```


يحصل على الحد الأقصى لعدد الكلمات في مقطع نصي بعد الكلمة المميزة. يجب أن تكون القيمة في النطاق من 0 إلى 10000. القيمة الافتراضية هي 7.


**Returns:**
int - الحد الأقصى لعدد الكلمات في مقطع نصي بعد الكلمة المميزة.

### setTermsAfter(int value) {#setTermsAfter-int-}
```
public void setTermsAfter(int value)
```


يضبط الحد الأقصى لعدد الكلمات في مقطع نصي بعد الكلمة المميزة. يجب أن تكون القيمة في النطاق من 0 إلى 10000. القيمة الافتراضية هي 7.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | قيمة | int | الحد الأقصى لعدد الكلمات في مقطع نصي بعد الكلمة المميزة. |
|

### getTermsTotal() {#getTermsTotal--}
```
public int getTermsTotal()
```


يحصل على الحد الأقصى لعدد الكلمات في مقطع نصي. يجب أن تكون القيمة في النطاق من 0 إلى 10000. القيمة الافتراضية هي 21.


**Returns:**
int - الحد الأقصى لعدد الكلمات في مقطع نصي.

### setTermsTotal(int value) {#setTermsTotal-int-}
```
public void setTermsTotal(int value)
```


يضبط الحد الأقصى لعدد الكلمات في مقطع نصي. يجب أن تكون القيمة في النطاق من 0 إلى 10000. القيمة الافتراضية هي 21.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | قيمة | int | الحد الأقصى لعدد الكلمات في مقطع نصي. |
|

### getUseInlineStyles() {#getUseInlineStyles--}
```
public boolean getUseInlineStyles()
```


يحصل على قيمة تشير إلى ما إذا كانت الأنماط المضمنة تُستخدم لتسليط الضوء على التكرارات. القيمة الافتراضية هي true.


**Returns:**
boolean - قيمة تشير إلى ما إذا كانت الأنماط المضمنة تُستخدم لتسليط الضوء على التكرارات.

### setUseInlineStyles(boolean value) {#setUseInlineStyles-boolean-}
```
public void setUseInlineStyles(boolean value)
```


يضبط قيمة تشير إلى ما إذا كانت الأنماط المضمنة تُستخدم لتسليط الضوء على التكرارات. القيمة الافتراضية هي true.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | قيمة | boolean | قيمة تشير إلى ما إذا كانت الأنماط المضمنة تُستخدم لتسليط الضوء على التكرارات. |
|

### getHighlightColor() {#getHighlightColor--}
```
public Color getHighlightColor()
```


يحصل على لون يُستخدم لتسليط الضوء على التكرارات. القيمة الافتراضية هي #FFD800.


**Returns:**
[Color](../../com.groupdocs.search.options/color) - A color that is used to highlight occurrences.

### setHighlightColor(Color value) {#setHighlightColor-com.groupdocs.search.options.Color-}
```
public void setHighlightColor(Color value)
```


يضبط لون يُستخدم لتسليط الضوء على التكرارات. القيمة الافتراضية هي #FFD800.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | value | [Color](../../com.groupdocs.search.options/color) | لون يُستخدم لتسليط الضوء على التكرارات. |
|

### getTermHighlightStartTag() {#getTermHighlightStartTag--}
```
public String getTermHighlightStartTag()
```


يحصل على وسم البداية لتسليط الضوء على الكلمة المكتشفة. يُستخدم هذا الوسم فقط عند التسليط في نص عادي. القيمة الافتراضية هي سلسلة فارغة.


**Returns:**
java.lang.String - وسم البداية لتسليط الضوء على الكلمة المكتشفة.

### setTermHighlightStartTag(String value) {#setTermHighlightStartTag-java.lang.String-}
```
public void setTermHighlightStartTag(String value)
```


يضبط وسم البداية لتسليط الضوء على الكلمة المكتشفة. يُستخدم هذا الوسم فقط عند التسليط في نص عادي. القيمة الافتراضية هي سلسلة فارغة.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | قيمة | java.lang.String | وسم البداية لتسليط الضوء على الكلمة المكتشفة. |
|

### getTermHighlightEndTag() {#getTermHighlightEndTag--}
```
public String getTermHighlightEndTag()
```


يحصل على وسم النهاية لتسليط الضوء على الكلمة المكتشفة. يُستخدم هذا الوسم فقط عند التسليط في نص عادي. القيمة الافتراضية هي سلسلة فارغة.


**Returns:**
java.lang.String - وسم النهاية لتسليط الضوء على الكلمة المكتشفة.

### setTermHighlightEndTag(String value) {#setTermHighlightEndTag-java.lang.String-}
```
public void setTermHighlightEndTag(String value)
```


يضبط علامة النهاية لتسليط الضوء على الكلمة الموجودة. تُستخدم هذه العلامة فقط عند التسليط في النص العادي. القيمة الافتراضية هي سلسلة فارغة.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | قيمة | java.lang.String | علامة النهاية لتسليط الضوء على الكلمة الموجودة. |
|

