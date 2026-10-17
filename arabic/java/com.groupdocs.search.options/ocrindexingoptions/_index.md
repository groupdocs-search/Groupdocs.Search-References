---
title: "OcrIndexingOptions"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يوفر خيارات لمعالجة OCR وفهرسة النص المعترف به."
type: docs
weight: 31
url: /ar/java/com.groupdocs.search.options/ocrindexingoptions/
---
**Inheritance:**
java.lang.Object
```
public abstract class OcrIndexingOptions
```

يوفر خيارات لمعالجة OCR وفهرسة النص المعترف به.

## المنشئات

| منشئ | الوصف |
| --- | --- |
| [OcrIndexingOptions()](#OcrIndexingOptions--) |  |
## طرق

| طريقة | الوصف |
| --- | --- |
|  | [getEnabledForSeparateImages()](#getEnabledForSeparateImages--) | يحصل على قيمة تشير إلى ما إذا كان يجب التعرف على النص في ملفات صور منفصلة. |
|
|  | [setEnabledForSeparateImages(boolean value)](#setEnabledForSeparateImages-boolean-) | يضبط قيمة تشير إلى ما إذا كان يجب التعرف على النص في ملفات صور منفصلة. |
|
|  | [getEnabledForContainerItemImages()](#getEnabledForContainerItemImages--) | يحصل على قيمة تشير إلى ما إذا كان يجب التعرف على النص في الصور التي هي عناصر في حاوية (مثال، الصور في أرشيف ZIP). |
|
|  | [setEnabledForContainerItemImages(boolean value)](#setEnabledForContainerItemImages-boolean-) | يضبط قيمة تشير إلى ما إذا كان يجب التعرف على النص في الصور التي هي عناصر في حاوية (مثال، الصور في أرشيف ZIP). |
|
|  | [getEnabledForEmbeddedImages()](#getEnabledForEmbeddedImages--) | يحصل على قيمة تشير إلى ما إذا كان سيتم التعرف على النص في الصور المضمّنة (على سبيل المثال، الصور في مستند DOCX). |
|
|  | [setEnabledForEmbeddedImages(boolean value)](#setEnabledForEmbeddedImages-boolean-) | يضبط قيمة تشير إلى ما إذا كان سيتم التعرف على النص في الصور المضمّنة (على سبيل المثال، الصور في مستند DOCX). |
|
|  | [getOcrConnector()](#getOcrConnector--) | يحصل على موصل OCR يُستخدم لمعالجة OCR. |
|
|  | [setOcrConnector(IOcrConnector value)](#setOcrConnector-com.groupdocs.search.options.IOcrConnector-) | يضبط موصل OCR يُستخدم لمعالجة OCR. |
|
### OcrIndexingOptions() {#OcrIndexingOptions--}
```
public OcrIndexingOptions()
```


### getEnabledForSeparateImages() {#getEnabledForSeparateImages--}
```
public abstract boolean getEnabledForSeparateImages()
```


يحصل على قيمة تشير إلى ما إذا كان سيتم التعرف على النص في ملفات صور منفصلة. القيمة الافتراضية هي  false .


**Returns:**
منطقي - قيمة تشير إلى ما إذا كان سيتم التعرف على النص في ملفات صور منفصلة.

### setEnabledForSeparateImages(boolean value) {#setEnabledForSeparateImages-boolean-}
```
public abstract void setEnabledForSeparateImages(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان سيتم التعرف على النص في ملفات صور منفصلة. القيمة الافتراضية هي  false .


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | قيمة | boolean | قيمة تشير إلى ما إذا كان سيتم التعرف على النص في ملفات صور منفصلة. |
|

### getEnabledForContainerItemImages() {#getEnabledForContainerItemImages--}
```
public abstract boolean getEnabledForContainerItemImages()
```


يحصل على قيمة تشير إلى ما إذا كان سيتم التعرف على النص في الصور التي هي عناصر في حاوية (على سبيل المثال، الصور في أرشيف ZIP). القيمة الافتراضية هي  false .


**Returns:**
منطقي - قيمة تشير إلى ما إذا كان سيتم التعرف على النص في الصور التي هي عناصر في حاوية.

### setEnabledForContainerItemImages(boolean value) {#setEnabledForContainerItemImages-boolean-}
```
public abstract void setEnabledForContainerItemImages(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان سيتم التعرف على النص في الصور التي هي عناصر في حاوية (على سبيل المثال، الصور في أرشيف ZIP). القيمة الافتراضية هي  false .


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | قيمة | boolean | قيمة تشير إلى ما إذا كان سيتم التعرف على النص في الصور التي هي عناصر في حاوية. |
|

### getEnabledForEmbeddedImages() {#getEnabledForEmbeddedImages--}
```
public abstract boolean getEnabledForEmbeddedImages()
```


يحصل على قيمة تشير إلى ما إذا كان سيتم التعرف على النص في الصور المضمّنة (على سبيل المثال، الصور في مستند DOCX). القيمة الافتراضية هي  false .


**Returns:**
منطقي - قيمة تشير إلى ما إذا كان سيتم التعرف على النص في الصور المضمّنة.

### setEnabledForEmbeddedImages(boolean value) {#setEnabledForEmbeddedImages-boolean-}
```
public abstract void setEnabledForEmbeddedImages(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان سيتم التعرف على النص في الصور المضمّنة (على سبيل المثال، الصور في مستند DOCX). القيمة الافتراضية هي  false .


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | قيمة | boolean | قيمة تشير إلى ما إذا كان سيتم التعرف على النص في الصور المضمّنة. |
|

### getOcrConnector() {#getOcrConnector--}
```
public abstract IOcrConnector getOcrConnector()
```


يحصل على موصل OCR يُستخدم لمعالجة OCR. القيمة الافتراضية هي  null , مما يعني عدم استخدام OCR.


**Returns:**
[IOcrConnector](../../com.groupdocs.search.options/iocrconnector) - An OCR connector that is used for OCR processing.

### setOcrConnector(IOcrConnector value) {#setOcrConnector-com.groupdocs.search.options.IOcrConnector-}
```
public abstract void setOcrConnector(IOcrConnector value)
```


يضبط موصل OCR يُستخدم لمعالجة OCR. القيمة الافتراضية هي  null , مما يعني عدم استخدام OCR.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | value | [IOcrConnector](../../com.groupdocs.search.options/iocrconnector) | موصل OCR يُستخدم لمعالجة OCR. |
|

