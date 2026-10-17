---
title: "FuzzyAlgorithm"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يمثل الفئة الأساسية لخوارزميات البحث الضبابي."
type: docs
weight: 20
url: /ar/java/com.groupdocs.search.options/fuzzyalgorithm/
---
**Inheritance:**
java.lang.Object
```
public abstract class FuzzyAlgorithm
```

يمثل الفئة الأساسية لخوارزميات البحث الضبابي.


**Learn more**

* [Fuzzy search](../https://docs.groupdocs.com/display/searchjava/Fuzzy+search)

## طرق

| طريقة | الوصف |
| --- | --- |
|  | [getSimilarityLevel(int termLength)](#getSimilarityLevel-int-) | يحصل على مستوى التشابه للطول المحدد للمصطلح. |
|
|  | [getMaxMistakeCount(int termLength)](#getMaxMistakeCount-int-) | يحصل على الحد الأقصى المسموح به لعدد الأخطاء للطول المحدد للمصطلح. |
|
| [getCore()](#getCore--) |  |
### getSimilarityLevel(int termLength) {#getSimilarityLevel-int-}
```
public abstract double getSimilarityLevel(int termLength)
```


يحصل على مستوى التشابه للطول المحدد للمصطلح.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | termLength | int | طول المصطلح. |
|

**Returns:**
double - مستوى التشابه.

### getMaxMistakeCount(int termLength) {#getMaxMistakeCount-int-}
```
public abstract int getMaxMistakeCount(int termLength)
```


يحصل على الحد الأقصى المسموح به لعدد الأخطاء للطول المحدد للمصطلح.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | termLength | int | طول المصطلح. |
|

**Returns:**
int - الحد الأقصى المسموح به لعدد الأخطاء.

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
