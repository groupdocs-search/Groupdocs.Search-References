---
title: "SearchQuery"
second_title: "GroupDocs.Search for .NET API Reference"
description: "يمثل استعلام بحث في شكل كائن."
type: docs
weight: 1580
url: /ar/net/groupdocs.search/searchquery/
---
## SearchQuery class

يمثل استعلام بحث في شكل كائن.

```csharp
public abstract class SearchQuery
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| virtual [ChildCount](../../groupdocs.search/searchquery/childcount) { get; } | يحصل على عدد الاستعلامات الفرعية. |
| virtual [FieldName](../../groupdocs.search/searchquery/fieldname) { get; } | يحصل على اسم الحقل. |
| virtual [FirstChild](../../groupdocs.search/searchquery/firstchild) { get; } | يحصل على الاستعلام الفرعي الأول. |
| [SearchOptions](../../groupdocs.search/searchquery/searchoptions) { get; set; } | يحصل أو يضبط خيارات البحث لهذا استعلام البحث. |
| virtual [SecondChild](../../groupdocs.search/searchquery/secondchild) { get; } | يحصل على الاستعلام الفرعي الثاني. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| static [CreateAndQuery](../../groupdocs.search/searchquery/createandquery#createandquery_1)(params SearchQuery[]) | ينشئ استعلاماً مركباً سيجد المستندات التي ستُعثر عليها فقط لكل استعلام أصلي. |
| static [CreateAndQuery](../../groupdocs.search/searchquery/createandquery#createandquery)(SearchQuery, SearchQuery) | ينشئ استعلاماً مركباً سيجد المستندات التي ستُعثر عليها فقط لكل استعلام أصلي. |
| static [CreateDateRangeQuery](../../groupdocs.search/searchquery/createdaterangequery)(DateTime, DateTime) | ينشئ استعلام نطاق تاريخ. |
| static [CreateFieldQuery](../../groupdocs.search/searchquery/createfieldquery)(string, SearchQuery) | يضيف حقلًا إلى الاستعلام المحدد. |
| static [CreateNotQuery](../../groupdocs.search/searchquery/createnotquery)(SearchQuery) | ينشئ استعلامًا مقلوبًا سيُظهر المستندات المتبقية في الفهرس مقابل المستندات التي سيتم العثور عليها للاستعلام الأصلي. |
| static [CreateNumericRangeQuery](../../groupdocs.search/searchquery/createnumericrangequery)(long, long) | ينشئ استعلام نطاق رقمي. |
| static [CreateOrQuery](../../groupdocs.search/searchquery/createorquery#createorquery_1)(params SearchQuery[]) | ينشئ استعلامًا مركبًا سيجد جميع المستندات التي سيتم العثور عليها على الأقل في أحد الاستعلامات الأصلية. |
| static [CreateOrQuery](../../groupdocs.search/searchquery/createorquery#createorquery)(SearchQuery, SearchQuery) | ينشئ استعلامًا مركبًا سيجد جميع المستندات التي سيتم العثور عليها على الأقل في أحد الاستعلامات الأصلية. |
| static [CreatePhraseSearchQuery](../../groupdocs.search/searchquery/createphrasesearchquery)(params SearchQuery[]) | ينشئ استعلام بحث عن عبارة. |
| static [CreateRegexQuery](../../groupdocs.search/searchquery/createregexquery#createregexquery)(string) | ينشئ استعلام تعبير نمطي. |
| static [CreateRegexQuery](../../groupdocs.search/searchquery/createregexquery#createregexquery_1)(string, RegexOptions) | ينشئ استعلام تعبير نمطي. |
| static [CreateWildcardQuery](../../groupdocs.search/searchquery/createwildcardquery#createwildcardquery)(int) | ينشئ حرفًا بديلًا للبحث عن العبارة. |
| static [CreateWildcardQuery](../../groupdocs.search/searchquery/createwildcardquery#createwildcardquery_1)(int, int) | ينشئ حرفًا بديلًا للبحث عن العبارة. |
| static [CreateWordPatternQuery](../../groupdocs.search/searchquery/createwordpatternquery)(WordPattern) | ينشئ استعلام نمط كلمة. |
| static [CreateWordQuery](../../groupdocs.search/searchquery/createwordquery)(string) | ينشئ استعلام كلمة بسيطة. |
| abstract [GetChild](../../groupdocs.search/searchquery/getchild)(int) | يحصل على استعلام فرعي بواسطة فهرس. |
| abstract [ToString](../../groupdocs.search/searchquery/tostring)() | يرجع String يمثل المثيل الحالي لـ [`SearchQuery`](../searchquery). |

### ملاحظات

**Learn more**

* [Searching](https://docs.groupdocs.com/display/searchnet/Searching)
* [Queries in text and object form](https://docs.groupdocs.com/display/searchnet/Queries+in+text+and+object+form)
* [Nesting search queries in object form](https://docs.groupdocs.com/display/searchnet/Nesting+search+queries+in+object+form)

### أمثلة

يوضح المثال استخدامًا نموذجيًا للفئة.

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

* namespace [GroupDocs.Search](../../groupdocs.search)
* assembly [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.search.dll -->
