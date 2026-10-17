---
title: "SimilarityLevel"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يمثل خوارزمية البحث الضبابي التي تحدد مستوى التشابه."
type: docs
weight: 35
url: /ar/java/com.groupdocs.search.options/similaritylevel/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.options.FuzzyAlgorithm](../../com.groupdocs.search.options/fuzzyalgorithm)
```
public class SimilarityLevel extends FuzzyAlgorithm
```

يمثل خوارزمية البحث الضبابي التي تحدد مستوى التشابه. تحسب خوارزمية مستوى التشابه الحد الأقصى لعدد الأخطاء لكلمة ما بشكل عكسي يتناسب مع طول الكلمة.


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
options.getFuzzySearch().setFuzzyAlgorithm(new SimilarityLevel(0.8)); // إنشاء خوارزمية البحث الضبابي
// تحدد هذه الدالة 0 كحد أقصى لعدد الأخطاء للكلمات من 1 إلى 4 أحرف.
// تحدد 1 كحد أقصى لعدد الأخطاء للكلمات من 5 إلى 9 أحرف.
// تحدد 2 كحد أقصى لعدد الأخطاء للكلمات من 10 إلى 14 حرفًا. وهكذا.
SearchResult result = index.search(query, options); // بحث في الفهرس
 
```
 
````


## المنشئات

| منشئ | الوصف |
| --- | --- |
|  | [SimilarityLevel(double value)](#SimilarityLevel-double-) | ينشئ مثيلًا جديدًا من الفئة  SimilarityLevel . |
|
|  | [SimilarityLevel(Object data)](#SimilarityLevel-java.lang.Object-) | ينشئ مثيلًا جديدًا من الفئة  SimilarityLevel . |
|
## طرق

| طريقة | الوصف |
| --- | --- |
|  | [getSimilarityLevel(int termLength)](#getSimilarityLevel-int-) | يحصل على قيمة مستوى التشابه للطول المحدد للمصطلح. |
|
|  | [getMaxMistakeCount(int termLength)](#getMaxMistakeCount-int-) | يحصل على الحد الأقصى المسموح به لعدد الأخطاء للطول المحدد للمصطلح. |
|
### SimilarityLevel(double value) {#SimilarityLevel-double-}
```
public SimilarityLevel(double value)
```


ينشئ مثيلًا جديدًا من الفئة  SimilarityLevel .


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | قيمة | double | قيمة مستوى التشابه. |
|

### SimilarityLevel(Object data) {#SimilarityLevel-java.lang.Object-}
```
public SimilarityLevel(Object data)
```


ينشئ مثيلًا جديدًا من الفئة  SimilarityLevel .


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | البيانات | java.lang.Object | البيانات المتسلسلة. |
|

### getSimilarityLevel(int termLength) {#getSimilarityLevel-int-}
```
public double getSimilarityLevel(int termLength)
```


يحصل على قيمة مستوى التشابه للطول المحدد للمصطلح.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | termLength | int | طول المصطلح. |
|

**Returns:**
double - قيمة مستوى التشابه.

### getMaxMistakeCount(int termLength) {#getMaxMistakeCount-int-}
```
public int getMaxMistakeCount(int termLength)
```


يحصل على الحد الأقصى المسموح به لعدد الأخطاء للطول المحدد للمصطلح.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | termLength | int | طول المصطلح. |
|

**Returns:**
int - الحد الأقصى المسموح به لعدد الأخطاء.

