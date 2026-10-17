---
title: "SpellingCorrectorOptions"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يوفر خيارات لمصحح الإملاء."
type: docs
weight: 36
url: /ar/java/com.groupdocs.search.options/spellingcorrectoroptions/
---
**Inheritance:**
java.lang.Object
```
public abstract class SpellingCorrectorOptions
```

يوفر خيارات لمصحح الإملاء.


**Learn more**

* [Spell checking](../https://docs.groupdocs.com/display/searchjava/Spell+checking)
* [Search options](../https://docs.groupdocs.com/display/searchjava/Search+options)

## المنشئات

| منشئ | الوصف |
| --- | --- |
| [SpellingCorrectorOptions()](#SpellingCorrectorOptions--) |  |
## طرق

| طريقة | الوصف |
| --- | --- |
|  | [getEnabled()](#getEnabled--) | يحصل على قيمة تشير إلى ما إذا كان مصحح الإملاء مفعلاً. |
|
|  | [setEnabled(boolean value)](#setEnabled-boolean-) | يضبط قيمة تشير إلى ما إذا كان مصحح الإملاء مفعلاً. |
|
|  | [getMaxMistakeCount()](#getMaxMistakeCount--) | يحصل على الحد الأقصى لعدد الأخطاء. |
|
|  | [setMaxMistakeCount(int value)](#setMaxMistakeCount-int-) | يضبط الحد الأقصى لعدد الأخطاء. |
|
|  | [getOnlyBestResults()](#getOnlyBestResults--) | يحصل على قيمة تشير إلى ما إذا كانت النتائج الأفضل فقط ستُعاد. |
|
|  | [setOnlyBestResults(boolean value)](#setOnlyBestResults-boolean-) | يضبط قيمة تشير إلى ما إذا كانت النتائج الأفضل فقط ستُعاد. |
|
|  | [getOnlyBestResultsRange()](#getOnlyBestResultsRange--) | يحصل على الحد الأقصى لتجاوز الحد الأدنى لعدد الأخطاء التي تم العثور عليها. |
|
|  | [setOnlyBestResultsRange(byte value)](#setOnlyBestResultsRange-byte-) | يضبط الحد الأقصى لتجاوز الحد الأدنى لعدد الأخطاء التي تم العثور عليها. |
|
|  | [getConsiderTranspositions()](#getConsiderTranspositions--) | يحصل على قيمة تشير إلى ما إذا كان يجب على الخوارزمية اعتبار تبديل حرفين متجاورين كخطأ واحد. |
|
|  | [setConsiderTranspositions(boolean value)](#setConsiderTranspositions-boolean-) | يضبط قيمة تشير إلى ما إذا كان يجب على الخوارزمية اعتبار تبديل حرفين متجاورين كخطأ واحد. |
|
### SpellingCorrectorOptions() {#SpellingCorrectorOptions--}
```
public SpellingCorrectorOptions()
```


### getEnabled() {#getEnabled--}
```
public abstract boolean getEnabled()
```


يحصل على قيمة تشير إلى ما إذا كان مصحح الإملاء مفعلاً. القيمة الافتراضية هي false.


**Returns:**
boolean - قيمة تشير إلى ما إذا كان مصحح الإملاء مفعلاً.

### setEnabled(boolean value) {#setEnabled-boolean-}
```
public abstract void setEnabled(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان مصحح الإملاء مفعلاً. القيمة الافتراضية هي false.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | قيمة | boolean | قيمة تشير إلى ما إذا كان مصحح الإملاء مفعلاً. |
|

### getMaxMistakeCount() {#getMaxMistakeCount--}
```
public abstract int getMaxMistakeCount()
```


يحصل على الحد الأقصى لعدد الأخطاء. القيمة الافتراضية هي 2.


**Returns:**
int - الحد الأقصى لعدد الأخطاء.

### setMaxMistakeCount(int value) {#setMaxMistakeCount-int-}
```
public abstract void setMaxMistakeCount(int value)
```


يضبط الحد الأقصى لعدد الأخطاء. القيمة الافتراضية هي 2.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | قيمة | int | الحد الأقصى لعدد الأخطاء. |
|

### getOnlyBestResults() {#getOnlyBestResults--}
```
public abstract boolean getOnlyBestResults()
```


يحصل على قيمة تشير إلى ما إذا كانت النتائج الأفضل فقط ستُعاد. القيمة الافتراضية هي false.


**Returns:**
boolean -  true  إذا كانت النتائج الأفضل فقط ستُعاد؛ وإلا  false .

### setOnlyBestResults(boolean value) {#setOnlyBestResults-boolean-}
```
public abstract void setOnlyBestResults(boolean value)
```


يضبط قيمة تشير إلى ما إذا كانت النتائج الأفضل فقط ستُعاد. القيمة الافتراضية هي false.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | قيمة | boolean | true  إذا كانت النتائج الأفضل فقط ستُعاد؛ وإلا  false . |
|

### getOnlyBestResultsRange() {#getOnlyBestResultsRange--}
```
public abstract byte getOnlyBestResultsRange()
```


يحصل على الحد الأقصى لتجاوز الحد الأدنى لعدد الأخطاء التي تم العثور عليها. القيمة الافتراضية هي 0.


**Returns:**
byte - الحد الأقصى لتجاوز الحد الأدنى لعدد الأخطاء التي تم العثور عليها.

### setOnlyBestResultsRange(byte value) {#setOnlyBestResultsRange-byte-}
```
public abstract void setOnlyBestResultsRange(byte value)
```


يضبط الحد الأقصى لتجاوز الحد الأدنى لعدد الأخطاء التي تم العثور عليها. القيمة الافتراضية هي 0.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | قيمة | byte | الحد الأقصى لتجاوز الحد الأدنى لعدد الأخطاء التي تم العثور عليها. |
|

### getConsiderTranspositions() {#getConsiderTranspositions--}
```
public abstract boolean getConsiderTranspositions()
```


يحصل على قيمة تشير إلى ما إذا كان يجب على الخوارزمية اعتبار تبديل حرفين متجاورين كخطأ واحد. القيمة الافتراضية هي true.


**Returns:**
boolean - true إذا كان خوارزمية تصحيح الإملاء تعتبر التبديلات؛ وإلا false.

### setConsiderTranspositions(boolean value) {#setConsiderTranspositions-boolean-}
```
public abstract void setConsiderTranspositions(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان يجب على الخوارزمية اعتبار تبديل حرفين متجاورين كخطأ واحد. القيمة الافتراضية هي true.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | قيمة | boolean | true إذا كان خوارزمية تصحيح الإملاء تعتبر التبديلات؛ وإلا false. |
|

