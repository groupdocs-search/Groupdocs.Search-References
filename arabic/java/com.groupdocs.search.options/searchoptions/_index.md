---
title: "SearchOptions"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يوفر خيارات لعملية البحث."
type: docs
weight: 34
url: /ar/java/com.groupdocs.search.options/searchoptions/
---
**Inheritance:**
java.lang.Object
```
public class SearchOptions
```

يوفر خيارات لعملية البحث.


**Learn more**

* [Search options](../https://docs.groupdocs.com/display/searchjava/Search+options)

## المنشئات

| منشئ | الوصف |
| --- | --- |
|  | [SearchOptions()](#SearchOptions--) | يقوم بتهيئة نسخة جديدة من الفئة  SearchOptions  . |
|
|  | [SearchOptions(Object data)](#SearchOptions-java.lang.Object-) | يقوم بتهيئة نسخة جديدة من الفئة  SearchOptions  . |
|
## طرق

| طريقة | الوصف |
| --- | --- |
|  | [getUseSynonymSearch()](#getUseSynonymSearch--) | يحصل على علم استخدام المرادفات في البحث. |
|
|  | [setUseSynonymSearch(boolean value)](#setUseSynonymSearch-boolean-) | يضبط علم استخدام المرادفات في البحث. |
|
|  | [getUseHomophoneSearch()](#getUseHomophoneSearch--) | يحصل على علم استخدام المتشابهات الصوتية في البحث. |
|
|  | [setUseHomophoneSearch(boolean value)](#setUseHomophoneSearch-boolean-) | يضبط علم استخدام المتشابهات الصوتية في البحث. |
|
|  | [getUseWordFormsSearch()](#getUseWordFormsSearch--) | يحصل على علم استخدام صيغ الكلمات المختلفة في البحث. |
|
|  | [setUseWordFormsSearch(boolean value)](#setUseWordFormsSearch-boolean-) | يضبط علم استخدام صيغ الكلمات المختلفة في البحث. |
|
|  | [getRetrieveAttributes()](#getRetrieveAttributes--) | يحصل على علم استرجاع السمات المرتبطة بالمستندات التي تم العثور عليها. |
|
|  | [setRetrieveAttributes(boolean value)](#setRetrieveAttributes-boolean-) | يضبط علم استرجاع السمات المرتبطة بالمستندات التي تم العثور عليها. |
|
|  | [getFuzzySearch()](#getFuzzySearch--) | يحصل على خيارات البحث الضبابي. |
|
|  | [getSpellingCorrector()](#getSpellingCorrector--) | يحصل على خيارات مصحح الإملاء. |
|
|  | [getKeyboardLayoutCorrector()](#getKeyboardLayoutCorrector--) | يحصل على خيارات مصحح تخطيط لوحة المفاتيح. |
|
|  | [getUseCaseSensitiveSearch()](#getUseCaseSensitiveSearch--) | يحصل على علم البحث حساس لحالة الأحرف. |
|
|  | [setUseCaseSensitiveSearch(boolean value)](#setUseCaseSensitiveSearch-boolean-) | يضبط علم البحث حساس لحالة الأحرف. |
|
|  | [getMaxTotalOccurrenceCount()](#getMaxTotalOccurrenceCount--) | يحصل على الحد الأقصى الإجمالي لعدد مرات ظهور جميع المصطلحات في استعلام البحث. |
|
|  | [setMaxTotalOccurrenceCount(int value)](#setMaxTotalOccurrenceCount-int-) | يحدد الحد الأقصى الإجمالي لعدد مرات ظهور جميع المصطلحات في استعلام البحث. |
|
|  | [getMaxOccurrenceCountPerTerm()](#getMaxOccurrenceCountPerTerm--) | يحصل على الحد الأقصى لعدد مرات ظهور كل مصطلح في استعلام البحث. |
|
|  | [setMaxOccurrenceCountPerTerm(int value)](#setMaxOccurrenceCountPerTerm-int-) | يحدد الحد الأقصى لعدد مرات ظهور كل مصطلح في استعلام البحث. |
|
|  | [getDateFormats()](#getDateFormats--) | يحصل على مجموعة صيغ التاريخ للبحث في نطاق التاريخ. |
|
|  | [isChunkSearch()](#isChunkSearch--) | يحصل على علم البحث على أجزاء. |
|
|  | [setChunkSearch(boolean value)](#setChunkSearch-boolean-) | يحدد علم البحث على أجزاء. |
|
|  | [getSearchDocumentFilter()](#getSearchDocumentFilter--) | يحصل على مرشح مستند البحث. |
|
|  | [setSearchDocumentFilter(ISearchDocumentFilter value)](#setSearchDocumentFilter-com.groupdocs.search.options.ISearchDocumentFilter-) | يحدد مرشح مستند البحث. |
|
|  | [getCancellation()](#getCancellation--) | يحصل على كائن إلغاء العملية. |
|
|  | [setCancellation(Cancellation value)](#setCancellation-com.groupdocs.search.common.Cancellation-) | يضبط كائن إلغاء العملية. |
|
| [getCore()](#getCore--) |  |
### SearchOptions() {#SearchOptions--}
```
public SearchOptions()
```


يقوم بتهيئة نسخة جديدة من الفئة  SearchOptions  .


### SearchOptions(Object data) {#SearchOptions-java.lang.Object-}
```
public SearchOptions(Object data)
```


يقوم بتهيئة نسخة جديدة من الفئة  SearchOptions  .


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | البيانات | java.lang.Object | البيانات المتسلسلة. |
|

### getUseSynonymSearch() {#getUseSynonymSearch--}
```
public boolean getUseSynonymSearch()
```


يحصل على علم استخدام المرادفات في البحث. القيمة الافتراضية هي  false .


**Returns:**
boolean - علم استخدام المرادفات في البحث.

### setUseSynonymSearch(boolean value) {#setUseSynonymSearch-boolean-}
```
public void setUseSynonymSearch(boolean value)
```


يحدد علم استخدام المرادفات في البحث. القيمة الافتراضية هي  false .


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | قيمة | boolean | علم استخدام المرادفات في البحث. |
|

### getUseHomophoneSearch() {#getUseHomophoneSearch--}
```
public boolean getUseHomophoneSearch()
```


يحصل على علم استخدام المتشابهات الصوتية في البحث. القيمة الافتراضية هي  false .


**Returns:**
boolean - علم استخدام المتشابهات الصوتية في البحث.

### setUseHomophoneSearch(boolean value) {#setUseHomophoneSearch-boolean-}
```
public void setUseHomophoneSearch(boolean value)
```


يحدد علم استخدام المتشابهات الصوتية في البحث. القيمة الافتراضية هي  false .


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | قيمة | boolean | علم استخدام المتشابهات الصوتية في البحث. |
|

### getUseWordFormsSearch() {#getUseWordFormsSearch--}
```
public boolean getUseWordFormsSearch()
```


يحصل على علم استخدام صيغ الكلمات المختلفة في البحث. القيمة الافتراضية هي  false .


**Returns:**
boolean - علم استخدام صيغ الكلمات المختلفة في البحث.

### setUseWordFormsSearch(boolean value) {#setUseWordFormsSearch-boolean-}
```
public void setUseWordFormsSearch(boolean value)
```


يحدد علم استخدام صيغ الكلمات المختلفة في البحث. القيمة الافتراضية هي  false .


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | قيمة | boolean | علم استخدام صيغ الكلمات المختلفة في البحث. |
|

### getRetrieveAttributes() {#getRetrieveAttributes--}
```
public boolean getRetrieveAttributes()
```


يحصل على علم استرجاع السمات المرتبطة بالمستندات التي تم العثور عليها. القيمة الافتراضية هي  false .


**Returns:**
boolean - علم استرجاع السمات المرتبطة بالمستندات التي تم العثور عليها.

### setRetrieveAttributes(boolean value) {#setRetrieveAttributes-boolean-}
```
public void setRetrieveAttributes(boolean value)
```


يحدد علم استرجاع السمات المرتبطة بالمستندات التي تم العثور عليها. القيمة الافتراضية هي  false .


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | قيمة | boolean | علم استرجاع السمات المرتبطة بالمستندات التي تم العثور عليها. |
|

### getFuzzySearch() {#getFuzzySearch--}
```
public FuzzySearchOptions getFuzzySearch()
```


يحصل على خيارات البحث الضبابي.


**Returns:**
[FuzzySearchOptions](../../com.groupdocs.search.options/fuzzysearchoptions) - The fuzzy search options.

### getSpellingCorrector() {#getSpellingCorrector--}
```
public SpellingCorrectorOptions getSpellingCorrector()
```


يحصل على خيارات مصحح الإملاء.


**Returns:**
[SpellingCorrectorOptions](../../com.groupdocs.search.options/spellingcorrectoroptions) - The spelling corrector options.

### getKeyboardLayoutCorrector() {#getKeyboardLayoutCorrector--}
```
public KeyboardLayoutCorrectorOptions getKeyboardLayoutCorrector()
```


يحصل على خيارات مصحح تخطيط لوحة المفاتيح.


**Returns:**
[KeyboardLayoutCorrectorOptions](../../com.groupdocs.search.options/keyboardlayoutcorrectoroptions) - The keyboard layout corrector options.

### getUseCaseSensitiveSearch() {#getUseCaseSensitiveSearch--}
```
public boolean getUseCaseSensitiveSearch()
```


يحصل على علم البحث حساس لحالة الأحرف. القيمة الافتراضية هي  false .


**Returns:**
boolean - علم البحث حساس لحالة الأحرف.

### setUseCaseSensitiveSearch(boolean value) {#setUseCaseSensitiveSearch-boolean-}
```
public void setUseCaseSensitiveSearch(boolean value)
```


يضبط علامة البحث حسّاس لحالة الأحرف. القيمة الافتراضية هي false .


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | قيمة | boolean | علامة البحث حسّاس لحالة الأحرف. |
|

### getMaxTotalOccurrenceCount() {#getMaxTotalOccurrenceCount--}
```
public int getMaxTotalOccurrenceCount()
```


يحصل على الحد الأقصى لإجمالي عدد التكرارات لجميع المصطلحات في استعلام البحث. القيمة الافتراضية هي 500000 .


**Returns:**
int - الحد الأقصى لإجمالي عدد التكرارات.

### setMaxTotalOccurrenceCount(int value) {#setMaxTotalOccurrenceCount-int-}
```
public void setMaxTotalOccurrenceCount(int value)
```


يضبط الحد الأقصى لإجمالي عدد التكرارات لجميع المصطلحات في استعلام البحث. القيمة الافتراضية هي 500000 .


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | قيمة | int | الحد الأقصى لإجمالي عدد التكرارات. |
|

### getMaxOccurrenceCountPerTerm() {#getMaxOccurrenceCountPerTerm--}
```
public int getMaxOccurrenceCountPerTerm()
```


يحصل على الحد الأقصى لعدد التكرارات لكل مصطلح في استعلام البحث. القيمة الافتراضية هي 100000 .


**Returns:**
int - الحد الأقصى لعدد التكرارات لكل مصطلح في استعلام البحث.

### setMaxOccurrenceCountPerTerm(int value) {#setMaxOccurrenceCountPerTerm-int-}
```
public void setMaxOccurrenceCountPerTerm(int value)
```


يضبط الحد الأقصى لعدد التكرارات لكل مصطلح في استعلام البحث. القيمة الافتراضية هي 100000 .


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | قيمة | int | الحد الأقصى لعدد التكرارات لكل مصطلح في استعلام البحث. |
|

### getDateFormats() {#getDateFormats--}
```
public DateFormatCollection getDateFormats()
```


يحصل على مجموعة صيغ التاريخ للبحث في نطاق التاريخ. صيغ التاريخ الافتراضية هي 'dd.MM.yyyy'، 'MM/dd/yyyy'، و'yyyy-MM-dd'.


**Returns:**
[DateFormatCollection](../../com.groupdocs.search.options/dateformatcollection) - The collection of date formats for date range search.


يوضح المثال كيفية ضبط صيغ التاريخ للبحث.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // إنشاء فهرس في المجلد المحدد
index.add(documentsFolder); // فهرسة المستندات من المجلد المحدد
SearchOptions options = new SearchOptions();
options.getDateFormats().clear(); // إزالة تنسيقات التاريخ الافتراضية
DateFormatElement[] elements = new DateFormatElement[] {
DateFormatElement.getMonthTwoDigits(),
DateFormatElement.getDayOfMonthTwoDigits(),
DateFormatElement.getYearFourDigits(),
};
// إنشاء نمط تنسيق تاريخ 'MM/dd/yyyy'
com.groupdocs.search.DateFormat dateFormat = new com.groupdocs.search.DateFormat(elements, "/");
options.getDateFormats().addItem(dateFormat);
SearchResult result = index.search(query, options); // بحث في الفهرس
 
```
 
````


### isChunkSearch() {#isChunkSearch--}
```
public boolean isChunkSearch()
```


يحصل على علامة البحث على أجزاء. القيمة الافتراضية هي false .


**Returns:**
boolean - علامة البحث على أجزاء.

### setChunkSearch(boolean value) {#setChunkSearch-boolean-}
```
public void setChunkSearch(boolean value)
```


يضبط علامة البحث على أجزاء. القيمة الافتراضية هي false .


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | قيمة | boolean | علامة البحث على أجزاء. |
|

### getSearchDocumentFilter() {#getSearchDocumentFilter--}
```
public ISearchDocumentFilter getSearchDocumentFilter()
```


يحصل على مرشح مستند البحث.  SearchDocumentFilter  يعمل وفق منطق الإدراج. استخدم فئة  SearchDocumentFilter  لإنشاء مثيلات مرشح مستند البحث. القيمة الافتراضية هي null ، مما يعني أنه سيتم إرجاع جميع المستندات التي تم العثور عليها.


**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - The search document filter.


يوضح المثال كيفية ضبط مرشح المستندات.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments1\\";
// إنشاء فهرس في المجلد المحدد
Index index = new Index(indexFolder);
// فهرسة المستندات
index.add(documentsFolder);
// إنشاء مرشح مستند بحث يتخطى المستندات ذات الامتدادات '.doc', '.docx', '.rtf'
SearchOptions options = new SearchOptions();
ISearchDocumentFilter fileExtensionFilter = SearchDocumentFilter.createFileExtension(".doc", ".docx", ".rtf"); // إنشاء مرشح امتداد الملف
ISearchDocumentFilter invertedFilter = SearchDocumentFilter.createNot(fileExtensionFilter); // عكس مرشح امتداد الملف
options.setSearchDocumentFilter(invertedFilter);
// البحث في الفهرس
SearchResult result = index.search("Einstein", options);
 
```
 
````


### setSearchDocumentFilter(ISearchDocumentFilter value) {#setSearchDocumentFilter-com.groupdocs.search.options.ISearchDocumentFilter-}
```
public void setSearchDocumentFilter(ISearchDocumentFilter value)
```


يضبط مرشح مستند البحث.  SearchDocumentFilter  يعمل وفق منطق الإدراج. استخدم فئة  SearchDocumentFilter  لإنشاء مثيلات مرشح مستند البحث. القيمة الافتراضية هي null ، مما يعني أنه سيتم إرجاع جميع المستندات التي تم العثور عليها.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | value | [ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) | مرشح مستند البحث. |


يوضح المثال كيفية ضبط مرشح المستندات.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments1\\";
// إنشاء فهرس في المجلد المحدد
Index index = new Index(indexFolder);
// فهرسة المستندات
index.add(documentsFolder);
// إنشاء مرشح مستند بحث يتخطى المستندات ذات الامتدادات '.doc', '.docx', '.rtf'
SearchOptions options = new SearchOptions();
ISearchDocumentFilter fileExtensionFilter = SearchDocumentFilter.createFileExtension(".doc", ".docx", ".rtf"); // إنشاء مرشح امتداد الملف
ISearchDocumentFilter invertedFilter = SearchDocumentFilter.createNot(fileExtensionFilter); // عكس مرشح امتداد الملف
options.setSearchDocumentFilter(invertedFilter);
// البحث في الفهرس
SearchResult result = index.search("Einstein", options);
 
```
 
````

|

### getCancellation() {#getCancellation--}
```
public Cancellation getCancellation()
```


يحصل على كائن إلغاء العملية. القيمة الافتراضية هي null.


**Returns:**
[Cancellation](../../com.groupdocs.search.common/cancellation) - The operation cancellation object.

### setCancellation(Cancellation value) {#setCancellation-com.groupdocs.search.common.Cancellation-}
```
public void setCancellation(Cancellation value)
```


يضبط كائن إلغاء العملية. القيمة الافتراضية هي null.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | value | [Cancellation](../../com.groupdocs.search.common/cancellation) | كائن إلغاء العملية. |
|

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
