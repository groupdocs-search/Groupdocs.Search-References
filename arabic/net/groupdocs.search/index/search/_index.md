---
title: Search
second_title: GroupDocs. ابحث عن مرجع .NET API
description: عمليات البحث في الفهرس .
type: docs
weight: 220
url: /ar/net/groupdocs.search/index/search/
---
## Search(string) {#search_3}

عمليات البحث في الفهرس .

```csharp
public SearchResult Search(string query)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| query | String | استعلام البحث. |

### قيمة الإرجاع

نتيجة البحث.

### أمثلة

يوضح المثال التالي كيفية إجراء بحث بسيط.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

Index index = new Index(indexFolder); // إنشاء الفهرس في المجلد المحدد
index.Add(documentsFolder); // فهرسة المستندات من المجلد المحدد

SearchResult result = index.Search(query); // يبحث
```

يوضح المثال التالي كيفية إجراء بحث Regex.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // إنشاء الفهرس في المجلد المحدد
index.Add(documentsFolder); // فهرسة المستندات من المجلد المحدد

string query = "^[0-9]{3,}"; // يخبر رمز علامة الإقحام في بداية استعلام البحث الفهرس أنه استعلام Regex
SearchResult result = index.Search(query); // يبحث
```

يوضح المثال التالي كيفية إجراء بحث متعدد الأوجه.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // إنشاء الفهرس في المجلد المحدد
index.Add(documentsFolder); // فهرسة المستندات من المجلد المحدد

string query = "content:Newton"; // تعني الكلمة الموجودة قبل النقطتين في الاستعلام اسم حقل المستند المراد البحث فيه
SearchResult result = index.Search(query); // يبحث
```

### أنظر أيضا

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [Index](../../index)
* مساحة الاسم [GroupDocs.Search](../../index)
* المجسم [GroupDocs.Search](../../../)

---

## Search(string, SearchOptions) {#search_4}

عمليات البحث في الفهرس .

```csharp
public SearchResult Search(string query, SearchOptions options)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| query | String | استعلام البحث. |
| options | SearchOptions | خيارات البحث. |

### قيمة الإرجاع

نتيجة البحث.

### أمثلة

يوضح المثال التالي كيفية إجراء بحث غامض.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // إنشاء الفهرس في المجلد المحدد
index.Add(documentsFolder); // فهرسة المستندات من المجلد المحدد

SearchOptions options = new SearchOptions();
options.FuzzySearch.Enabled = true; // تمكين البحث الغامض
options.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(1); // تحديد عدد الاختلافات المحتملة لكل كلمة

// علامات الاقتباس المزدوجة في البداية والنهاية تخبر الفهرس بأنه استعلام بحث بالعبارة
string query = "\"The Pursuit of Happiness\"";
SearchResult result = index.Search(query, options); // يبحث
```

يوضح المثال التالي كيفية إجراء بحث المرادفات.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // إنشاء الفهرس في المجلد المحدد
index.Add(documentsFolder); // فهرسة المستندات من المجلد المحدد

SearchOptions options = new SearchOptions();
options.UseSynonymSearch = true; // تمكين البحث عن المرادفات

string query = "cry";
SearchResult result = index.Search(query, options); // يبحث
```

### أنظر أيضا

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchOptions](../../../groupdocs.search.options/searchoptions)
* class [Index](../../index)
* مساحة الاسم [GroupDocs.Search](../../index)
* المجسم [GroupDocs.Search](../../../)

---

## Search(SearchQuery) {#search_1}

عمليات البحث في الفهرس .

```csharp
public SearchResult Search(SearchQuery query)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| query | SearchQuery | استعلام البحث. |

### قيمة الإرجاع

نتيجة البحث.

### أمثلة

يوضح المثال التالي كيفية إجراء البحث باستخدام الاستعلام في شكل كائن.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // إنشاء الفهرس في المجلد المحدد
index.Add(documentsFolder); // فهرسة المستندات من المجلد المحدد

// إنشاء استعلام فرعي 1
SearchQuery subquery1 = SearchQuery.CreateWordQuery("accommodation");
subquery1.SearchOptions = new SearchOptions(); // تعيين خيارات البحث للاستعلام الفرعي 1 فقط
subquery1.SearchOptions.FuzzySearch.Enabled = true; // تمكين البحث الغامض
subquery1.SearchOptions.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(3); // تعيين الحد الأقصى لعدد الاختلافات

// إنشاء استعلام فرعي 2
SearchQuery subquery2 = SearchQuery.CreateNumericRangeQuery(1, 1000000);

// إنشاء استعلام فرعي 3
SearchQuery subquery3 = SearchQuery.CreateRegexQuery(@"(.)\1");

// دمج الاستعلامات الفرعية في استعلام واحد
SearchQuery query = SearchQuery.CreatePhraseSearchQuery(subquery1, subquery2, subquery3);

SearchResult result = index.Search(query); // يبحث
```

### أنظر أيضا

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchQuery](../../searchquery)
* class [Index](../../index)
* مساحة الاسم [GroupDocs.Search](../../index)
* المجسم [GroupDocs.Search](../../../)

---

## Search(SearchQuery, SearchOptions) {#search_2}

عمليات البحث في الفهرس .

```csharp
public SearchResult Search(SearchQuery query, SearchOptions options)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| query | SearchQuery | استعلام البحث. |
| options | SearchOptions | خيارات البحث. |

### قيمة الإرجاع

نتيجة البحث.

### أمثلة

يوضح المثال التالي كيفية إجراء البحث باستخدام الاستعلام في شكل كائن.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // إنشاء الفهرس في المجلد المحدد
index.Add(documentsFolder); // فهرسة المستندات من المجلد المحدد

// إنشاء استعلام فرعي للبحث في النطاق الزمني
SearchQuery subquery1 = SearchQuery.CreateDateRangeQuery(new DateTime(2011, 6, 17), new DateTime(2013, 1, 1));

// إنشاء استعلام فرعي لحرف البدل بعدد الكلمات المفقودة من 0 إلى 2
SearchQuery subquery2 = SearchQuery.CreateWildcardQuery(0, 2);

// إنشاء استعلام فرعي لكلمة بسيطة
SearchQuery subquery3 = SearchQuery.CreateWordQuery("birth");
subquery3.SearchOptions = new SearchOptions(); // تعيين خيارات البحث للاستعلام الفرعي فقط 3
subquery3.SearchOptions.FuzzySearch.Enabled = true;
subquery3.SearchOptions.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(1);

// دمج الاستعلامات الفرعية في استعلام واحد
SearchQuery query = SearchQuery.CreatePhraseSearchQuery(subquery1, subquery2, subquery3);

// إنشاء كائن خيارات البحث بقدرة متزايدة على التكرارات التي تم العثور عليها
SearchOptions options = new SearchOptions(); // خيارات البحث الشاملة
options.MaxOccurrenceCountPerTerm = 1000000;
options.MaxTotalOccurrenceCount = 10000000;

SearchResult result = index.Search(query, options); // يبحث
```

### أنظر أيضا

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchQuery](../../searchquery)
* class [SearchOptions](../../../groupdocs.search.options/searchoptions)
* class [Index](../../index)
* مساحة الاسم [GroupDocs.Search](../../index)
* المجسم [GroupDocs.Search](../../../)

---

## Search(SearchImage, ImageSearchOptions) {#search}

يقوم بإجراء بحث عكسي عن الصور في الفهرس.

```csharp
public ImageSearchResult Search(SearchImage image, ImageSearchOptions options)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| image | SearchImage | الصورة للبحث. |
| options | ImageSearchOptions | خيارات البحث عن الصور. |

### قيمة الإرجاع

نتيجة البحث العكسي عن الصور.

### أنظر أيضا

* class [ImageSearchResult](../../../groupdocs.search.results/imagesearchresult)
* class [SearchImage](../../../groupdocs.search.common/searchimage)
* class [ImageSearchOptions](../../../groupdocs.search.options/imagesearchoptions)
* class [Index](../../index)
* مساحة الاسم [GroupDocs.Search](../../index)
* المجسم [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
