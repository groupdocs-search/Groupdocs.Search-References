---
title: "TableDiscreteFunction"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يمثل خوارزمية البحث الضبابي التي تحتوي على تطابقات بين أطوال الكلمات وعدد الأخطاء المسموح بها."
type: docs
weight: 40
url: /ar/java/com.groupdocs.search.options/tablediscretefunction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.options.FuzzyAlgorithm](../../com.groupdocs.search.options/fuzzyalgorithm)
```
public class TableDiscreteFunction extends FuzzyAlgorithm
```

يمثل خوارزمية البحث الضبابي التي تحتوي على تطابقات بين أطوال الكلمات وعدد الأخطاء المسموح بها. يمكن تحديد هذه الخوارزمية بجدول قيم الإخراج أو بواسطة دالة خطوة.


**Learn more**

* [Fuzzy search](../https://docs.groupdocs.com/display/searchjava/Fuzzy+search)


المثال يوضح استخدامًا نموذجيًا للفئة.

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


## المنشئات

| منشئ | الوصف |
| --- | --- |
|  | [TableDiscreteFunction(int offsetOfInputs, int[] tableOfOutputs)](#TableDiscreteFunction-int-int---) | ينشئ مثيلاً جديداً من الفئة TableDiscreteFunction. |
|
|  | [TableDiscreteFunction(int firstStepLevel, Step[] steps)](#TableDiscreteFunction-int-com.groupdocs.search.options.Step...-) | ينشئ مثيلاً جديداً من الفئة TableDiscreteFunction. |
|
## طرق

| طريقة | الوصف |
| --- | --- |
|  | [getSimilarityLevel(int termLength)](#getSimilarityLevel-int-) | يحصل على مستوى التشابه للطول المحدد للمصطلح. |
|
|  | [getMaxMistakeCount(int termLength)](#getMaxMistakeCount-int-) | يحصل على الحد الأقصى المسموح لعدد الأخطاء للطول المحدد للمصطلح. |
|
### TableDiscreteFunction(int offsetOfInputs, int[] tableOfOutputs) {#TableDiscreteFunction-int-int---}
```
public TableDiscreteFunction(int offsetOfInputs, int[] tableOfOutputs)
```


ينشئ مثيلاً جديداً من الفئة TableDiscreteFunction.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | offsetOfInputs | int | الإزاحة في فهارس الجدول بالنسبة للقيم المدخلة. |
|
|  | tableOfOutputs | int[] | جدول قيم الإخراج. |
|

### TableDiscreteFunction(int firstStepLevel, Step[] steps) {#TableDiscreteFunction-int-com.groupdocs.search.options.Step...-}
```
public TableDiscreteFunction(int firstStepLevel, Step[] steps)
```


ينشئ مثيلاً جديداً من الفئة TableDiscreteFunction.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | firstStepLevel | int | مستوى الخطوة الأولى من دالة الخطوة. |
|
|  | steps | [Step\[\]](../../com.groupdocs.search.options/step) | الخطوات التالية لدالة الخطوة. |
|

### getSimilarityLevel(int termLength) {#getSimilarityLevel-int-}
```
public double getSimilarityLevel(int termLength)
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
public int getMaxMistakeCount(int termLength)
```


يحصل على الحد الأقصى المسموح لعدد الأخطاء للطول المحدد للمصطلح.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | termLength | int | طول المصطلح. |
|

**Returns:**
int - الحد الأقصى المسموح لعدد الأخطاء.

