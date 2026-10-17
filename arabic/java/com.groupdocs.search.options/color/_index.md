---
title: "Color"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يمثل لون ARGB ألفا أحمر أخضر أزرق."
type: docs
weight: 11
url: /ar/java/com.groupdocs.search.options/color/
---
**Inheritance:**
java.lang.Object
```
public class Color
```

يمثل لون ARGB (ألفا، أحمر، أخضر، أزرق).

## المنشئات

| منشئ | الوصف |
| --- | --- |
|  | [Color(int alpha, int red, int green, int blue)](#Color-int-int-int-int-) | ينشئ مثيلاً جديداً من فئة  Color  . |
|
|  | [Color(int red, int green, int blue)](#Color-int-int-int-) | ينشئ مثيلاً جديداً من فئة  Color  . |
|
|  | [Color(Object data)](#Color-java.lang.Object-) | ينشئ مثيلاً جديداً من فئة  Color  . |
|
## طرق

| طريقة | الوصف |
| --- | --- |
|  | [getAlpha()](#getAlpha--) | يحصل على قيمة مكوّن الألفا لهذا المثيل. |
|
|  | [getRed()](#getRed--) | يحصل على قيمة مكوّن الأحمر لهذا المثيل. |
|
|  | [getGreen()](#getGreen--) | يحصل على قيمة مكوّن الأخضر لهذا المثيل. |
|
|  | [getBlue()](#getBlue--) | يحصل على قيمة مكوّن الأزرق لهذا المثيل. |
|
|  | [toString()](#toString--) | يرجع  String  تمثّل الـ  Color  الحالي. |
|
| [getCore()](#getCore--) |  |
### Color(int alpha, int red, int green, int blue) {#Color-int-int-int-int-}
```
public Color(int alpha, int red, int green, int blue)
```


ينشئ مثيلاً جديداً من فئة  Color  .


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | alpha | int | مكوّن الألفا من 0 إلى 255. |
|
|  | red | int | المكوّن الأحمر من 0 إلى 255. |
|
|  | أخضر | int | المكوّن الأخضر من 0 إلى 255. |
|
|  | أزرق | int | المكوّن الأزرق من 0 إلى 255. |
|

### Color(int red, int green, int blue) {#Color-int-int-int-}
```
public Color(int red, int green, int blue)
```


ينشئ مثيلاً جديداً من فئة  Color  .


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | red | int | المكوّن الأحمر من 0 إلى 255. |
|
|  | أخضر | int | المكوّن الأخضر من 0 إلى 255. |
|
|  | أزرق | int | المكوّن الأزرق من 0 إلى 255. |
|

### Color(Object data) {#Color-java.lang.Object-}
```
public Color(Object data)
```


ينشئ مثيلاً جديداً من فئة  Color  .


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | البيانات | java.lang.Object | البيانات المتسلسلة. |
|

### getAlpha() {#getAlpha--}
```
public int getAlpha()
```


يحصل على قيمة مكوّن الألفا لهذا المثيل.


**Returns:**
int - قيمة المكوّن ألفا لهذا الكائن.

### getRed() {#getRed--}
```
public int getRed()
```


يحصل على قيمة مكوّن الأحمر لهذا المثيل.


**Returns:**
int - قيمة المكوّن الأحمر لهذا الكائن.

### getGreen() {#getGreen--}
```
public int getGreen()
```


يحصل على قيمة مكوّن الأخضر لهذا المثيل.


**Returns:**
int - قيمة المكوّن الأخضر لهذا الكائن.

### getBlue() {#getBlue--}
```
public int getBlue()
```


يحصل على قيمة مكوّن الأزرق لهذا المثيل.


**Returns:**
int - قيمة المكوّن الأزرق لهذا الكائن.

### toString() {#toString--}
```
public String toString()
```


يرجع  String  تمثّل الـ  Color  الحالي.


**Returns:**
java.lang.String - سلسلة تمثل اللون الحالي.

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
