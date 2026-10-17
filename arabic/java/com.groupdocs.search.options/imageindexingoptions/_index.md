---
title: "ImageIndexingOptions"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يوفر خيارات فهرسة الصور للبحث العكسي عن الصور."
type: docs
weight: 23
url: /ar/java/com.groupdocs.search.options/imageindexingoptions/
---
**Inheritance:**
java.lang.Object
```
public abstract class ImageIndexingOptions
```

يوفر خيارات فهرسة الصور للبحث العكسي عن الصور.

## المنشئات

| منشئ | الوصف |
| --- | --- |
| [ImageIndexingOptions()](#ImageIndexingOptions--) |  |
## طرق

| طريقة | الوصف |
| --- | --- |
|  | [getEnabledForSeparateImages()](#getEnabledForSeparateImages--) | يحصل على قيمة تشير إلى ما إذا كان سيتم فهرسة ملفات الصور المنفصلة. |
|
|  | [setEnabledForSeparateImages(boolean value)](#setEnabledForSeparateImages-boolean-) | يضبط قيمة تشير إلى ما إذا كان سيتم فهرسة ملفات الصور المنفصلة. |
|
|  | [getEnabledForContainerItemImages()](#getEnabledForContainerItemImages--) | يحصل على قيمة تشير إلى ما إذا كان سيتم فهرسة الصور التي هي عناصر في حاوية (على سبيل المثال، الصور في أرشيف ZIP). |
|
|  | [setEnabledForContainerItemImages(boolean value)](#setEnabledForContainerItemImages-boolean-) | يضبط قيمة تشير إلى ما إذا كان سيتم فهرسة الصور التي هي عناصر في حاوية (على سبيل المثال، الصور في أرشيف ZIP). |
|
|  | [getEnabledForEmbeddedImages()](#getEnabledForEmbeddedImages--) | يحصل على قيمة تشير إلى ما إذا كان سيتم فهرسة الصور المدمجة (على سبيل المثال، الصور في مستند DOCX). |
|
|  | [setEnabledForEmbeddedImages(boolean value)](#setEnabledForEmbeddedImages-boolean-) | يضبط قيمة تشير إلى ما إذا كان سيتم فهرسة الصور المدمجة (على سبيل المثال، الصور في مستند DOCX). |
|
### ImageIndexingOptions() {#ImageIndexingOptions--}
```
public ImageIndexingOptions()
```


### getEnabledForSeparateImages() {#getEnabledForSeparateImages--}
```
public abstract boolean getEnabledForSeparateImages()
```


يحصل على قيمة تشير إلى ما إذا كان سيتم فهرسة ملفات الصور المنفصلة. القيمة الافتراضية هي false .


**Returns:**
منطقي - قيمة تشير إلى ما إذا كان سيتم فهرسة ملفات الصور المنفصلة.

### setEnabledForSeparateImages(boolean value) {#setEnabledForSeparateImages-boolean-}
```
public abstract void setEnabledForSeparateImages(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان سيتم فهرسة ملفات الصور المنفصلة. القيمة الافتراضية هي false .


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | قيمة | boolean | قيمة تشير إلى ما إذا كان سيتم فهرسة ملفات الصور المنفصلة. |
|

### getEnabledForContainerItemImages() {#getEnabledForContainerItemImages--}
```
public abstract boolean getEnabledForContainerItemImages()
```


يحصل على قيمة تشير إلى ما إذا كان سيتم فهرسة الصور التي هي عناصر في حاوية (على سبيل المثال، الصور في أرشيف ZIP). القيمة الافتراضية هي false .


**Returns:**
منطقي - قيمة تشير إلى ما إذا كان سيتم فهرسة الصور التي هي عناصر في حاوية.

### setEnabledForContainerItemImages(boolean value) {#setEnabledForContainerItemImages-boolean-}
```
public abstract void setEnabledForContainerItemImages(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان سيتم فهرسة الصور التي هي عناصر في حاوية (على سبيل المثال، الصور في أرشيف ZIP). القيمة الافتراضية هي false .


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | قيمة | boolean | قيمة تشير إلى ما إذا كان سيتم فهرسة الصور التي هي عناصر في حاوية. |
|

### getEnabledForEmbeddedImages() {#getEnabledForEmbeddedImages--}
```
public abstract boolean getEnabledForEmbeddedImages()
```


يحصل على قيمة تشير إلى ما إذا كان سيتم فهرسة الصور المدمجة (على سبيل المثال، الصور في مستند DOCX). القيمة الافتراضية هي false .


**Returns:**
منطقي - قيمة تشير إلى ما إذا كان سيتم فهرسة الصور المدمجة.

### setEnabledForEmbeddedImages(boolean value) {#setEnabledForEmbeddedImages-boolean-}
```
public abstract void setEnabledForEmbeddedImages(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان سيتم فهرسة الصور المدمجة (على سبيل المثال، الصور في مستند DOCX). القيمة الافتراضية هي false .


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | قيمة | boolean | قيمة تشير إلى ما إذا كان سيتم فهرسة الصور المدمجة. |
|

