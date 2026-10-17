---
title: "فهرس"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يمثل الفئة الرئيسية لفهرسة المستندات والبحث فيها."
type: docs
weight: 17
url: /ar/java/com.groupdocs.search/index/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.io.Closeable
```
public class Index implements Closeable
```

يمثل الفئة الرئيسية لفهرسة المستندات والبحث فيها.


**Learn more**

* [Creating an index](../https://docs.groupdocs.com/display/searchjava/Creating+an+index)
* [Indexing](../https://docs.groupdocs.com/display/searchjava/Indexing)
* [Searching](../https://docs.groupdocs.com/display/searchjava/Searching)


المثال يوضح استخدامًا نموذجيًا للفئة.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // إنشاء فهرس في المجلد المحدد
index.add(documentsFolder); // فهرسة المستندات من المجلد المحدد
SearchResult result = index.search(query); // البحث في الفهرس
 
```
 
````


## المنشئات

| منشئ | الوصف |
| --- | --- |
|  | [Index()](#Index--) | ينشئ مثيلاً جديداً من الفئة  Index  في الذاكرة. |
|
|  | [Index(IndexSettings settings)](#Index-com.groupdocs.search.IndexSettings-) | ينشئ مثيلاً جديداً من الفئة  Index  في الذاكرة مع إعدادات فهرس معينة. |
|
|  | [Index(String indexFolder)](#Index-java.lang.String-) | ينشئ مثيلاً جديداً من الفئة  Index . |
|
|  | [Index(String indexFolder, IndexSettings settings)](#Index-java.lang.String-com.groupdocs.search.IndexSettings-) | يُنشئ مثيلاً جديدًا لـ |
فهرس
الفئة.
|
|  | [Index(String indexFolder, boolean overwriteIfExists)](#Index-java.lang.String-boolean-) | يُنشئ مثيلاً جديدًا لـ |
فهرس
الفئة.
|
|  | [Index(String indexFolder, IndexSettings settings, boolean overwriteIfExists)](#Index-java.lang.String-com.groupdocs.search.IndexSettings-boolean-) | يُنشئ مثيلاً جديدًا لـ |
فهرس
الفئة.
|
## طرق

| طريقة | الوصف |
| --- | --- |
|  | [getEvents()](#getEvents--) | يحصل على مركز الأحداث للاشتراك في الأحداث. |
|
|  | [getIndexInfo()](#getIndexInfo--) | يحصل على المعلومات الأساسية حول الفهرس. |
|
|  | [getRepository()](#getRepository--) | يحصل على كائن مستودع الفهرس إذا كان الفهرس موجودًا فيه. |
|
|  | [getIndexSettings()](#getIndexSettings--) | يحصل على إعدادات الفهرس. |
|
|  | [getDictionaries()](#getDictionaries--) | يحصل على مستودع القاموس. |
|
|  | [close()](#close--) | يطلق جميع الموارد المستخدمة بواسطة |
فهرس
.
|
|  | [add(String path)](#add-java.lang.String-) | ينفذ عملية الفهرسة. |
|
|  | [add(String path, IndexingOptions options)](#add-java.lang.String-com.groupdocs.search.options.IndexingOptions-) | ينفذ عملية الفهرسة. |
|
|  | [add(String[] paths)](#add-java.lang.String---) | ينفذ عملية الفهرسة. |
|
|  | [add(String[] paths, IndexingOptions options)](#add-java.lang.String---com.groupdocs.search.options.IndexingOptions-) | ينفذ عملية الفهرسة. |
|
|  | [add(Document[] documents, IndexingOptions options)](#add-com.groupdocs.search.Document---com.groupdocs.search.options.IndexingOptions-) | ينفذ عملية الفهرسة. |
|
|  | [add(ExtractedData[] data, IndexingOptions options)](#add-com.groupdocs.search.ExtractedData---com.groupdocs.search.options.IndexingOptions-) | ينفذ عملية الفهرسة. |
|
|  | [update()](#update--) | يعيد فهرسة المستندات التي تم تغييرها أو حذفها منذ آخر تحديث. |
|
|  | [update(UpdateOptions options)](#update-com.groupdocs.search.options.UpdateOptions-) | يعيد فهرسة المستندات التي تم تغييرها أو حذفها منذ آخر تحديث. |
|
|  | [getIndexingReports()](#getIndexingReports--) | يحصل على التقارير حول عمليات الفهرسة. |
|
|  | [getSearchReports()](#getSearchReports--) | يحصل على التقارير حول عمليات البحث. |
|
|  | [search(String query)](#search-java.lang.String-) | يبحث في الفهرس. |
|
|  | [search(String query, SearchOptions options)](#search-java.lang.String-com.groupdocs.search.options.SearchOptions-) | يبحث في الفهرس. |
|
|  | [search(SearchQuery query)](#search-com.groupdocs.search.SearchQuery-) | يبحث في الفهرس. |
|
|  | [search(SearchQuery query, SearchOptions options)](#search-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-) | يبحث في الفهرس. |
|
|  | [search(SearchImage image, ImageSearchOptions options)](#search-com.groupdocs.search.common.SearchImage-com.groupdocs.search.options.ImageSearchOptions-) | ينفذ بحث صورة عكسي في الفهرس. |
|
|  | [searchNext(ChunkSearchToken chunkSearchToken)](#searchNext-com.groupdocs.search.common.ChunkSearchToken-) | يكمل بحث الجزء الذي بدأ بطريقة Search. |
|
|  | [searchNext(ChunkSearchToken chunkSearchToken, Cancellation cancellation)](#searchNext-com.groupdocs.search.common.ChunkSearchToken-com.groupdocs.search.common.Cancellation-) | يكمل بحث الجزء الذي بدأ بطريقة Search. |
|
|  | [optimize()](#optimize--) | يقلل عدد مقاطع الفهرس بدمجها واحدة مع الأخرى. |
|
|  | [optimize(MergeOptions options)](#optimize-com.groupdocs.search.options.MergeOptions-) | يقلل عدد مقاطع الفهرس بدمجها واحدة مع الأخرى. |
|
|  | [merge(Index index, MergeOptions options)](#merge-com.groupdocs.search.Index-com.groupdocs.search.options.MergeOptions-) | يدمج الفهرس المحدد في الفهرس الحالي. |
|
|  | [merge(IndexRepository repository, MergeOptions options)](#merge-com.groupdocs.search.IndexRepository-com.groupdocs.search.options.MergeOptions-) | يدمج الفهارس من مستودع الفهرس المحدد إلى الفهرس الحالي. |
|
|  | [highlight(FoundDocument document, Highlighter highlighter)](#highlight-com.groupdocs.search.results.FoundDocument-com.groupdocs.search.highlighters.Highlighter-) | ينشئ نصًا بتنسيق HTML مع تسليط الضوء على المصطلحات التي تم العثور عليها. |
|
|  | [highlight(FoundDocument document, Highlighter highlighter, HighlightOptions options)](#highlight-com.groupdocs.search.results.FoundDocument-com.groupdocs.search.highlighters.Highlighter-com.groupdocs.search.options.HighlightOptions-) | ينشئ نصًا بتنسيق HTML مع تسليط الضوء على المصطلحات التي تم العثور عليها. |
|
|  | [getIndexedDocuments()](#getIndexedDocuments--) | يحصل على مصفوفة من جميع المستندات المفهرسة. |
|
|  | [getIndexedDocumentItems(DocumentInfo documentInfo)](#getIndexedDocumentItems-com.groupdocs.search.results.DocumentInfo-) | يحصل على مصفوفة من عناصر المستند. |
|
|  | [GetIndexedDocument(String documentKey)](#GetIndexedDocument-java.lang.String-) | يحصل على مستند مفهرس بواسطة مفتاح المستند. |
|
|  | [getDocumentText(DocumentInfo documentInfo, OutputAdapter adapter)](#getDocumentText-com.groupdocs.search.results.DocumentInfo-com.groupdocs.search.common.OutputAdapter-) | ينشئ نص المستند المفهرس ويمرره عبر محول الإخراج. |
|
|  | [getDocumentText(DocumentInfo documentInfo, OutputAdapter adapter, TextOptions options)](#getDocumentText-com.groupdocs.search.results.DocumentInfo-com.groupdocs.search.common.OutputAdapter-com.groupdocs.search.options.TextOptions-) | ينشئ نصًا بتنسيق HTML للمستند المفهرس وينقله عبر محول الإخراج. |
|
|  | [getIndexedPaths()](#getIndexedPaths--) | يحصل على مصفوفة من المسارات المفهرسة - مستندات أو مجلدات. |
|
|  | [delete(String[] paths, UpdateOptions options)](#delete-java.lang.String---com.groupdocs.search.options.UpdateOptions-) | يحذف الملفات أو المجلدات المفهرسة من الفهرس. |
|
|  | [delete(UpdateOptions options, String[] documentKeys)](#delete-com.groupdocs.search.options.UpdateOptions-java.lang.String---) | يحذف المستندات المفهرسة من التدفقات أو البنى. |
|
|  | [notifyIndex(Notification notification)](#notifyIndex-com.groupdocs.search.Notification-) | يمرر كائن الإشعار المحدد إلى الفهرس لتنفيذ الإشعار. |
|
|  | [changeAttributes(AttributeChangeBatch batch)](#changeAttributes-com.groupdocs.search.common.AttributeChangeBatch-) | يطبق دفعة التغييرات على السمات المحددة على المستندات المفهرسة دون إعادة الفهرسة أثناء عملية التحديث. |
|
|  | [getAttributes(String path)](#getAttributes-java.lang.String-) | يحصل على جميع السمات المرتبطة بالمستند المفهرس المحدد. |
|
|  | [loadIntoMemoryCompletely(String indexFolder)](#loadIntoMemoryCompletely-java.lang.String-) | يقوم بتحميل الفهرس بالكامل إلى الذاكرة. |
|
|  | [loadIntoMemoryCompletely(String indexFolder, IndexSettings settings)](#loadIntoMemoryCompletely-java.lang.String-com.groupdocs.search.IndexSettings-) | يقوم بتحميل الفهرس بالكامل إلى الذاكرة. |
|
### Index() {#Index--}
```
public Index()
```


ينشئ مثيلاً جديداً من الفئة  Index  في الذاكرة.


يوضح المثال كيفية إنشاء فهرس في الذاكرة دون حفظ الملفات على القرص.

````
 ```

Index index = new Index();
 
```
 
````



### Index(IndexSettings settings) {#Index-com.groupdocs.search.IndexSettings-}
```
public Index(IndexSettings settings)
```


ينشئ مثيلاً جديداً من الفئة  Index  في الذاكرة مع إعدادات فهرس معينة.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | كائن إعدادات الفهرس. |


يوضح المثال كيفية إنشاء فهرس في الذاكرة دون حفظ الملفات على القرص باستخدام إعدادات فهرس معينة.

````
 ```

IndexSettings settings = new IndexSettings();
settings.setIndexType(IndexType.CompactIndex);
Index index = new Index(settings);
 
```
 
````

|

### Index(String indexFolder) {#Index-java.lang.String-}
```
public Index(String indexFolder)
```


يُهيئ نسخة جديدة من الفئة Index. ينشئ فهرسًا جديدًا أو يفتح فهرسًا موجودًا على القرص.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | indexFolder | java.lang.String | مسار مجلد الفهرس. |


يوضح المثال كيفية إنشاء فهرس على القرص أو فتح فهرس موجود.

````
 ```

String indexFolder = "c:\\MyIndex\\";
Index index = new Index(indexFolder);
 
```
 
````

|

### Index(String indexFolder, IndexSettings settings) {#Index-java.lang.String-com.groupdocs.search.IndexSettings-}
```
public Index(String indexFolder, IndexSettings settings)
```


يُنشئ مثيلاً جديدًا لـ
فهرس
الفئة.
ينشئ فهرسًا جديدًا بإعدادات معينة أو يفتح فهرسًا موجودًا على القرص.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | indexFolder | java.lang.String | مسار مجلد الفهرس. |
|
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | كائن إعدادات الفهرس. |

يوضح المثال كيفية إنشاء فهرس على القرص بإعدادات فهرس معينة.

````
 ```

String indexFolder = "c:\\MyIndex\\";
IndexSettings settings = new IndexSettings();
settings.setIndexType(IndexType.CompactIndex);
Index index = new Index(indexFolder, settings);
 
```
 
````

|

### Index(String indexFolder, boolean overwriteIfExists) {#Index-java.lang.String-boolean-}
```
public Index(String indexFolder, boolean overwriteIfExists)
```


يُنشئ مثيلاً جديدًا لـ
فهرس
الفئة.
يقوم بتحميل فهرس موجود من القرص إذا
overwriteIfExists
هو
false
;
ينشئ فهرسًا جديدًا على القرص وإلا.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | indexFolder | java.lang.String | مسار مجلد الفهرس. |
|
|  | overwriteIfExists | boolean | علامة استبدال مجلد الفهرس. |

يوضح المثال كيفية إنشاء فهرس جديد في مجلد يحتوي بالفعل على فهرس آخر.

````
 ```

String indexFolder = "c:\\MyIndex\\";
Index index = new Index(indexFolder, true);
 
```
 
````

|

### Index(String indexFolder, IndexSettings settings, boolean overwriteIfExists) {#Index-java.lang.String-com.groupdocs.search.IndexSettings-boolean-}
```
public Index(String indexFolder, IndexSettings settings, boolean overwriteIfExists)
```


يُنشئ مثيلاً جديدًا لـ
فهرس
الفئة.
يقوم بتحميل فهرس موجود من القرص إذا
overwriteIfExists
هو
false
;
ينشئ فهرسًا جديدًا على القرص بإعدادات فهرس معينة وإلا.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | indexFolder | java.lang.String | مسار مجلد الفهرس. |
|
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | كائن إعدادات الفهرس. |
|
|  | overwriteIfExists | boolean | علامة استبدال مجلد الفهرس. |

يوضح المثال كيفية إنشاء فهرس على القرص بإعدادات فهرس معينة.

````
 ```

String indexFolder = "c:\\MyIndex\\";
IndexSettings settings = new IndexSettings();
settings.setIndexType(IndexType.CompactIndex);
Index index = new Index(indexFolder, settings, true);
 
```
 
````

|

### getEvents() {#getEvents--}
```
public final EventHub getEvents()
```


يحصل على مركز الأحداث للاشتراك في الأحداث.


**Returns:**
[EventHub](../../com.groupdocs.search.events/eventhub) - The event hub for subscribing to events.

### getIndexInfo() {#getIndexInfo--}
```
public final IndexInfo getIndexInfo()
```


يحصل على المعلومات الأساسية حول الفهرس.


**Returns:**
[IndexInfo](../../com.groupdocs.search.common/indexinfo) - The basic information on the index.

### getRepository() {#getRepository--}
```
public final IndexRepository getRepository()
```


يحصل على كائن مستودع الفهرس إذا كان الفهرس موجودًا فيه.


**Returns:**
[IndexRepository](../../com.groupdocs.search/indexrepository) - The index repository object.

### getIndexSettings() {#getIndexSettings--}
```
public final IndexSettings getIndexSettings()
```


يحصل على إعدادات الفهرس.


**Returns:**
[IndexSettings](../../com.groupdocs.search/indexsettings) - The index settings.

### getDictionaries() {#getDictionaries--}
```
public final DictionaryRepository getDictionaries()
```


يحصل على مستودع القاموس.


**Returns:**
[DictionaryRepository](../../com.groupdocs.search.dictionaries/dictionaryrepository) - The dictionary repository.

### close() {#close--}
```
public final void close()
```


يطلق جميع الموارد المستخدمة بواسطة
فهرس
.


### add(String path) {#add-java.lang.String-}
```
public final void add(String path)
```


ينفذ عملية الفهرسة.
يضيف ملفًا أو مجلدًا بمسار مطلق أو نسبي.
ستتم فهرسة المستندات من جميع المجلدات الفرعية.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | path | java.lang.String | المسار إلى ملف أو مجلد ليتم فهرسته. |

يوضح المثال كيفية إضافة مستندات إلى فهرس.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String folderPath = "c:\\MyDocuments\\";
String filePath = "c:\\Documents\\MyFile.txt";
Index index = new Index(indexFolder); // إنشاء فهرس في المجلد المحدد
index.add(folderPath); // فهرسة المستندات في المجلد المحدد
index.add(filePath); // فهرسة المستند المحدد
 
```
 
````

|

### add(String path, IndexingOptions options) {#add-java.lang.String-com.groupdocs.search.options.IndexingOptions-}
```
public final void add(String path, IndexingOptions options)
```


ينفذ عملية الفهرسة.
يضيف ملفًا أو مجلدًا بمسار مطلق أو نسبي.
ستتم فهرسة المستندات من جميع المجلدات الفرعية.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | path | java.lang.String | المسار إلى ملف أو مجلد ليتم فهرسته. |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | خيارات الفهرسة. |

يوضح المثال كيفية إضافة مستندات إلى فهرس مع خيارات فهرسة معينة.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String folderPath = "c:\\MyDocuments\\";
String filePath = "c:\\Documents\\MyFile.txt";
Index index = new Index(indexFolder); // إنشاء فهرس في المجلد المحدد
IndexingOptions options = new IndexingOptions();
options.setThreads(2); // ضبط عدد خيوط الفهرسة
index.add(folderPath, options); // فهرسة المستندات في المجلد المحدد
index.add(filePath, options); // فهرسة المستند المحدد
 
```
 
````

|

### add(String[] paths) {#add-java.lang.String---}
```
public final void add(String[] paths)
```


ينفذ عملية الفهرسة.
يضيف ملفات أو مجلدات باستخدام مسار مطلق أو نسبي.
ستتم فهرسة المستندات من جميع المجلدات الفرعية.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | المسارات | java.lang.String[] | المسارات إلى الملفات أو المجلدات التي سيتم فهرستها. |

يوضح المثال كيفية إضافة مستندات إلى فهرس.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String folderPath = "c:\\MyDocuments\\";
String filePath = "c:\\Documents\\MyFile.txt";
Index index = new Index(indexFolder); // إنشاء فهرس في المجلد المحدد
String[] paths = new String[] { folderPath, filePath };
index.add(paths); // فهرسة المستندات في المسارات المحددة
 
```
 
````

|

### add(String[] paths, IndexingOptions options) {#add-java.lang.String---com.groupdocs.search.options.IndexingOptions-}
```
public final void add(String[] paths, IndexingOptions options)
```


ينفذ عملية الفهرسة.
يضيف ملفات أو مجلدات باستخدام مسار مطلق أو نسبي.
ستتم فهرسة المستندات من جميع المجلدات الفرعية.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | المسارات | java.lang.String[] | المسارات إلى الملفات أو المجلدات التي سيتم فهرستها. |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | خيارات الفهرسة. |

يوضح المثال كيفية إضافة مستندات إلى فهرس مع خيارات فهرسة معينة.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String folderPath = "c:\\MyDocuments\\";
String filePath = "c:\\Documents\\MyFile.txt";
Index index = new Index(indexFolder); // إنشاء فهرس في المجلد المحدد
IndexingOptions options = new IndexingOptions();
options.setThreads(2); // ضبط عدد خيوط الفهرسة
String[] paths = new String[] { folderPath, filePath };
index.add(paths, options); // فهرسة المستندات في المسارات المحددة
 
```
 
````

|

### add(Document[] documents, IndexingOptions options) {#add-com.groupdocs.search.Document---com.groupdocs.search.options.IndexingOptions-}
```
public final void add(Document[] documents, IndexingOptions options)
```


ينفذ عملية الفهرسة.
يضيف مستندات من نظام الملفات أو التدفق أو الهيكل.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | documents | [Document\[\]](../../com.groupdocs.search/document) | المستندات من نظام الملفات أو التدفق أو الهيكل. |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | خيارات الفهرسة. |
|

### add(ExtractedData[] data, IndexingOptions options) {#add-com.groupdocs.search.ExtractedData---com.groupdocs.search.options.IndexingOptions-}
```
public final void add(ExtractedData[] data, IndexingOptions options)
```


ينفذ عملية الفهرسة.
يضيف البيانات المستخرجة إلى الفهرس.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | data | [ExtractedData\[\]](../../com.groupdocs.search/extracteddata) | البيانات المستخرجة. |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | خيارات الفهرسة. |
|

### update() {#update--}
```
public final void update()
```


يعيد فهرسة المستندات التي تم تغييرها أو حذفها منذ آخر تحديث.
يضيف ملفات جديدة تم إضافتها إلى المجلدات المفهرسة.

يوضح المثال كيفية تحديث فهرس.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // إنشاء فهرس في المجلد المحدد
index.add(documentsFolder); // فهرسة المستندات من المجلد المحدد
// حذف المستندات من مجلد المستندات أو تعديلها أو إضافة مستندات جديدة إلى المجلد
index.update(); // تحديث الفهرس
 
```
 
````



### update(UpdateOptions options) {#update-com.groupdocs.search.options.UpdateOptions-}
```
public final void update(UpdateOptions options)
```


يعيد فهرسة المستندات التي تم تغييرها أو حذفها منذ آخر تحديث.
يضيف ملفات جديدة تم إضافتها إلى المجلدات المفهرسة.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | options | [UpdateOptions](../../com.groupdocs.search.options/updateoptions) | خيارات التحديث. |

يوضح المثال كيفية تحديث فهرس باستخدام خيارات تحديث معينة.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // إنشاء فهرس في المجلد المحدد
index.add(documentsFolder); // فهرسة المستندات من المجلد المحدد
// حذف المستندات من مجلد المستندات أو تعديلها أو إضافة مستندات جديدة إلى المجلد
UpdateOptions options = new UpdateOptions();
options.setThreads(2); // ضبط عدد خيوط الفهرسة
index.update(options); // تحديث الفهرس
 
```
 
````

|

### getIndexingReports() {#getIndexingReports--}
```
public final IndexingReport[] getIndexingReports()
```


يحصل على التقارير حول عمليات الفهرسة.


**Returns:**
com.groupdocs.search.common.IndexingReport[] - تقارير الفهرسة.

يوضح المثال كيفية الحصول على تقارير الفهرسة.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // إنشاء فهرس في المجلد المحدد
index.add(documentsFolder); // فهرسة المستندات من المجلد المحدد
IndexingReport[] reports = index.getIndexingReports(); // الحصول على تقارير الفهرسة
 
```
 
````


### getSearchReports() {#getSearchReports--}
```
public final SearchReport[] getSearchReports()
```


يحصل على التقارير حول عمليات البحث.


**Returns:**
com.groupdocs.search.common.SearchReport[] - تقارير البحث.

يوضح المثال كيفية الحصول على تقارير البحث.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query1 = \"Einstein\";
String query2 = \"Newton\";
Index index = new Index(indexFolder); // إنشاء فهرس في المجلد المحدد
index.add(documentsFolder); // فهرسة المستندات من المجلد المحدد
SearchResult result1 = index.search(query1); // بحث
SearchResult result2 = index.search(query2);
SearchResult result3 = index.search(query1 + \" & \" + query2);
SearchReport[] reports = index.getSearchReports(); // جلب تقارير البحث
 
```
 
````


### search(String query) {#search-java.lang.String-}
```
public final SearchResult search(String query)
```


يبحث في الفهرس.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | query | java.lang.String | استعلام البحث. |

المثال التالي يوضح كيفية إجراء بحث بسيط.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // إنشاء فهرس في المجلد المحدد
index.add(documentsFolder); // فهرسة المستندات من المجلد المحدد
SearchResult result = index.search(query); // البحث
 
```
 
````

المثال التالي يوضح كيفية إجراء بحث Regex.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // إنشاء فهرس في المجلد المحدد
index.add(documentsFolder); // فهرسة المستندات من المجلد المحدد
String query = "^[0-9]{3,}"; // رمز ^ في بداية استعلام البحث يخبر الفهرس بأنه استعلام Regex
SearchResult result = index.search(query); // البحث
 
```
 
````

المثال التالي يوضح كيفية إجراء بحث Faceted.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // إنشاء فهرس في المجلد المحدد
index.add(documentsFolder); // فهرسة المستندات من المجلد المحدد
String query = "content:Newton"; // الكلمة قبل النقطتين في الاستعلام تعني اسم حقل المستند للبحث
SearchResult result = index.search(query); // البحث
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(String query, SearchOptions options) {#search-java.lang.String-com.groupdocs.search.options.SearchOptions-}
```
public final SearchResult search(String query, SearchOptions options)
```


يبحث في الفهرس.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | query | java.lang.String | استعلام البحث. |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | خيارات البحث. |

المثال التالي يوضح كيفية إجراء بحث Fuzzy.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // إنشاء فهرس في المجلد المحدد
index.add(documentsFolder); // فهرسة المستندات من المجلد المحدد
SearchOptions options = new SearchOptions();
options.getFuzzySearch().setEnabled(true); // تمكين بحث Fuzzy
options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(1)); // تعيين عدد الاختلافات الممكنة لكل كلمة
// علامات الاقتباس المزدوجة في البداية والنهاية تخبر الفهرس بأنه استعلام بحث عبارة
String query = "\"The Pursuit of Happiness\"";
SearchResult result = index.search(query, options); // البحث
 
```
 
````

المثال التالي يوضح كيفية إجراء بحث المرادفات.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // إنشاء فهرس في المجلد المحدد
index.add(documentsFolder); // فهرسة المستندات من المجلد المحدد
SearchOptions options = new SearchOptions();
options.setUseSynonymSearch(true); // تمكين بحث المرادفات
String query = "cry";
SearchResult result = index.search(query, options); // البحث
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(SearchQuery query) {#search-com.groupdocs.search.SearchQuery-}
```
public final SearchResult search(SearchQuery query)
```


يبحث في الفهرس.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | استعلام البحث. |

المثال التالي يوضح كيفية إجراء بحث باستخدام الاستعلام في شكل كائن.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // إنشاء فهرس في المجلد المحدد
index.add(documentsFolder); // فهرسة المستندات من المجلد المحدد
// إنشاء الاستعلام الفرعي 1
SearchQuery subquery1 = SearchQuery.createWordQuery("accommodation");
subquery1.setSearchOptions(new SearchOptions()); // تعيين خيارات البحث فقط للاستعلام الفرعي 1
subquery1.getSearchOptions().getFuzzySearch().setEnabled(true); // تمكين بحث Fuzzy
subquery1.getSearchOptions().getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(3)); // تعيين الحد الأقصى لعدد الاختلافات
// إنشاء الاستعلام الفرعي 2
SearchQuery subquery2 = SearchQuery.createNumericRangeQuery(1, 1000000);
// إنشاء الاستعلام الفرعي 3
SearchQuery subquery3 = SearchQuery.createRegexQuery("(.)\\1");
// دمج الاستعلامات الفرعية في استعلام واحد
SearchQuery query = SearchQuery.createPhraseSearchQuery(subquery1, subquery2, subquery3);
SearchResult result = index.search(query); // البحث
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(SearchQuery query, SearchOptions options) {#search-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-}
```
public final SearchResult search(SearchQuery query, SearchOptions options)
```


يبحث في الفهرس.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | استعلام البحث. |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | خيارات البحث. |

المثال التالي يوضح كيفية إجراء بحث باستخدام الاستعلام في شكل كائن.

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

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(SearchImage image, ImageSearchOptions options) {#search-com.groupdocs.search.common.SearchImage-com.groupdocs.search.options.ImageSearchOptions-}
```
public final ImageSearchResult search(SearchImage image, ImageSearchOptions options)
```


ينفذ بحث صورة عكسي في الفهرس.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | image | [SearchImage](../../com.groupdocs.search.common/searchimage) | الصورة للبحث. |
|
|  | options | [ImageSearchOptions](../../com.groupdocs.search.options/imagesearchoptions) | خيارات بحث الصورة. |
|

**Returns:**
[ImageSearchResult](../../com.groupdocs.search.results/imagesearchresult) - The result of a reverse image search.

### searchNext(ChunkSearchToken chunkSearchToken) {#searchNext-com.groupdocs.search.common.ChunkSearchToken-}
```
public final SearchResult searchNext(ChunkSearchToken chunkSearchToken)
```


يكمل بحث الجزء الذي بدأ بطريقة Search.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | chunkSearchToken | [ChunkSearchToken](../../com.groupdocs.search.common/chunksearchtoken) | رمز البحث عن الجزء. |

يوضح المثال كيفية إجراء بحث عن الجزء.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // إنشاء فهرس في المجلد المحدد
index.add(documentsFolder); // فهرسة المستندات من المجلد المحدد
SearchOptions options = new SearchOptions();
options.setChunkSearch(true); // تمكين بحث الجزء
SearchResult result = index.search(query, options); // بدء بحث الجزء
System.out.println("Document count: " + result.getDocumentCount());
System.out.println("Occurrence count: " + result.getOccurrenceCount());
while (result.getNextChunkSearchToken() != null) {
result = index.searchNext(result.getNextChunkSearchToken()); // متابعة بحث الجزء
System.out.println("Document count: " + result.getDocumentCount());
System.out.println("Occurrence count: " + result.getOccurrenceCount());
}
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### searchNext(ChunkSearchToken chunkSearchToken, Cancellation cancellation) {#searchNext-com.groupdocs.search.common.ChunkSearchToken-com.groupdocs.search.common.Cancellation-}
```
public final SearchResult searchNext(ChunkSearchToken chunkSearchToken, Cancellation cancellation)
```


يكمل بحث الجزء الذي بدأ بطريقة Search.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | chunkSearchToken | [ChunkSearchToken](../../com.groupdocs.search.common/chunksearchtoken) | رمز البحث عن الجزء. |
|
|  | cancellation | [Cancellation](../../com.groupdocs.search.common/cancellation) | كائن الإلغاء. |

يوضح المثال كيفية إجراء البحث باستخدام الاستعلام في شكل كائن.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // إنشاء فهرس في المجلد المحدد
index.add(documentsFolder); // فهرسة المستندات من المجلد المحدد
Cancellation cancellation = new Cancellation(); // هذا الكائن يلغي جميع استمرارات البحث إذا تم الإلغاء
SearchOptions options = new SearchOptions();
options.setChunkSearch(true); // تمكين بحث الجزء
options.setCancellation(cancellation);
SearchResult result = index.search(query, options); // بدء بحث الجزء
System.out.println("Document count: " + result.getDocumentCount());
System.out.println("Occurrence count: " + result.getOccurrenceCount());
while (result.getNextChunkSearchToken() != null) {
result = index.searchNext(result.getNextChunkSearchToken(), cancellation); // متابعة بحث الجزء
System.out.println("Document count: " + result.getDocumentCount());
System.out.println("Occurrence count: " + result.getOccurrenceCount());
}
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### optimize() {#optimize--}
```
public final void optimize()
```


يقلل عدد مقاطع الفهرس بدمجها واحدة مع الأخرى.
هذه العملية تحسن أداء البحث.

يوضح المثال كيفية دمج أجزاء الفهرس.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder1 = "c:\\MyDocuments1\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
String documentsFolder3 = "c:\\MyDocuments3\\";
Index index = new Index(indexFolder); // إنشاء فهرس في المجلد المحدد
index.add(documentsFolder1); // فهرسة المستندات من المجلد المحدد
index.add(documentsFolder2); // كل استدعاء لـ AddToIndex ينشئ على الأقل جزءًا جديدًا في الفهرس
index.add(documentsFolder3);
// دمج أجزاء الفهرس
index.optimize();
 
```
 
````



### optimize(MergeOptions options) {#optimize-com.groupdocs.search.options.MergeOptions-}
```
public final void optimize(MergeOptions options)
```


يقلل عدد مقاطع الفهرس بدمجها واحدة مع الأخرى.
هذه العملية تحسن أداء البحث.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | options | [MergeOptions](../../com.groupdocs.search.options/mergeoptions) | خيارات الدمج. |

يوضح المثال كيفية دمج أجزاء من الفهرس باستخدام خيارات دمج معينة.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder1 = "c:\\MyDocuments1\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
String documentsFolder3 = "c:\\MyDocuments3\\";
Index index = new Index(indexFolder); // إنشاء فهرس في المجلد المحدد
index.add(documentsFolder1); // فهرسة المستندات من المجلد المحدد
index.add(documentsFolder2); // كل استدعاء لـ AddToIndex ينشئ على الأقل جزءًا جديدًا في الفهرس
index.add(documentsFolder3);
MergeOptions options = new MergeOptions();
options.setAsync(true); // عملية غير متزامنة
options.setCancellation(new Cancellation()); // إنشاء كائن الإلغاء
// دمج أجزاء الفهرس
index.optimize(options); // ستعود هذه الطريقة قبل إكمال العملية
options.getCancellation().cancelAfter(10000); // تحديد أقصى مدة للعملية إلى 10 ثوانٍ
 
```
 
````

|

### merge(Index index, MergeOptions options) {#merge-com.groupdocs.search.Index-com.groupdocs.search.options.MergeOptions-}
```
public final void merge(Index index, MergeOptions options)
```


يدمج الفهرس المحدد في الفهرس الحالي.
لاحظ أن الفهرس الآخر لن يتغير.


إذا كان للفهرس الآخر نسخة سابقة، يجب تحديثها قبل الدمج مع
IndexUpdater
.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | index | [Index](../../com.groupdocs.search/index) | الفهرس المراد الدمج إليه. |
|
|  | options | [MergeOptions](../../com.groupdocs.search.options/mergeoptions) | خيارات الدمج. |

يوضح المثال كيفية دمج فهرس في الفهرس الحالي.

````
 ```

String indexFolder1 = "c:\\MyIndex1\\";
String indexFolder2 = "c:\\MyIndex2\\";
String documentsFolder1 = "c:\\MyDocuments1\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
Index index1 = new Index(indexFolder1); // إنشاء index1
index1.add(documentsFolder1); // فهرسة المستندات
Index index2 = new Index(indexFolder2); // إنشاء index2
index2.add(documentsFolder2); // فهرسة المستندات
MergeOptions options = new MergeOptions();
options.setCancellation(new Cancellation()); // إنشاء كائن الإلغاء
// دمج index2 في index1. لاحظ أن ملفات index2 لن تتغير.
index1.merge(index2, options);
 
```
 
````

|

### merge(IndexRepository repository, MergeOptions options) {#merge-com.groupdocs.search.IndexRepository-com.groupdocs.search.options.MergeOptions-}
```
public final void merge(IndexRepository repository, MergeOptions options)
```


يدمج الفهارس من مستودع الفهرس المحدد إلى الفهرس الحالي.
لاحظ أن الفهارس في المستودع لن تتغير.


إذا كان للفهارس الأخرى نسخة سابقة، يجب تحديثها قبل الدمج مع
IndexUpdater
.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | repository | [IndexRepository](../../com.groupdocs.search/indexrepository) | مستودع الفهارس المراد الدمج إليه. |
|
|  | options | [MergeOptions](../../com.groupdocs.search.options/mergeoptions) | خيارات الدمج. |

يوضح المثال كيفية دمج مستودع فهارس في الفهرس الحالي.

````
 ```

String indexFolder1 = "c:\\MyIndex1\\";
String indexFolder2 = "c:\\MyIndex2\\";
String indexFolder3 = "c:\\MyIndex3\\";
String documentsFolder1 = "c:\\MyDocuments1\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
String documentsFolder3 = "c:\\MyDocuments3\\";
Index index1 = new Index(indexFolder1); // إنشاء index1
index1.add(documentsFolder1); // فهرسة المستندات
IndexRepository repository = new IndexRepository(); // إنشاء مستودع الفهارس
Index index2 = repository.create(indexFolder2); // إنشاء الفهرس2
index2.add(documentsFolder2); // فهرسة المستندات
Index index3 = repository.create(indexFolder3); // إنشاء الفهرس3
index3.add(documentsFolder3); // فهرسة المستندات
MergeOptions options = new MergeOptions();
options.setCancellation(new Cancellation()); // إنشاء كائن الإلغاء
// دمج جميع الفهارس في مستودع الفهارس إلى الفهرس1. لاحظ أن الفهرس2 والفهرس3 لن يتغيرا.
index1.merge(repository, options);
 
```
 
````

|

### highlight(FoundDocument document, Highlighter highlighter) {#highlight-com.groupdocs.search.results.FoundDocument-com.groupdocs.search.highlighters.Highlighter-}
```
public final void highlight(FoundDocument document, Highlighter highlighter)
```


ينشئ نصًا بتنسيق HTML مع تسليط الضوء على المصطلحات التي تم العثور عليها.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | document | [FoundDocument](../../com.groupdocs.search.results/founddocument) | المستند الموجود. |
|
|  | highlighter | [Highlighter](../../com.groupdocs.search.highlighters/highlighter) | مُبرز نتيجة البحث. |

يوضح المثال كيفية تمييز التكرارات في نص منسق بـHTML.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentFolder = "c:\\MyDocuments\\";
// إنشاء فهرس
Index index = new Index(indexFolder);
// فهرسة المستندات من المجلد المحدد
index.add(documentFolder);
// البحث عن كلمة 'eternity'
SearchResult result = index.search("eternity");
// تمييز التكرارات في النص
if (result.getDocumentCount() > 0) {
FoundDocument document = result.getFoundDocument(0); // الحصول على أول مستند تم العثور عليه
OutputAdapter outputAdapter = new FileOutputAdapter("c:\\Highlighted.html"); // إنشاء محول إخراج إلى الملف
Highlighter highlighter = new HtmlHighlighter(outputAdapter); // إنشاء كائن المُبرز
index.highlight(document, highlighter); // إنشاء نص منسق بـHTML مع تمييز التكرارات
}
 
```
 
````

|

### highlight(FoundDocument document, Highlighter highlighter, HighlightOptions options) {#highlight-com.groupdocs.search.results.FoundDocument-com.groupdocs.search.highlighters.Highlighter-com.groupdocs.search.options.HighlightOptions-}
```
public final void highlight(FoundDocument document, Highlighter highlighter, HighlightOptions options)
```


ينشئ نصًا بتنسيق HTML مع تسليط الضوء على المصطلحات التي تم العثور عليها.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | document | [FoundDocument](../../com.groupdocs.search.results/founddocument) | المستند الموجود. |
|
|  | highlighter | [Highlighter](../../com.groupdocs.search.highlighters/highlighter) | مُبرز نتيجة البحث. |
|
|  | options | [HighlightOptions](../../com.groupdocs.search.options/highlightoptions) | خيارات التمييز. |

يوضح المثال كيفية تمييز التكرارات في نص منسق بـHTML.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentFolder = "c:\\MyDocuments\\";
// إنشاء فهرس
Index index = new Index(indexFolder);
// فهرسة المستندات من المجلد المحدد
index.add(documentFolder);
// البحث عن كلمة 'eternity'
SearchResult result = index.search("eternity");
// تمييز التكرارات في النص
if (result.getDocumentCount() > 0) {
FoundDocument document = result.getFoundDocument(0); // الحصول على أول مستند تم العثور عليه
OutputAdapter outputAdapter = new FileOutputAdapter("c:\\Highlighted.html"); // إنشاء محول إخراج إلى الملف
Highlighter highlighter = new HtmlHighlighter(outputAdapter); // إنشاء كائن المُبرز
HighlightOptions options = new HighlightOptions(); // إنشاء كائن خيارات التمييز
options.setTermsBefore(5);
options.setTermsAfter(5);
options.setTermsTotal(15);
index.highlight(document, highlighter, options); // إنشاء نص بتنسيق HTML مع تظليل الحالات
}
 
```
 
````

|

### getIndexedDocuments() {#getIndexedDocuments--}
```
public final DocumentInfo[] getIndexedDocuments()
```


يحصل على مصفوفة من جميع المستندات المفهرسة.


**Returns:**
com.groupdocs.search.results.DocumentInfo[] - مصفوفة تحتوي على جميع المستندات المفهرسة.

يوضح المثال كيفية الحصول على قائمة بالمستندات المفهرسة من الفهرس.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// إنشاء فهرس في المجلد المحدد
Index index = new Index(indexFolder);
// فهرسة المستندات من المجلد المحدد
index.add(documentsFolder);
// الحصول على قائمة بالمستندات المفهرسة
DocumentInfo[] documents = index.getIndexedDocuments();
 
```
 
````


### getIndexedDocumentItems(DocumentInfo documentInfo) {#getIndexedDocumentItems-com.groupdocs.search.results.DocumentInfo-}
```
public final DocumentInfo[] getIndexedDocumentItems(DocumentInfo documentInfo)
```


يحصل على مصفوفة من عناصر المستند.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | documentInfo | [DocumentInfo](../../com.groupdocs.search.results/documentinfo) | معلومات المستند. |

يوضح المثال كيفية الحصول على قائمة بعناصر مستند مفهرس من الفهرس.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// إنشاء فهرس في المجلد المحدد
Index index = new Index(indexFolder);
// فهرسة المستندات من المجلد المحدد
index.add(documentsFolder);
// الحصول على قائمة بالمستندات المفهرسة
DocumentInfo[] documents = index.getIndexedDocuments();
for (int i = 0; i < documents.length; i++) {
DocumentInfo document = documents[i];
System.out.println(document.getFilePath());
DocumentInfo[] items = index.getIndexedDocumentItems(document); // الحصول على قائمة بعناصر المستند
for (int j = 0; j < items.length; j++) {
DocumentInfo item = items[j];
System.out.println("\t" + item.getInnerPath());
}
}
 
```
 
````

|

**Returns:**
com.groupdocs.search.results.DocumentInfo[] - مصفوفة لعناصر المستند.

### GetIndexedDocument(String documentKey) {#GetIndexedDocument-java.lang.String-}
```
public DocumentInfo GetIndexedDocument(String documentKey)
```


يحصل على مستند مفهرس بواسطة مفتاح المستند.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | documentKey | java.lang.String | مفتاح المستند. |
|

**Returns:**
[DocumentInfo](../../com.groupdocs.search.results/documentinfo) - The indexed document.

### getDocumentText(DocumentInfo documentInfo, OutputAdapter adapter) {#getDocumentText-com.groupdocs.search.results.DocumentInfo-com.groupdocs.search.common.OutputAdapter-}
```
public final void getDocumentText(DocumentInfo documentInfo, OutputAdapter adapter)
```


ينشئ نص المستند المفهرس ويمرره عبر محول الإخراج.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | documentInfo | [DocumentInfo](../../com.groupdocs.search.results/documentinfo) | معلومات المستند المفهرس. |
|
|  | adapter | [OutputAdapter](../../com.groupdocs.search.common/outputadapter) | محول الإخراج. |

يوضح المثال كيفية الحصول على نص مستند مفهرس من الفهرس.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// إنشاء فهرس في المجلد المحدد
Index index = new Index(indexFolder);
// فهرسة المستندات من المجلد المحدد
index.add(documentsFolder);
// الحصول على قائمة بالمستندات المفهرسة
DocumentInfo[] documents = index.getIndexedDocuments();
// الحصول على نص المستند
if (documents.length > 0) {
FileOutputAdapter outputAdapter = new FileOutputAdapter("C:\\Text.html");
index.getDocumentText(documents[0], outputAdapter);
}
 
```
 
````

|

### getDocumentText(DocumentInfo documentInfo, OutputAdapter adapter, TextOptions options) {#getDocumentText-com.groupdocs.search.results.DocumentInfo-com.groupdocs.search.common.OutputAdapter-com.groupdocs.search.options.TextOptions-}
```
public final void getDocumentText(DocumentInfo documentInfo, OutputAdapter adapter, TextOptions options)
```


ينشئ نصًا بتنسيق HTML للمستند المفهرس وينقله عبر محول الإخراج.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | documentInfo | [DocumentInfo](../../com.groupdocs.search.results/documentinfo) | معلومات المستند المفهرس. |
|
|  | adapter | [OutputAdapter](../../com.groupdocs.search.common/outputadapter) | محول الإخراج. |
|
|  | options | [TextOptions](../../com.groupdocs.search.options/textoptions) | خيارات استرجاع النص. |
|

### getIndexedPaths() {#getIndexedPaths--}
```
public final String[] getIndexedPaths()
```


يحصل على مصفوفة من المسارات المفهرسة - مستندات أو مجلدات.


**Returns:**
java.lang.String[] - مصفوفة للمسارات المفهرسة.

### delete(String[] paths, UpdateOptions options) {#delete-java.lang.String---com.groupdocs.search.options.UpdateOptions-}
```
public final DeleteResult delete(String[] paths, UpdateOptions options)
```


يحذف الملفات أو المجلدات المفهرسة من الفهرس. ثم يقوم بتحديث الفهرس دون المسارات المحذوفة.
لاحظ أن المستند الفردي لا يمكن حذفه من الفهرس إذا تم إضافته إلى الفهرس كجزء من مجلد.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | المسارات | java.lang.String[] | المسارات إلى الملفات أو المجلدات التي سيتم حذفها. |
|
|  | options | [UpdateOptions](../../com.groupdocs.search.options/updateoptions) | خيارات التحديث. |

يوضح المثال كيفية حذف المسارات المفهرسة من الفهرس.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder1 = "c:\\MyDocuments\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
// إنشاء فهرس في المجلد المحدد
Index index = new Index(indexFolder);
// فهرسة المستندات من المجلدات المحددة
index.add(documentsFolder1);
index.add(documentsFolder2);
// الحصول على المسارات المفهرسة من الفهرس
String[] indexedPaths1 = index.getIndexedPaths();
// كتابة المسارات المفهرسة إلى وحدة التحكم
System.out.println("المسارات المفهرسة:");
for (String path : indexedPaths1) {
System.out.println("\t" + path);
}
// حذف مسار الفهرس من الفهرس
DeleteResult deleteResult = index.delete(new String[] { documentsFolder1 }, new UpdateOptions());
// الحصول على المسارات المفهرسة بعد الحذف
String[] indexedPaths2 = index.getIndexedPaths();
System.out.println("\nالمسارات المحذوفة: " + deleteResult.getSuccessCount());
System.out.println("\nالمسارات المفهرسة:");
for (String path : indexedPaths2) {
System.out.println("\t" + path);
}
 
```
 
````

|

**Returns:**
[DeleteResult](../../com.groupdocs.search.results/deleteresult) - An object describing the result of deleting files or folders from the index.

### delete(UpdateOptions options, String[] documentKeys) {#delete-com.groupdocs.search.options.UpdateOptions-java.lang.String---}
```
public final DeleteResult delete(UpdateOptions options, String[] documentKeys)
```


يحذف المستندات المفهرسة من التدفقات أو الهياكل. ثم يقوم بتحديث الفهرس بدون المستندات المحذوفة.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | options | [UpdateOptions](../../com.groupdocs.search.options/updateoptions) | خيارات التحديث. |
|
|  | documentKeys | java.lang.String[] | مفاتيح المستندات المضافة من التدفقات أو الهياكل. |
|

**Returns:**
[DeleteResult](../../com.groupdocs.search.results/deleteresult) - An object describing the result of deleting documents from the index.

### notifyIndex(Notification notification) {#notifyIndex-com.groupdocs.search.Notification-}
```
public final boolean notifyIndex(Notification notification)
```


يمرر كائن الإشعار المحدد إلى الفهرس لتنفيذ الإشعار.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | notification | [Notification](../../com.groupdocs.search/notification) | كائن الإشعار. |
|

**Returns:**
boolean - يُعيد  true  إذا تم تنفيذ الإشعار بنجاح؛ وإلا  false .

### changeAttributes(AttributeChangeBatch batch) {#changeAttributes-com.groupdocs.search.common.AttributeChangeBatch-}
```
public final void changeAttributes(AttributeChangeBatch batch)
```


يطبق دفعة التغييرات على السمات المحددة على المستندات المفهرسة دون إعادة الفهرسة أثناء عملية التحديث.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | batch | [AttributeChangeBatch](../../com.groupdocs.search.common/attributechangebatch) | دفعة تغيير السمة. |
|

### getAttributes(String path) {#getAttributes-java.lang.String-}
```
public final String[] getAttributes(String path)
```


يحصل على جميع السمات المرتبطة بالمستند المفهرس المحدد.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | path | java.lang.String | مسار المستند. |
|

**Returns:**
java.lang.String[] - السمات المرتبطة بالمستند.

### loadIntoMemoryCompletely(String indexFolder) {#loadIntoMemoryCompletely-java.lang.String-}
```
public static Index loadIntoMemoryCompletely(String indexFolder)
```


يقوم بتحميل الفهرس بالكامل إلى الذاكرة.
أي تغييرات على الفهرس لا يتم حفظها تلقائيًا في المجلد الأصلي.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | indexFolder | java.lang.String | مسار مجلد الفهرس. |
|

**Returns:**
[Index](../../com.groupdocs.search/index) - The loaded in-memory index.

### loadIntoMemoryCompletely(String indexFolder, IndexSettings settings) {#loadIntoMemoryCompletely-java.lang.String-com.groupdocs.search.IndexSettings-}
```
public static Index loadIntoMemoryCompletely(String indexFolder, IndexSettings settings)
```


يقوم بتحميل الفهرس بالكامل إلى الذاكرة.
أي تغييرات على الفهرس لا يتم حفظها تلقائيًا في المجلد الأصلي.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | indexFolder | java.lang.String | مسار مجلد الفهرس. |
|
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | كائن إعدادات الفهرس. |
|

**Returns:**
[Index](../../com.groupdocs.search/index) - The loaded in-memory index.

