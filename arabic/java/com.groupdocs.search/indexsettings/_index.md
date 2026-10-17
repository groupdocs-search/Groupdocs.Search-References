---
title: "IndexSettings"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يمثل إعدادات الفهرس التي تسمح بتخصيص عمليات الفهرسة."
type: docs
weight: 19
url: /ar/java/com.groupdocs.search/indexsettings/
---
**Inheritance:**
java.lang.Object
```
public class IndexSettings
```

يمثل إعدادات الفهرس التي تسمح بتخصيص عمليات الفهرسة.


**Learn more**

* [Search index settings](../https://docs.groupdocs.com/display/searchjava/Search+index+settings)


المثال يوضح استخدامًا نموذجيًا للفئة.

````
 ```

String indexFolder = "c:\\MyIndex\\";
IndexSettings settings = new IndexSettings();
settings.setIndexType(IndexType.CompactIndex); // ضبط نوع الفهرس
Index index = new Index(indexFolder, settings); // إنشاء فهرس
 
```
 
````


## المنشئات

| منشئ | الوصف |
| --- | --- |
|  | [IndexSettings()](#IndexSettings--) | يقوم بتهيئة نسخة جديدة من الفئة IndexSettings. |
|
## طرق

| طريقة | الوصف |
| --- | --- |
|  | [getInMemoryIndex()](#getInMemoryIndex--) | يحصل على قيمة تشير إلى ما إذا كان الفهرس مخزنًا في الذاكرة أم على القرص. |
|
|  | [getUseStopWords()](#getUseStopWords--) | يحصل على قيمة تشير إلى ما إذا كان سيتم استخدام كلمات التوقف أم لا. |
|
|  | [setUseStopWords(boolean value)](#setUseStopWords-boolean-) | يضبط قيمة تشير إلى ما إذا كان سيتم استخدام كلمات التوقف أم لا. |
|
|  | [getMaxIndexingReportCount()](#getMaxIndexingReportCount--) | يحصل على الحد الأقصى لعدد تقارير الفهرسة. |
|
|  | [setMaxIndexingReportCount(int value)](#setMaxIndexingReportCount-int-) | يضبط الحد الأقصى لعدد تقارير الفهرسة. |
|
|  | [getMaxSearchReportCount()](#getMaxSearchReportCount--) | يحصل على الحد الأقصى لعدد تقارير البحث. |
|
|  | [setMaxSearchReportCount(int value)](#setMaxSearchReportCount-int-) | يضبط الحد الأقصى لعدد تقارير البحث. |
|
|  | [getUseCharacterReplacements()](#getUseCharacterReplacements--) | يحصل على قيمة تشير إلى ما إذا كان سيتم استخدام استبدالات الأحرف أم لا. |
|
|  | [setUseCharacterReplacements(boolean value)](#setUseCharacterReplacements-boolean-) | يضبط قيمة تشير إلى ما إذا كان سيتم استخدام استبدالات الأحرف أم لا. |
|
|  | [getDocumentFilter()](#getDocumentFilter--) | يحصل على مرشح المستند. |
|
|  | [setDocumentFilter(DocumentFilter value)](#setDocumentFilter-com.groupdocs.search.DocumentFilter-) | يضبط مرشح المستند. |
|
|  | [getTextStorageSettings()](#getTextStorageSettings--) | يحصل على إعدادات تخزين النص. |
|
|  | [setTextStorageSettings(TextStorageSettings value)](#setTextStorageSettings-com.groupdocs.search.options.TextStorageSettings-) | يضبط إعدادات تخزين النص. |
|
|  | [getIndexType()](#getIndexType--) | يحصل على نوع الفهرس. |
|
|  | [setIndexType(IndexType value)](#setIndexType-com.groupdocs.search.options.IndexType-) | يضبط نوع الفهرس. |
|
|  | [getSearchThreads()](#getSearchThreads--) | يحصل على عدد الخيوط المستخدمة في البحث. |
|
|  | [setSearchThreads(NumberOfThreads value)](#setSearchThreads-com.groupdocs.search.options.NumberOfThreads-) | يضبط عدد الخيوط المستخدمة في البحث. |
|
|  | [getCustomExtractors()](#getCustomExtractors--) | يحصل على مجموعة المستخرج المخصصة. |
|
|  | [getLogger()](#getLogger--) | يحصل على مسجل يُستخدم لتسجيل الأحداث والأخطاء في الفهرس. |
|
|  | [setLogger(ILogger value)](#setLogger-com.groupdocs.search.common.ILogger-) | يضبط مسجل يُستخدم لتسجيل الأحداث والأخطاء في الفهرس. |
|
### IndexSettings() {#IndexSettings--}
```
public IndexSettings()
```


يقوم بتهيئة نسخة جديدة من الفئة IndexSettings.


### getInMemoryIndex() {#getInMemoryIndex--}
```
public final boolean getInMemoryIndex()
```


يحصل على قيمة تشير إلى ما إذا كان الفهرس مخزنًا في الذاكرة أم على القرص.


**Returns:**
boolean - قيمة تشير إلى ما إذا كان الفهرس مخزنًا في الذاكرة أم على القرص.

### getUseStopWords() {#getUseStopWords--}
```
public final boolean getUseStopWords()
```


يحصل على قيمة تشير إلى ما إذا كان سيتم استخدام كلمات التوقف أم لا. القيمة الافتراضية هي  true .


**Returns:**
boolean - قيمة تشير إلى ما إذا كان سيتم استخدام كلمات التوقف أم لا.

### setUseStopWords(boolean value) {#setUseStopWords-boolean-}
```
public final void setUseStopWords(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان سيتم استخدام كلمات التوقف أم لا. القيمة الافتراضية هي  true .


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | قيمة | boolean | قيمة تشير إلى ما إذا كان سيتم استخدام كلمات التوقف أم لا. |
|

### getMaxIndexingReportCount() {#getMaxIndexingReportCount--}
```
public final int getMaxIndexingReportCount()
```


يحصل على الحد الأقصى لعدد تقارير الفهرسة. القيمة الافتراضية هي  5 .


**Returns:**
int - الحد الأقصى لعدد تقارير الفهرسة.

### setMaxIndexingReportCount(int value) {#setMaxIndexingReportCount-int-}
```
public final void setMaxIndexingReportCount(int value)
```


يضبط الحد الأقصى لعدد تقارير الفهرسة. القيمة الافتراضية هي  5 .


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | قيمة | int | الحد الأقصى لعدد تقارير الفهرسة. |
|

### getMaxSearchReportCount() {#getMaxSearchReportCount--}
```
public final int getMaxSearchReportCount()
```


يحصل على الحد الأقصى لعدد تقارير البحث. القيمة الافتراضية هي  10 .


**Returns:**
int - الحد الأقصى لعدد تقارير البحث.

### setMaxSearchReportCount(int value) {#setMaxSearchReportCount-int-}
```
public final void setMaxSearchReportCount(int value)
```


يضبط الحد الأقصى لعدد تقارير البحث. القيمة الافتراضية هي  10 .


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | قيمة | int | الحد الأقصى لعدد تقارير البحث. |
|

### getUseCharacterReplacements() {#getUseCharacterReplacements--}
```
public final boolean getUseCharacterReplacements()
```


يحصل على قيمة تشير إلى ما إذا كان سيتم استخدام استبدالات الأحرف أم لا. القيمة الافتراضية هي  false .


**Returns:**
boolean - قيمة تشير إلى ما إذا كان سيتم استخدام استبدالات الأحرف أم لا.

### setUseCharacterReplacements(boolean value) {#setUseCharacterReplacements-boolean-}
```
public final void setUseCharacterReplacements(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان سيتم استخدام استبدالات الأحرف أم لا. القيمة الافتراضية هي  false .


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | قيمة | boolean | قيمة تشير إلى ما إذا كان سيتم استخدام استبدالات الأحرف أم لا. |
|

### getDocumentFilter() {#getDocumentFilter--}
```
public final DocumentFilter getDocumentFilter()
```


يحصل على مرشح المستندات. الـ  DocumentFilter  يعمل وفق منطق الشمول. استخدم فئة  DocumentFilter  لإنشاء مثيل مرشح المستندات. القيمة الافتراضية هي  null , مما يعني أن جميع المستندات المضافة يتم فهرستها.


**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - The document filter.

يوضح المثال كيفية ضبط مرشح المستندات.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// إنشاء مرشح يتخطى المستندات ذات الامتدادات '.doc', '.docx', '.rtf'
IndexSettings settings = new IndexSettings();
DocumentFilter fileExtensionFilter = DocumentFilter.createFileExtension(".doc", ".docx", ".rtf"); // إنشاء مرشح امتداد الملف
DocumentFilter invertedFilter = DocumentFilter.createNot(fileExtensionFilter); // عكس مرشح امتداد الملف
settings.setDocumentFilter(invertedFilter);
// إنشاء فهرس في المجلد المحدد
Index index = new Index(indexFolder, settings);
// فهرسة المستندات
index.add(documentsFolder);
// البحث
SearchResult result = index.search("Einstein");
 
```
 
````


### setDocumentFilter(DocumentFilter value) {#setDocumentFilter-com.groupdocs.search.DocumentFilter-}
```
public final void setDocumentFilter(DocumentFilter value)
```


يضبط مرشح المستندات. الـ  DocumentFilter  يعمل وفق منطق الشمول. استخدم فئة  GroupDocs.Search.Options.DocumentFilter  لإنشاء مثيلات مرشح المستندات. القيمة الافتراضية هي  null ، مما يعني أن جميع المستندات المضافة يتم فهرستها.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | value | [DocumentFilter](../../com.groupdocs.search/documentfilter) | مرشح المستند. |

يوضح المثال كيفية ضبط مرشح المستندات.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// إنشاء مرشح يتخطى المستندات ذات الامتدادات '.doc', '.docx', '.rtf'
IndexSettings settings = new IndexSettings();
DocumentFilter fileExtensionFilter = DocumentFilter.createFileExtension(".doc", ".docx", ".rtf"); // إنشاء مرشح امتداد الملف
DocumentFilter invertedFilter = DocumentFilter.createNot(fileExtensionFilter); // عكس مرشح امتداد الملف
settings.setDocumentFilter(invertedFilter);
// إنشاء فهرس في المجلد المحدد
Index index = new Index(indexFolder, settings);
// فهرسة المستندات
index.add(documentsFolder);
// البحث
SearchResult result = index.search("Einstein");
 
```
 
````

|

### getTextStorageSettings() {#getTextStorageSettings--}
```
public final TextStorageSettings getTextStorageSettings()
```


يحصل على إعدادات تخزين النص. القيمة الافتراضية هي  null ، مما يعني أن نصوص المستندات غير مخزنة.


**Returns:**
[TextStorageSettings](../../com.groupdocs.search.options/textstoragesettings) - The text storage settings.

يوضح المثال كيفية ضبط إعدادات تخزين النص.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// إنشاء مثيل إعدادات الفهرس
IndexSettings settings = new IndexSettings();
settings.setTextStorageSettings(new TextStorageSettings(Compression.High)); // ضبط مستوى ضغط عالي لتخزين نص الفهرس
// إنشاء فهرس في المجلد المحدد
Index index = new Index(indexFolder, settings);
// فهرسة المستندات
index.add(documentsFolder);
// البحث
SearchResult result = index.search("Einstein");
 
```
 
````


### setTextStorageSettings(TextStorageSettings value) {#setTextStorageSettings-com.groupdocs.search.options.TextStorageSettings-}
```
public final void setTextStorageSettings(TextStorageSettings value)
```


يضبط إعدادات تخزين النص. القيمة الافتراضية هي  null ، مما يعني أن نصوص المستندات غير مخزنة.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | value | [TextStorageSettings](../../com.groupdocs.search.options/textstoragesettings) | إعدادات تخزين النص. |

يوضح المثال كيفية ضبط إعدادات تخزين النص.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// إنشاء مثيل إعدادات الفهرس
IndexSettings settings = new IndexSettings();
settings.setTextStorageSettings(new TextStorageSettings(Compression.High)); // ضبط مستوى ضغط عالي لتخزين نص الفهرس
// إنشاء فهرس في المجلد المحدد
Index index = new Index(indexFolder, settings);
// فهرسة المستندات
index.add(documentsFolder);
// البحث
SearchResult result = index.search("Einstein");
 
```
 
````

|

### getIndexType() {#getIndexType--}
```
public final IndexType getIndexType()
```


يحصل على نوع الفهرس. القيمة الافتراضية هي  GroupDocs.Search.Options.IndexType.NormalIndex .


**Returns:**
[IndexType](../../com.groupdocs.search.options/indextype) - The index type.

### setIndexType(IndexType value) {#setIndexType-com.groupdocs.search.options.IndexType-}
```
public final void setIndexType(IndexType value)
```


يضبط نوع الفهرس. القيمة الافتراضية هي  GroupDocs.Search.Options.IndexType.NormalIndex .


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | value | [IndexType](../../com.groupdocs.search.options/indextype) | نوع الفهرس. |
|

### getSearchThreads() {#getSearchThreads--}
```
public final NumberOfThreads getSearchThreads()
```


يحصل على عدد الخيوط المستخدمة في البحث. القيمة الافتراضية هي  GroupDocs.Search.Options.NumberOfThreads.Default ، مما يعني أن البحث سيُجرى باستخدام عدد الخيوط المساوي لعدد نوى المعالج.


**Returns:**
[NumberOfThreads](../../com.groupdocs.search.options/numberofthreads) - The number of threads used for the search.

### setSearchThreads(NumberOfThreads value) {#setSearchThreads-com.groupdocs.search.options.NumberOfThreads-}
```
public final void setSearchThreads(NumberOfThreads value)
```


يضبط عدد الخيوط المستخدمة في البحث. القيمة الافتراضية هي  GroupDocs.Search.Options.NumberOfThreads.Default ، مما يعني أن البحث سيُجرى باستخدام عدد الخيوط المساوي لعدد نوى المعالج.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | value | [NumberOfThreads](../../com.groupdocs.search.options/numberofthreads) | عدد الخيوط المستخدمة في البحث. |
|

### getCustomExtractors() {#getCustomExtractors--}
```
public final CustomExtractorCollection getCustomExtractors()
```


يحصل على مجموعة المستخرج المخصص. المثال الكامل لتطبيق مستخرج مخصص مُقدم في وثائق الواجهة  GroupDocs.Search.Common.IFieldExtractor .


**Returns:**
[CustomExtractorCollection](../../com.groupdocs.search.common/customextractorcollection) - The custom extractor collection.

### getLogger() {#getLogger--}
```
public final ILogger getLogger()
```


يحصل على مسجل يُستخدم لتسجيل الأحداث والأخطاء في الفهرس. لاحظ أن المسجل غير محفوظ ويجب إنشاؤه وتعيينه في كل مرة يتم فيها إنشاء أو تحميل الفهرس.


**Returns:**
[ILogger](../../com.groupdocs.search.common/ilogger) - A logger that is used for logging events and errors in the index.

### setLogger(ILogger value) {#setLogger-com.groupdocs.search.common.ILogger-}
```
public final void setLogger(ILogger value)
```


يضبط مسجل يُستخدم لتسجيل الأحداث والأخطاء في الفهرس. لاحظ أن المسجل غير محفوظ ويجب إنشاؤه وتعيينه في كل مرة يتم فيها إنشاء أو تحميل الفهرس.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | value | [ILogger](../../com.groupdocs.search.common/ilogger) | مسجل يُستخدم لتسجيل الأحداث والأخطاء في الفهرس. |
|

