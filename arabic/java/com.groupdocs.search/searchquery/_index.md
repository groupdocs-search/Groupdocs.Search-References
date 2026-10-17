---
title: "SearchQuery"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يمثل استعلام بحث في شكل كائن."
type: docs
weight: 25
url: /ar/java/com.groupdocs.search/searchquery/
---
**Inheritance:**
java.lang.Object
```
public abstract class SearchQuery
```

يمثل استعلام بحث في شكل كائن.


**Learn more**

* [Searching](../https://docs.groupdocs.com/display/searchjava/Searching)
* [Queries in text and object form](../https://docs.groupdocs.com/display/searchjava/Queries+in+text+and+object+form)
* [Nesting search queries in object form](../https://docs.groupdocs.com/display/searchjava/Nesting+search+queries+in+object+form)


المثال يوضح استخدامًا نموذجيًا للفئة.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
 
Index index = new Index(indexFolder); // إنشاء فهرس في المجلد المحدد
index.add(documentsFolder); // فهرسة المستندات من المجلد المحدد
 
// إنشاء استعلام فرعي للبحث بنطاق التاريخ
SearchQuery subquery1 = SearchQuery.createDateRangeQuery(new Date(2011, 6, 17), new Date(2013, 1, 1));
 
// إنشاء استعلام فرعي للوايلدكارد مع عدد الكلمات المفقودة من 0 إلى 2
SearchQuery subquery2 = SearchQuery.createWildcardQuery(0, 2);
 
// إنشاء استعلام فرعي لكلمة بسيطة
SearchQuery subquery3 = SearchQuery.createWordQuery("birth");
subquery3.setSearchOptions(new SearchOptions()); // ضبط خيارات البحث فقط للاستعلام الفرعي 3
subquery3.getSearchOptions().getFuzzySearch().setEnabled(true);
subquery3.getSearchOptions().getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(1));
 
// دمج الاستعلامات الفرعية في استعلام واحد
SearchQuery query = SearchQuery.createPhraseSearchQuery(subquery1, subquery2, subquery3);
 
// إنشاء كائن خيارات البحث بزيادة سعة النتائج المكتشفة
SearchOptions options = new SearchOptions(); // خيارات البحث العامة
options.setMaxOccurrenceCountPerTerm(1000000);
options.setMaxTotalOccurrenceCount(10000000);
 
SearchResult result = index.search(query, options); // البحث
 
```
 
````


## طرق

| طريقة | الوصف |
| --- | --- |
|  | [getFieldName()](#getFieldName--) | يحصل على اسم الحقل. |
|
|  | [getChildCount()](#getChildCount--) | يحصل على عدد الاستعلامات الفرعية. |
|
|  | [getFirstChild()](#getFirstChild--) | يحصل على الاستعلام الفرعي الأول. |
|
|  | [getSecondChild()](#getSecondChild--) | يحصل على الاستعلام الفرعي الثاني. |
|
|  | [getChild(int index)](#getChild-int-) | يحصل على استعلام فرعي وفق فهرس. |
|
|  | [getSearchOptions()](#getSearchOptions--) | يحصل أو يضبط خيارات البحث لهذا الاستعلام. |
|
|  | [setSearchOptions(SearchOptions value)](#setSearchOptions-com.groupdocs.search.options.SearchOptions-) | يحصل أو يضبط خيارات البحث لهذا الاستعلام. |
|
|  | [toString()](#toString--) | يرجع  System.String  الذي يمثل نسخة  SearchQuery  الحالية. |
|
|  | [createWordQuery(String term)](#createWordQuery-java.lang.String-) | ينشئ استعلام كلمة بسيط. |
|
|  | [createWordPatternQuery(WordPattern pattern)](#createWordPatternQuery-com.groupdocs.search.common.WordPattern-) | ينشئ استعلام نمط كلمة. |
|
|  | [createRegexQuery(String pattern)](#createRegexQuery-java.lang.String-) | ينشئ استعلام تعبير نمطي. |
|
|  | [createRegexQuery(String pattern, int options)](#createRegexQuery-java.lang.String-int-) | ينشئ استعلام تعبير نمطي. |
|
|  | [createNumericRangeQuery(long start, long end)](#createNumericRangeQuery-long-long-) | ينشئ استعلام نطاق رقمي. |
|
|  | [createDateRangeQuery(Date start, Date end)](#createDateRangeQuery-java.util.Date-java.util.Date-) | ينشئ استعلام نطاق تاريخ. |
|
|  | [createPhraseSearchQuery(SearchQuery[] queries)](#createPhraseSearchQuery-com.groupdocs.search.SearchQuery...-) | ينشئ استعلام بحث عبارة. |
|
|  | [createAndQuery(SearchQuery[] queries)](#createAndQuery-com.groupdocs.search.SearchQuery---) | ينشئ استعلامًا مركبًا سيجد فقط المستندات التي سيتم العثور عليها لكل استعلام أصلي. |
|
|  | [createFieldQuery(String fieldName, SearchQuery query)](#createFieldQuery-java.lang.String-com.groupdocs.search.SearchQuery-) | يضيف حقلًا إلى الاستعلام المحدد. |
|
|  | [createNotQuery(SearchQuery query)](#createNotQuery-com.groupdocs.search.SearchQuery-) | ينشئ استعلامًا مقلوبًا سيجد باقي المستندات في الفهرس مقابل تلك التي سيتم العثور عليها للاستعلام الأصلي. |
|
|  | [createAndQuery(SearchQuery leftQuery, SearchQuery rightQuery)](#createAndQuery-com.groupdocs.search.SearchQuery-com.groupdocs.search.SearchQuery-) | ينشئ استعلامًا مركبًا سيجد فقط المستندات التي سيتم العثور عليها لكل استعلام أصلي. |
|
|  | [createOrQuery(SearchQuery leftQuery, SearchQuery rightQuery)](#createOrQuery-com.groupdocs.search.SearchQuery-com.groupdocs.search.SearchQuery-) | ينشئ استعلامًا مركبًا سيجد جميع المستندات التي سيتم العثور عليها على الأقل في أحد الاستعلامات الأصلية. |
|
|  | [createOrQuery(SearchQuery[] queries)](#createOrQuery-com.groupdocs.search.SearchQuery---) | ينشئ استعلامًا مركبًا سيجد جميع المستندات التي سيتم العثور عليها على الأقل في أحد الاستعلامات الأصلية. |
|
|  | [createWildcardQuery(int count)](#createWildcardQuery-int-) | ينشئ حرفًا بديلًا للبحث عن العبارة. |
|
|  | [createWildcardQuery(int minCount, int maxCount)](#createWildcardQuery-int-int-) | ينشئ حرفًا بديلًا للبحث عن العبارة. |
|
### getFieldName() {#getFieldName--}
```
public String getFieldName()
```


يحصل على اسم الحقل.


**Returns:**
java.lang.String - اسم الحقل.

### getChildCount() {#getChildCount--}
```
public int getChildCount()
```


يحصل على عدد الاستعلامات الفرعية.


**Returns:**
int - عدد الاستعلامات الفرعية.

### getFirstChild() {#getFirstChild--}
```
public SearchQuery getFirstChild()
```


يحصل على الاستعلام الفرعي الأول.


**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - The first child query.

### getSecondChild() {#getSecondChild--}
```
public SearchQuery getSecondChild()
```


يحصل على الاستعلام الفرعي الثاني.


**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - The second child query.

### getChild(int index) {#getChild-int-}
```
public abstract SearchQuery getChild(int index)
```


يحصل على استعلام فرعي وفق فهرس.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | الفهرس | int | الفهرس. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A child query corresponding the specified index.

### getSearchOptions() {#getSearchOptions--}
```
public final SearchOptions getSearchOptions()
```


يحصل أو يضبط خيارات البحث لهذا الاستعلام.


**Returns:**
[SearchOptions](../../com.groupdocs.search.options/searchoptions) - The search options.

### setSearchOptions(SearchOptions value) {#setSearchOptions-com.groupdocs.search.options.SearchOptions-}
```
public final void setSearchOptions(SearchOptions value)
```


يحصل أو يضبط خيارات البحث لهذا الاستعلام.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | value | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | خيارات البحث. |
|

### toString() {#toString--}
```
public abstract String toString()
```


يرجع  System.String  الذي يمثل نسخة  SearchQuery  الحالية.


**Returns:**
java.lang.String - سلسلة System.String تمثل نسخة SearchQuery الحالية.

### createWordQuery(String term) {#createWordQuery-java.lang.String-}
```
public static SearchQuery createWordQuery(String term)
```


ينشئ استعلام كلمة بسيط.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | المصطلح | java.lang.String | المصطلح المراد البحث عنه. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A simple word query.

### createWordPatternQuery(WordPattern pattern) {#createWordPatternQuery-com.groupdocs.search.common.WordPattern-}
```
public static SearchQuery createWordPatternQuery(WordPattern pattern)
```


ينشئ استعلام نمط كلمة.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | pattern | [WordPattern](../../com.groupdocs.search.common/wordpattern) | نمط الكلمة. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A word pattern query.

### createRegexQuery(String pattern) {#createRegexQuery-java.lang.String-}
```
public static SearchQuery createRegexQuery(String pattern)
```


ينشئ استعلام تعبير نمطي.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | pattern | java.lang.String | نمط التعبير النمطي للمطابقة. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A regular expression query.

### createRegexQuery(String pattern, int options) {#createRegexQuery-java.lang.String-int-}
```
public static SearchQuery createRegexQuery(String pattern, int options)
```


ينشئ استعلام تعبير نمطي.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | pattern | java.lang.String | نمط التعبير النمطي للمطابقة. |
|
|  | options | int | تركيبة بتية من قيم التعداد التي تعدل التعبير النمطي. يجب أن يحتوي هذا القيمة على علم RegexOptions.IgnoreCase. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A regular expression query.

### createNumericRangeQuery(long start, long end) {#createNumericRangeQuery-long-long-}
```
public static SearchQuery createNumericRangeQuery(long start, long end)
```


ينشئ استعلام نطاق رقمي.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | البداية | long | قيمة البداية لنطاق. |
|
|  | النهاية | long | قيمة النهاية لنطاق. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A numeric range query.

### createDateRangeQuery(Date start, Date end) {#createDateRangeQuery-java.util.Date-java.util.Date-}
```
public static SearchQuery createDateRangeQuery(Date start, Date end)
```


ينشئ استعلام نطاق تاريخ.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | البداية | java.util.Date | قيمة البداية لنطاق. |
|
|  | النهاية | java.util.Date | قيمة النهاية لنطاق. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A date range query.

### createPhraseSearchQuery(SearchQuery[] queries) {#createPhraseSearchQuery-com.groupdocs.search.SearchQuery...-}
```
public static SearchQuery createPhraseSearchQuery(SearchQuery[] queries)
```


ينشئ استعلام بحث عبارة.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | queries | [SearchQuery\[\]](../../com.groupdocs.search/searchquery) | الاستعلامات الفرعية. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A phrase search query.

### createAndQuery(SearchQuery[] queries) {#createAndQuery-com.groupdocs.search.SearchQuery---}
```
public static SearchQuery createAndQuery(SearchQuery[] queries)
```


ينشئ استعلامًا مركبًا سيجد فقط المستندات التي سيتم العثور عليها لكل استعلام أصلي.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | queries | [SearchQuery\[\]](../../com.groupdocs.search/searchquery) | اسم الحقل للبحث فيه. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A combined AND query.

### createFieldQuery(String fieldName, SearchQuery query) {#createFieldQuery-java.lang.String-com.groupdocs.search.SearchQuery-}
```
public static SearchQuery createFieldQuery(String fieldName, SearchQuery query)
```


يضيف حقلًا إلى الاستعلام المحدد.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | fieldName | java.lang.String | اسم الحقل للبحث فيه. |
|
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | الاستعلام لإضافة الحقل. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A query with the field to search in.

### createNotQuery(SearchQuery query) {#createNotQuery-com.groupdocs.search.SearchQuery-}
```
public static SearchQuery createNotQuery(SearchQuery query)
```


ينشئ استعلامًا مقلوبًا سيجد باقي المستندات في الفهرس مقابل تلك التي سيتم العثور عليها للاستعلام الأصلي.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | الاستعلام لعكسه. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A combined NOT query.

### createAndQuery(SearchQuery leftQuery, SearchQuery rightQuery) {#createAndQuery-com.groupdocs.search.SearchQuery-com.groupdocs.search.SearchQuery-}
```
public static SearchQuery createAndQuery(SearchQuery leftQuery, SearchQuery rightQuery)
```


ينشئ استعلامًا مركبًا سيجد فقط المستندات التي سيتم العثور عليها لكل استعلام أصلي.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | leftQuery | [SearchQuery](../../com.groupdocs.search/searchquery) | استعلام الطفل الأيسر. |
|
|  | rightQuery | [SearchQuery](../../com.groupdocs.search/searchquery) | استعلام الطفل الأيمن. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A combined AND query.

### createOrQuery(SearchQuery leftQuery, SearchQuery rightQuery) {#createOrQuery-com.groupdocs.search.SearchQuery-com.groupdocs.search.SearchQuery-}
```
public static SearchQuery createOrQuery(SearchQuery leftQuery, SearchQuery rightQuery)
```


ينشئ استعلامًا مركبًا سيجد جميع المستندات التي سيتم العثور عليها على الأقل في أحد الاستعلامات الأصلية.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | leftQuery | [SearchQuery](../../com.groupdocs.search/searchquery) | استعلام الطفل الأيسر. |
|
|  | rightQuery | [SearchQuery](../../com.groupdocs.search/searchquery) | استعلام الطفل الأيمن. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A combined OR query.

### createOrQuery(SearchQuery[] queries) {#createOrQuery-com.groupdocs.search.SearchQuery---}
```
public static SearchQuery createOrQuery(SearchQuery[] queries)
```


ينشئ استعلامًا مركبًا سيجد جميع المستندات التي سيتم العثور عليها على الأقل في أحد الاستعلامات الأصلية.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | queries | [SearchQuery\[\]](../../com.groupdocs.search/searchquery) | الاستعلامات الفرعية. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A combined OR query.

### createWildcardQuery(int count) {#createWildcardQuery-int-}
```
public static SearchQuery createWildcardQuery(int count)
```


ينشئ حرفًا بديلًا للبحث عن العبارة.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | العدد | int | عدد الكلمات في البدل. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A wildcard for the phrase search.

### createWildcardQuery(int minCount, int maxCount) {#createWildcardQuery-int-int-}
```
public static SearchQuery createWildcardQuery(int minCount, int maxCount)
```


ينشئ حرفًا بديلًا للبحث عن العبارة.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | minCount | int | الحد الأدنى لعدد الكلمات في البدل. |
|
|  | maxCount | int | الحد الأقصى لعدد الكلمات في البدل. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A wildcard for the phrase search.

