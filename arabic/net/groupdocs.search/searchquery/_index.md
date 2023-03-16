---
title: SearchQuery
second_title: GroupDocs. ابحث عن مرجع .NET API
description: يمثل استعلام بحث في شكل كائن.
type: docs
weight: 1240
url: /ar/net/groupdocs.search/searchquery/
---
## SearchQuery class

يمثل استعلام بحث في شكل كائن.

```csharp
public abstract class SearchQuery
```

## الخصائص

| اسم | وصف |
| --- | --- |
| virtual [ChildCount](../../groupdocs.search/searchquery/childcount) { get; } | الحصول على عدد الاستعلامات الفرعية . |
| virtual [FieldName](../../groupdocs.search/searchquery/fieldname) { get; } | يحصل على اسم الحقل . |
| virtual [FirstChild](../../groupdocs.search/searchquery/firstchild) { get; } | الحصول على أول استعلام فرعي . |
| [SearchOptions](../../groupdocs.search/searchquery/searchoptions) { get; set; } | الحصول على أو تعيين خيارات البحث لاستعلام البحث هذا. |
| virtual [SecondChild](../../groupdocs.search/searchquery/secondchild) { get; } | الحصول على الاستعلام الفرعي الثاني . |

## طُرق

| اسم | وصف |
| --- | --- |
| static [CreateAndQuery](../../groupdocs.search/searchquery/createandquery)(SearchQuery, SearchQuery) | ينشئ استعلامًا مجمعًا يبحث فقط عن المستندات التي سيتم العثور عليها لكل استعلام أصلي. |
| static [CreateDateRangeQuery](../../groupdocs.search/searchquery/createdaterangequery)(DateTime, DateTime) | إنشاء استعلام عن نطاق تاريخ . |
| static [CreateFieldQuery](../../groupdocs.search/searchquery/createfieldquery)(string, SearchQuery) | إضافة حقل إلى الاستعلام المحدد. |
| static [CreateNotQuery](../../groupdocs.search/searchquery/createnotquery)(SearchQuery) | ينشئ استعلامًا مقلوبًا يعثر على باقي المستندات في فهرس مقابل المستندات التي سيتم العثور عليها للاستعلام الأصلي. |
| static [CreateNumericRangeQuery](../../groupdocs.search/searchquery/createnumericrangequery)(long, long) | لإنشاء استعلام نطاق رقمي . |
| static [CreateOrQuery](../../groupdocs.search/searchquery/createorquery)(SearchQuery, SearchQuery) | ينشئ استعلامًا مجمعًا يبحث عن جميع المستندات التي سيتم العثور عليها على الأقل لواحد من الاستعلامات الأصلية. |
| static [CreatePhraseSearchQuery](../../groupdocs.search/searchquery/createphrasesearchquery)(params SearchQuery[]) | لإنشاء استعلام بحث بالعبارة . |
| static [CreateRegexQuery](../../groupdocs.search/searchquery/createregexquery#createregexquery)(string) | إنشاء استعلام تعبير عادي . |
| static [CreateRegexQuery](../../groupdocs.search/searchquery/createregexquery#createregexquery_1)(string, RegexOptions) | إنشاء استعلام تعبير عادي . |
| static [CreateWildcardQuery](../../groupdocs.search/searchquery/createwildcardquery#createwildcardquery)(int) | لإنشاء حرف بدل للبحث بالعبارة . |
| static [CreateWildcardQuery](../../groupdocs.search/searchquery/createwildcardquery#createwildcardquery_1)(int, int) | لإنشاء حرف بدل للبحث بالعبارة . |
| static [CreateWordPatternQuery](../../groupdocs.search/searchquery/createwordpatternquery)(WordPattern) | إنشاء استعلام عن نمط كلمة . |
| static [CreateWordQuery](../../groupdocs.search/searchquery/createwordquery)(string) | لإنشاء استعلام كلمة بسيط . |
| abstract [GetChild](../../groupdocs.search/searchquery/getchild)(int) | الحصول على استعلام فرعي بواسطة فهرس . |
| abstract [ToString](../../groupdocs.search/searchquery/tostring)() | إرجاع أString التي تمثل التيار[`SearchQuery`](../searchquery) المثال. |

### ملاحظات

**يتعلم أكثر**

* [يبحث](https://docs.groupdocs.com/display/searchnet/Searching)
* [استعلامات في النص وشكل الكائن](https://docs.groupdocs.com/display/searchnet/Queries+in+text+and+object+form)
* [استعلامات البحث المتداخلة في شكل كائن](https://docs.groupdocs.com/display/searchnet/Nesting+search+queries+in+object+form)

### أمثلة

يوضح المثال استخدامًا نموذجيًا للفئة.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // إنشاء الفهرس في المجلد المحدد
index.Add(documentsFolder); // فهرسة المستندات من المجلد المحدد

// إنشاء استعلام فرعي للبحث في النطاق الزمني
SearchQuery subquery1 = SearchQuery.CreateDateRangeQuery(new DateTime(2011, 6, 17), new DateTime(2013, 1, 1));

// إنشاء استعلام فرعي لحرف البدل بعدد الكلمات المفقودة من 0 إلى 2
SearchQuery subquery2 = SearchQuery.CreateWildcardQuery(0, 2);

// إنشاء استعلام فرعي من كلمة بسيطة
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

* مساحة الاسم [GroupDocs.Search](../../groupdocs.search)
* المجسم [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
