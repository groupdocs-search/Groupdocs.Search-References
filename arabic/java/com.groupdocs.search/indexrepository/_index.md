---
title: "IndexRepository"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يمثل حاوية لدمج فهارس متعددة وإجراء عمليات شائعة عليها."
type: docs
weight: 18
url: /ar/java/com.groupdocs.search/indexrepository/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.io.Closeable
```
public class IndexRepository implements Closeable
```

يمثل حاوية لدمج فهارس متعددة وإجراء عمليات شائعة عليها.


**Learn more**

* [Search index repository](../https://docs.groupdocs.com/display/searchjava/Search+index+repository)


المثال يوضح استخدامًا نموذجيًا للفئة.

````
 ```

String indexFolder1 = "c:\\MyIndex\\";
String indexFolder2 = "c:\\MyIndex\\";
String query = "Einstein";
IndexRepository repository = new IndexRepository();
repository.addToRepository(indexFolder1); // تحميل فهرس موجود
repository.addToRepository(indexFolder2); // تحميل فهرس موجود آخر
SearchResult result = repository.search(query); // البحث في فهارس المستودع
 
```
 
````


## المنشئات

| منشئ | الوصف |
| --- | --- |
|  | [IndexRepository()](#IndexRepository--) | يُنشئ مثيلاً جديدًا لـ |
IndexRepository
الفئة.
|
## طرق

| طريقة | الوصف |
| --- | --- |
|  | [getEvents()](#getEvents--) | يحصل على مركز الأحداث للاشتراك في الأحداث. |
|
|  | [getIndexes()](#getIndexes--) | يحصل على الفهارس الموجودة في هذا |
IndexRepository
.
|
|  | [close()](#close--) | يطلق جميع الموارد المستخدمة بواسطة |
IndexRepository
.
|
|  | [create()](#create--) | ينشئ فهرسًا جديدًا في الذاكرة. |
|
|  | [create(IndexSettings settings)](#create-com.groupdocs.search.IndexSettings-) | ينشئ فهرسًا جديدًا في الذاكرة. |
|
|  | [create(String indexFolder)](#create-java.lang.String-) | ينشئ فهرسًا جديدًا على القرص. |
|
|  | [create(String indexFolder, IndexSettings settings)](#create-java.lang.String-com.groupdocs.search.IndexSettings-) | ينشئ فهرسًا جديدًا على القرص. |
|
|  | [addToRepository(Index index)](#addToRepository-com.groupdocs.search.Index-) | يضيف فهرسًا إلى مستودع الفهارس. |
|
|  | [addToRepository(String indexFolder)](#addToRepository-java.lang.String-) | يفتح ويضيف فهرسًا إلى مستودع الفهارس. |
|
|  | [update()](#update--) | يحدّث جميع الفهارس في المستودع. |
|
|  | [update(UpdateOptions options)](#update-com.groupdocs.search.options.UpdateOptions-) | يحدّث جميع الفهارس في المستودع. |
|
|  | [search(String query)](#search-java.lang.String-) | يبحث في جميع الفهارس في المستودع. |
|
|  | [search(String query, SearchOptions options)](#search-java.lang.String-com.groupdocs.search.options.SearchOptions-) | يبحث في جميع الفهارس في المستودع. |
|
|  | [search(SearchQuery query)](#search-com.groupdocs.search.SearchQuery-) | يبحث في جميع الفهارس في المستودع. |
|
|  | [search(SearchQuery query, SearchOptions options)](#search-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-) | يبحث في جميع الفهارس في المستودع. |
|
### IndexRepository() {#IndexRepository--}
```
public IndexRepository()
```


يُنشئ مثيلاً جديدًا لـ
IndexRepository
الفئة.


### getEvents() {#getEvents--}
```
public final EventHub getEvents()
```


يحصل على مركز الأحداث للاشتراك في الأحداث.


**Returns:**
[EventHub](../../com.groupdocs.search.events/eventhub) - The event hub for subscribing to events.

### getIndexes() {#getIndexes--}
```
public final Index[] getIndexes()
```


يحصل على الفهارس الموجودة في هذا
IndexRepository
.


**Returns:**
com.groupdocs.search.Index[] - الفهارس.

### close() {#close--}
```
public final void close()
```


يطلق جميع الموارد المستخدمة بواسطة
IndexRepository
.


### create() {#create--}
```
public final Index create()
```


ينشئ فهرسًا جديدًا في الذاكرة.


**Returns:**
[Index](../../com.groupdocs.search/index) - The created index.

يوضح المثال كيفية إنشاء فهرس في الذاكرة عبر مستودع الفهارس.

````
 ```

IndexRepository indexRepository = new IndexRepository();
Index index = indexRepository.create();
 
```
 
````


### create(IndexSettings settings) {#create-com.groupdocs.search.IndexSettings-}
```
public final Index create(IndexSettings settings)
```


ينشئ فهرسًا جديدًا في الذاكرة.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | إعدادات الفهرس. |

يوضح المثال كيفية إنشاء فهرس في الذاكرة عبر مستودع الفهارس.

````
 ```

IndexRepository indexRepository = new IndexRepository();
IndexSettings settings = new IndexSettings();
settings.setUseStopWords(false); // تعطيل استخدام كلمات التوقف أثناء الفهرسة
Index index = indexRepository.create(settings);
 
```
 
````

|

**Returns:**
[Index](../../com.groupdocs.search/index) - The created index.

### create(String indexFolder) {#create-java.lang.String-}
```
public final Index create(String indexFolder)
```


ينشئ فهرسًا جديدًا على القرص.
سيتم تنظيف مجلد الفهرس قبل إنشاء الفهرس.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | indexFolder | java.lang.String | مجلد الفهرس. |

يوضح المثال كيفية إنشاء فهرس على القرص عبر مستودع الفهارس.

````
 ```

String indexFolder = "c:\\MyIndex\\";
IndexRepository indexRepository = new IndexRepository();
Index index = indexRepository.create(indexFolder);
 
```
 
````

|

**Returns:**
[Index](../../com.groupdocs.search/index) - The created index.

### create(String indexFolder, IndexSettings settings) {#create-java.lang.String-com.groupdocs.search.IndexSettings-}
```
public final Index create(String indexFolder, IndexSettings settings)
```


ينشئ فهرسًا جديدًا على القرص.
سيتم تنظيف مجلد الفهرس قبل إنشاء الفهرس.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | indexFolder | java.lang.String | مجلد الفهرس. |
|
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | إعدادات الفهرس. |

يوضح المثال كيفية إنشاء فهرس على القرص عبر مستودع الفهارس.

````
 ```

String indexFolder = "c:\\MyIndex\\";
IndexRepository indexRepository = new IndexRepository();
IndexSettings settings = new IndexSettings();
settings.setUseStopWords(false); // تعطيل استخدام كلمات التوقف أثناء الفهرسة
Index index = indexRepository.create(indexFolder, settings);
 
```
 
````

|

**Returns:**
[Index](../../com.groupdocs.search/index) - The created index.

### addToRepository(Index index) {#addToRepository-com.groupdocs.search.Index-}
```
public final void addToRepository(Index index)
```


يضيف فهرسًا إلى مستودع الفهارس.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | index | [Index](../../com.groupdocs.search/index) | الفهرس للإضافة. |

يوضح المثال كيفية إضافة فهرس إلى مستودع الفهارس.

````
 ```

Index index = new Index();
IndexRepository indexRepository = new IndexRepository();
indexRepository.addToRepository(index);
 
```
 
````

|

### addToRepository(String indexFolder) {#addToRepository-java.lang.String-}
```
public final void addToRepository(String indexFolder)
```


يفتح ويضيف فهرسًا إلى مستودع الفهارس.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | indexFolder | java.lang.String | مجلد الفهرس. |

يوضح المثال كيفية إضافة فهرس إلى مستودع الفهارس.

````
 ```

String indexFolder = "c:\\MyIndex\\";
IndexRepository indexRepository = new IndexRepository();
indexRepository.addToRepository(indexFolder);
 
```
 
````

|

### update() {#update--}
```
public final void update()
```


يحدّث جميع الفهارس في المستودع.

يوضح المثال كيفية تحديث الفهارس في المستودع.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // إنشاء الفهرس
index.add(documentsFolder); // فهرسة المستندات
// حذف المستندات من مجلد المستندات أو تعديلها أو إضافة مستندات جديدة إلى المجلد
repository.update();
 
```
 
````



### update(UpdateOptions options) {#update-com.groupdocs.search.options.UpdateOptions-}
```
public final void update(UpdateOptions options)
```


يحدّث جميع الفهارس في المستودع.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | options | [UpdateOptions](../../com.groupdocs.search.options/updateoptions) | خيارات التحديث. |

يوضح المثال كيفية تحديث الفهارس في المستودع.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // إنشاء الفهرس
index.add(documentsFolder); // فهرسة المستندات
// حذف المستندات من مجلد المستندات أو تعديلها أو إضافة مستندات جديدة إلى المجلد
UpdateOptions options = new UpdateOptions();
options.setThreads(2); // ضبط عدد خيوط الفهرسة
repository.update(options);
 
```
 
````

|

### search(String query) {#search-java.lang.String-}
```
public final SearchResult search(String query)
```


يبحث في جميع الفهارس في المستودع.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | query | java.lang.String | استعلام البحث. |

يوضح المثال كيفية إجراء البحث في مستودع الفهرس.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // إنشاء الفهرس
index.add(documentsFolder); // فهرسة المستندات
SearchResult result = repository.search(query); // البحث
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(String query, SearchOptions options) {#search-java.lang.String-com.groupdocs.search.options.SearchOptions-}
```
public final SearchResult search(String query, SearchOptions options)
```


يبحث في جميع الفهارس في المستودع.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | query | java.lang.String | استعلام البحث. |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | خيارات البحث. |

يوضح المثال كيفية إجراء البحث في مستودع الفهرس.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // إنشاء الفهرس
index.add(documentsFolder); // فهرسة المستندات
SearchOptions options = new SearchOptions();
options.setUseCaseSensitiveSearch(true); // ضبط علامة البحث حسّاس لحالة الأحرف
SearchResult result = repository.search(query, options); // البحث
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(SearchQuery query) {#search-com.groupdocs.search.SearchQuery-}
```
public final SearchResult search(SearchQuery query)
```


يبحث في جميع الفهارس في المستودع.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | استعلام البحث. |

يوضح المثال كيفية إجراء البحث في مستودع الفهرس.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // إنشاء الفهرس
index.add(documentsFolder); // فهرسة المستندات
SearchQuery query = SearchQuery.createWordQuery("Einstein"); // إنشاء استعلام بحث في شكل كائن
SearchResult result = repository.search(query); // البحث
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(SearchQuery query, SearchOptions options) {#search-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-}
```
public final SearchResult search(SearchQuery query, SearchOptions options)
```


يبحث في جميع الفهارس في المستودع.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | استعلام البحث. |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | خيارات البحث. |

يوضح المثال كيفية إجراء البحث في مستودع الفهرس.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // إنشاء الفهرس
index.add(documentsFolder); // فهرسة المستندات
SearchOptions options = new SearchOptions();
options.setUseCaseSensitiveSearch(true); // ضبط علامة البحث حسّاس لحالة الأحرف
SearchQuery query = SearchQuery.createWordQuery("Einstein"); // إنشاء استعلام بحث في شكل كائن
SearchResult result = repository.search(query, options); // البحث
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

