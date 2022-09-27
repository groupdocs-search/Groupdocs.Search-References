---
title: SearchQuery
second_title: GroupDocs.Search for .NET API Reference
description: Represents a search query in object form.
type: docs
weight: 1080
url: /net/groupdocs.search/searchquery/
---
## SearchQuery class

Represents a search query in object form.

```csharp
public abstract class SearchQuery
```

## Properties

| Name | Description |
| --- | --- |
| virtual [ChildCount](../../groupdocs.search/searchquery/childcount) { get; } | Gets the number of child queries. |
| virtual [FieldName](../../groupdocs.search/searchquery/fieldname) { get; } | Gets the field name. |
| virtual [FirstChild](../../groupdocs.search/searchquery/firstchild) { get; } | Gets the first child query. |
| [SearchOptions](../../groupdocs.search/searchquery/searchoptions) { get; set; } | Gets or sets the search options of this seach query. |
| virtual [SecondChild](../../groupdocs.search/searchquery/secondchild) { get; } | Gets the second child query. |

## Methods

| Name | Description |
| --- | --- |
| static [CreateAndQuery](../../groupdocs.search/searchquery/createandquery)(SearchQuery, SearchQuery) | Creates a combined query that will find only documents which will be found for each original query. |
| static [CreateDateRangeQuery](../../groupdocs.search/searchquery/createdaterangequery)(DateTime, DateTime) | Creates a date range query. |
| static [CreateFieldQuery](../../groupdocs.search/searchquery/createfieldquery)(string, SearchQuery) | Adds a field to the specified query. |
| static [CreateNotQuery](../../groupdocs.search/searchquery/createnotquery)(SearchQuery) | Creates an inverted query that will find the rest documents in an index against ones which will be found for the original query. |
| static [CreateNumericRangeQuery](../../groupdocs.search/searchquery/createnumericrangequery)(long, long) | Creates a numeric range query. |
| static [CreateOrQuery](../../groupdocs.search/searchquery/createorquery)(SearchQuery, SearchQuery) | Creates a combined query that will find all the documents which will be found at least for one of the original queries. |
| static [CreatePhraseSearchQuery](../../groupdocs.search/searchquery/createphrasesearchquery)(params SearchQuery[]) | Creates a phrase search query. |
| static [CreateRegexQuery](../../groupdocs.search/searchquery/createregexquery#createregexquery)(string) | Creates a regular expression query. |
| static [CreateRegexQuery](../../groupdocs.search/searchquery/createregexquery#createregexquery_1)(string, RegexOptions) | Creates a regular expression query. |
| static [CreateWildcardQuery](../../groupdocs.search/searchquery/createwildcardquery#createwildcardquery)(int) | Creates a wildcard for the phrase search. |
| static [CreateWildcardQuery](../../groupdocs.search/searchquery/createwildcardquery#createwildcardquery_1)(int, int) | Creates a wildcard for the phrase search. |
| static [CreateWordPatternQuery](../../groupdocs.search/searchquery/createwordpatternquery)(WordPattern) | Creates a word pattern query. |
| static [CreateWordQuery](../../groupdocs.search/searchquery/createwordquery)(string) | Creates a simple word query. |
| abstract [GetChild](../../groupdocs.search/searchquery/getchild)(int) | Gets a child query by an index. |
| abstract [ToString](../../groupdocs.search/searchquery/tostring)() | Returns a String that represents the current [`SearchQuery`](../searchquery) instance. |

### Remarks

**Learn more**

* [Searching](https://docs.groupdocs.com/display/searchnet/Searching)
* [Queries in text and object form](https://docs.groupdocs.com/display/searchnet/Queries+in+text+and+object+form)
* [Nesting search queries in object form](https://docs.groupdocs.com/display/searchnet/Nesting+search+queries+in+object+form)

### Examples

The example demonstrates a typical usage of the class.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

// Creating subquery of date range search
SearchQuery subquery1 = SearchQuery.CreateDateRangeQuery(new DateTime(2011, 6, 17), new DateTime(2013, 1, 1));

// Creating subquery of wildcard with number of missed words from 0 to 2
SearchQuery subquery2 = SearchQuery.CreateWildcardQuery(0, 2);

// Creating subquery of simple word
SearchQuery subquery3 = SearchQuery.CreateWordQuery("birth");
subquery3.SearchOptions = new SearchOptions(); // Setting search options only for subquery 3
subquery3.SearchOptions.FuzzySearch.Enabled = true;
subquery3.SearchOptions.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(1);

// Combining subqueries into one query
SearchQuery query = SearchQuery.CreatePhraseSearchQuery(subquery1, subquery2, subquery3);

// Creating search options object with increased capacity of found occurrences
SearchOptions options = new SearchOptions(); // Overall search options
options.MaxOccurrenceCountPerTerm = 1000000;
options.MaxTotalOccurrenceCount = 10000000;

SearchResult result = index.Search(query, options); // Searching
```

### See Also

* namespace [GroupDocs.Search](../../groupdocs.search)
* assembly [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.search.dll -->
