---
title: "بحث"
second_title: "GroupDocs.Search for .NET API Reference"
description: "يبحث في الفهرس."
type: docs
weight: 260
url: /ar/net/groupdocs.search/index/search/
---
## Search(string) {#search_3}

يبحث في الفهرس.

```csharp
public SearchResult Search(string query)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| استعلام | سلسلة | استعلام البحث. |

### قيمة الإرجاع

نتيجة البحث.

### أمثلة

يوضح المثال التالي كيفية إجراء بحث بسيط.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

SearchResult result = index.Search(query); // Searching
```

يوضح المثال التالي كيفية إجراء بحث باستخدام تعبيرات regex.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

string query = "^[0-9]{3,}"; // The caret symbol at the beginning of the search query tells the index that it is a Regex query
SearchResult result = index.Search(query); // Searching
```

يوضح المثال التالي كيفية إجراء بحث متعدد الأوجه.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

string query = "content:Newton"; // The word before the colon in the query means the document field name to search
SearchResult result = index.Search(query); // Searching
```

### انظر أيضًا

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Search(string, SearchOptions) {#search_4}

يبحث في الفهرس.

```csharp
public SearchResult Search(string query, SearchOptions options)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| استعلام | سلسلة | استعلام البحث. |
| الخيارات | SearchOptions | خيارات البحث. |

### قيمة الإرجاع

نتيجة البحث.

### أمثلة

يوضح المثال التالي كيفية إجراء بحث غير دقيق.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

SearchOptions options = new SearchOptions();
options.FuzzySearch.Enabled = true; // Enabling the fuzzy search
options.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(1); // Setting the number of possible differences for each word

// تشير علامات الاقتباس المزدوجة في البداية والنهاية إلى الفهرس بأنها استعلام بحث عبارة.
string query = "\"The Pursuit of Happiness\"";
SearchResult result = index.Search(query, options); // Searching
```

يوضح المثال التالي كيفية إجراء بحث عن المرادفات.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

SearchOptions options = new SearchOptions();
options.UseSynonymSearch = true; // Enabling the synonym search

string query = "cry";
SearchResult result = index.Search(query, options); // Searching
```

### انظر أيضًا

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchOptions](../../../groupdocs.search.options/searchoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Search(SearchQuery) {#search_1}

يبحث في الفهرس.

```csharp
public SearchResult Search(SearchQuery query)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| استعلام | SearchQuery | استعلام البحث. |

### قيمة الإرجاع

نتيجة البحث.

### أمثلة

يوضح المثال التالي كيفية إجراء بحث باستخدام استعلام بصيغة كائن.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

// إنشاء استعلام فرعي 1
SearchQuery subquery1 = SearchQuery.CreateWordQuery("accommodation");
subquery1.SearchOptions = new SearchOptions(); // Setting search options only for subquery 1
subquery1.SearchOptions.FuzzySearch.Enabled = true; // Enabling the fuzzy search
subquery1.SearchOptions.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(3); // Setting maximum number of differences

// إنشاء استعلام فرعي 2
SearchQuery subquery2 = SearchQuery.CreateNumericRangeQuery(1, 1000000);

// إنشاء استعلام فرعي 3
SearchQuery subquery3 = SearchQuery.CreateRegexQuery(@"(.)\1");

// دمج الاستعلامات الفرعية في استعلام واحد
SearchQuery query = SearchQuery.CreatePhraseSearchQuery(subquery1, subquery2, subquery3);

SearchResult result = index.Search(query); // Searching
```

### انظر أيضًا

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchQuery](../../searchquery)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Search(SearchQuery, SearchOptions) {#search_2}

يبحث في الفهرس.

```csharp
public SearchResult Search(SearchQuery query, SearchOptions options)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| استعلام | SearchQuery | استعلام البحث. |
| الخيارات | SearchOptions | خيارات البحث. |

### قيمة الإرجاع

نتيجة البحث.

### أمثلة

يوضح المثال التالي كيفية إجراء بحث باستخدام استعلام بصيغة كائن.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

// إنشاء استعلام فرعي للبحث بنطاق التاريخ
SearchQuery subquery1 = SearchQuery.CreateDateRangeQuery(new DateTime(2011, 6, 17), new DateTime(2013, 1, 1));

// إنشاء استعلام فرعي لحرف بديل مع عدد الكلمات المفقودة من 0 إلى 2
SearchQuery subquery2 = SearchQuery.CreateWildcardQuery(0, 2);

// إنشاء استعلام فرعي لكلمة بسيطة
SearchQuery subquery3 = SearchQuery.CreateWordQuery("birth");
subquery3.SearchOptions = new SearchOptions(); // Setting search options only for subquery 3
subquery3.SearchOptions.FuzzySearch.Enabled = true;
subquery3.SearchOptions.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(1);

// دمج الاستعلامات الفرعية في استعلام واحد
SearchQuery query = SearchQuery.CreatePhraseSearchQuery(subquery1, subquery2, subquery3);

// إنشاء كائن خيارات البحث بزيادة سعة التكرارات المكتشفة
SearchOptions options = new SearchOptions(); // Overall search options
options.MaxOccurrenceCountPerTerm = 1000000;
options.MaxTotalOccurrenceCount = 10000000;

SearchResult result = index.Search(query, options); // Searching
```

### انظر أيضًا

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchQuery](../../searchquery)
* class [SearchOptions](../../../groupdocs.search.options/searchoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Search(SearchImage, ImageSearchOptions) {#search}

ينفّذ بحثًا عكسيًا عن الصور في الفهرس.

```csharp
public ImageSearchResult Search(SearchImage image, ImageSearchOptions options)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| صورة | SearchImage | الصورة للبحث. |
| الخيارات | ImageSearchOptions | خيارات بحث الصورة. |

### قيمة الإرجاع

نتيجة بحث صورة عكسي.

### انظر أيضًا

* class [ImageSearchResult](../../../groupdocs.search.results/imagesearchresult)
* class [SearchImage](../../../groupdocs.search.common/searchimage)
* class [ImageSearchOptions](../../../groupdocs.search.options/imagesearchoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.search.dll -->
