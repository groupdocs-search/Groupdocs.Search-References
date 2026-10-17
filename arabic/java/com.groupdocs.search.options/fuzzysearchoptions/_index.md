---
title: "FuzzySearchOptions"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يوفر خيارات للبحث الضبابي."
type: docs
weight: 21
url: /ar/java/com.groupdocs.search.options/fuzzysearchoptions/
---
**Inheritance:**
java.lang.Object
```
public abstract class FuzzySearchOptions
```

يوفر خيارات للبحث الضبابي.


**Learn more**

* [Fuzzy search](../https://docs.groupdocs.com/display/searchjava/Fuzzy+search)
* [Search options](../https://docs.groupdocs.com/display/searchjava/Search+options)

## المنشئات

| منشئ | الوصف |
| --- | --- |
| [FuzzySearchOptions()](#FuzzySearchOptions--) |  |
## طرق

| طريقة | الوصف |
| --- | --- |
|  | [getEnabled()](#getEnabled--) | يحصل على قيمة تشير إلى ما إذا كانت ميزة البحث الضبابي مفعلة. |
|
|  | [setEnabled(boolean value)](#setEnabled-boolean-) | يضبط قيمة تشير إلى ما إذا كانت ميزة البحث الضبابي مفعلة. |
|
|  | [getFuzzyAlgorithm()](#getFuzzyAlgorithm--) | يحصل على خوارزمية البحث الضبابي. |
|
|  | [setFuzzyAlgorithm(FuzzyAlgorithm value)](#setFuzzyAlgorithm-com.groupdocs.search.options.FuzzyAlgorithm-) | يضبط خوارزمية البحث الضبابي. |
|
|  | [getOnlyBestResults()](#getOnlyBestResults--) | يحصل على قيمة تشير إلى ما إذا كانت النتائج الأفضل فقط ستُعاد. |
|
|  | [setOnlyBestResults(boolean value)](#setOnlyBestResults-boolean-) | يضبط قيمة تشير إلى ما إذا كانت النتائج الأفضل فقط ستُعاد. |
|
|  | [getOnlyBestResultsRange()](#getOnlyBestResultsRange--) | يحصل على الحد الأقصى لتجاوز الحد الأدنى لعدد الأخطاء التي تم العثور عليها. |
|
|  | [setOnlyBestResultsRange(byte value)](#setOnlyBestResultsRange-byte-) | يضبط الحد الأقصى لتجاوز الحد الأدنى لعدد الأخطاء التي تم العثور عليها. |
|
|  | [getConsiderTranspositions()](#getConsiderTranspositions--) | يحصل على قيمة تشير إلى ما إذا كان يجب على خوارزمية البحث الضبابي اعتبار تبديل حرفين متجاورين كخطأ واحد. |
|
|  | [setConsiderTranspositions(boolean value)](#setConsiderTranspositions-boolean-) | يضبط قيمة تشير إلى ما إذا كان يجب على خوارزمية البحث الضبابي اعتبار تبديل حرفين متجاورين كخطأ واحد. |
|
### FuzzySearchOptions() {#FuzzySearchOptions--}
```
public FuzzySearchOptions()
```


### getEnabled() {#getEnabled--}
```
public abstract boolean getEnabled()
```


يحصل على قيمة تشير إلى ما إذا كانت ميزة البحث الضبابي مفعلة. القيمة الافتراضية هي false.


**Returns:**
boolean - قيمة تشير إلى ما إذا كانت ميزة البحث الضبابي مفعلة.

### setEnabled(boolean value) {#setEnabled-boolean-}
```
public abstract void setEnabled(boolean value)
```


يضبط قيمة تشير إلى ما إذا كانت ميزة البحث الضبابي مفعلة. القيمة الافتراضية هي false.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | قيمة | boolean | قيمة تشير إلى ما إذا كانت ميزة البحث الضبابي مفعلة. |
|

### getFuzzyAlgorithm() {#getFuzzyAlgorithm--}
```
public abstract FuzzyAlgorithm getFuzzyAlgorithm()
```


يحصل على خوارزمية البحث الضبابي. الخوارزميات المتاحة حاليًا للبحث الضبابي هي SimilarityLevel و TableDiscreteFunction. القيمة الافتراضية هي نسخة من SimilarityLevel بمستوى تشابه قدره 0.5.


**Returns:**
[FuzzyAlgorithm](../../com.groupdocs.search.options/fuzzyalgorithm) - The fuzzy search algorithm.


يوضح المثال كيفية ضبط خوارزمية البحث الضبابي.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // إنشاء فهرس في المجلد المحدد
index.add(documentsFolder); // فهرسة المستندات من المجلد المحدد
SearchOptions options = new SearchOptions();
options.getFuzzySearch().setEnabled(true); // تمكين بحث Fuzzy
options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(1, new Step(5, 2), new Step(8, 3))); // إنشاء خوارزمية البحث الضبابي
// تحدد هذه الدالة 1 كحد أقصى لعدد الأخطاء للكلمات من 1 إلى 4 أحرف.
// تحدد 2 كحد أقصى لعدد الأخطاء للكلمات من 5 إلى 7 أحرف.
// تحدد 3 كحد أقصى لعدد الأخطاء للكلمات من 8 أحرف فأكثر.
SearchResult result = index.search(query, options); // بحث في الفهرس
 
```
 
````


### setFuzzyAlgorithm(FuzzyAlgorithm value) {#setFuzzyAlgorithm-com.groupdocs.search.options.FuzzyAlgorithm-}
```
public abstract void setFuzzyAlgorithm(FuzzyAlgorithm value)
```


يضبط خوارزمية البحث الضبابي. الخوارزميات المتاحة حاليًا للبحث الضبابي هي SimilarityLevel و TableDiscreteFunction. القيمة الافتراضية هي نسخة من SimilarityLevel بمستوى تشابه قدره 0.5.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | value | [FuzzyAlgorithm](../../com.groupdocs.search.options/fuzzyalgorithm) | خوارزمية البحث الضبابي. |


يوضح المثال كيفية ضبط خوارزمية البحث الضبابي.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // إنشاء فهرس في المجلد المحدد
index.add(documentsFolder); // فهرسة المستندات من المجلد المحدد
SearchOptions options = new SearchOptions();
options.getFuzzySearch().setEnabled(true); // تمكين بحث Fuzzy
options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(1, new Step(5, 2), new Step(8, 3))); // إنشاء خوارزمية البحث الضبابي
// تحدد هذه الدالة 1 كحد أقصى لعدد الأخطاء للكلمات من 1 إلى 4 أحرف.
// تحدد 2 كحد أقصى لعدد الأخطاء للكلمات من 5 إلى 7 أحرف.
// تحدد 3 كحد أقصى لعدد الأخطاء للكلمات من 8 أحرف فأكثر.
SearchResult result = index.search(query, options); // بحث في الفهرس
 
```
 
````

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


يحصل على قيمة تشير إلى ما إذا كانت خوارزمية البحث الضبابي يجب أن تعتبر تبديل حرفين متجاورين كخطأ واحد. القيمة الافتراضية هي true.


**Returns:**
منطقي - true إذا كانت خوارزمية البحث الضبابي تعتبر التبديلات؛ وإلا false.

### setConsiderTranspositions(boolean value) {#setConsiderTranspositions-boolean-}
```
public abstract void setConsiderTranspositions(boolean value)
```


يضبط قيمة تشير إلى ما إذا كانت خوارزمية البحث الضبابي يجب أن تعتبر تبديل حرفين متجاورين كخطأ واحد. القيمة الافتراضية هي true.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | قيمة | boolean | : true إذا كانت خوارزمية البحث الضبابي تعتبر التبديلات؛ وإلا false. |
|

