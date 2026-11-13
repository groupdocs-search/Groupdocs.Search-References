---
title: Search
second_title: GroupDocs.Search for .NET API Reference
description: Searches in the index.
type: docs
weight: 260
url: /net/groupdocs.search/index/search/
---

## Search(string) {#search_3}

Searches in the index.

```csharp
public SearchResult Search(string query)
```

| Parameter | Type | Description |
| --- | --- | --- |
| query | String | The search query. |

### Return Value

The search result.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | The query is `null`. |
| ObjectDisposedException | The index is disposed. |

### Remarks

The errors of a search are reported by the [`ErrorOccurred`](../../../groupdocs.search.events/eventhub/erroroccurred) event of the index, and [`Warnings`](../../../groupdocs.search.results/searchresult/warnings) of the result tells them as well. The method throws an exception only for an argument that is not valid and for a disposed index.

* A query that cannot be parsed or used, search options that cannot be used together and a failure of the search give an empty result, which has no token of the next chunk in a search by chunks.
* A part of the query that cannot be used, for example a regular expression that is not valid, finds nothing, and the other parts of the query are searched.
* A part of the index that cannot be read is passed over, and [`Truncated`](../../../groupdocs.search.results/searchresult/truncated) of the result is `true`.

### Examples

The following example demonstrates how to perform simple search.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

SearchResult result = index.Search(query); // Searching
```

The following example demonstrates how to perform Regex search.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

string query = "^[0-9]{3,}"; // The caret symbol at the beginning of the search query tells the index that it is a Regex query
SearchResult result = index.Search(query); // Searching
```

The following example demonstrates how to perform faceted search.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

string query = "content:Newton"; // The word before the colon in the query means the document field name to search
SearchResult result = index.Search(query); // Searching
```

### See Also

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Search(string, SearchOptions) {#search_4}

Searches in the index.

```csharp
public SearchResult Search(string query, SearchOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| query | String | The search query. |
| options | SearchOptions | The search options. |

### Return Value

The search result.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | The query is `null`. |
| ObjectDisposedException | The index is disposed. |

### Remarks

The errors of a search are reported by the [`ErrorOccurred`](../../../groupdocs.search.events/eventhub/erroroccurred) event of the index, and [`Warnings`](../../../groupdocs.search.results/searchresult/warnings) of the result tells them as well. The method throws an exception only for an argument that is not valid and for a disposed index.

* A query that cannot be parsed or used, search options that cannot be used together and a failure of the search give an empty result, which has no token of the next chunk in a search by chunks.
* A part of the query that cannot be used, for example a regular expression that is not valid, finds nothing, and the other parts of the query are searched.
* A part of the index that cannot be read is passed over, and [`Truncated`](../../../groupdocs.search.results/searchresult/truncated) of the result is `true`.

### Examples

The following example demonstrates how to perform fuzzy search.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

SearchOptions options = new SearchOptions();
options.FuzzySearch.Enabled = true; // Enabling the fuzzy search
options.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(1); // Setting the number of possible differences for each word

// Double quotes at the beginning and end tell the index that it is a phrase search query
string query = "\"The Pursuit of Happiness\"";
SearchResult result = index.Search(query, options); // Searching
```

The following example demonstrates how to perform synonym search.

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

### See Also

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchOptions](../../../groupdocs.search.options/searchoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Search(SearchQuery) {#search_1}

Searches in the index.

```csharp
public SearchResult Search(SearchQuery query)
```

| Parameter | Type | Description |
| --- | --- | --- |
| query | SearchQuery | The search query. |

### Return Value

The search result.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | The query is `null`. |
| ArgumentException | The query cannot be the root of a query: it is a wildcard of words, see [`CreateWildcardQuery`](../../searchquery/createwildcardquery). |
| ObjectDisposedException | The index is disposed. |

### Remarks

The errors of a search are reported by the [`ErrorOccurred`](../../../groupdocs.search.events/eventhub/erroroccurred) event of the index, and [`Warnings`](../../../groupdocs.search.results/searchresult/warnings) of the result tells them as well. The method throws an exception only for an argument that is not valid and for a disposed index.

* A query that cannot be parsed or used, search options that cannot be used together and a failure of the search give an empty result, which has no token of the next chunk in a search by chunks.
* A part of the query that cannot be used, for example a regular expression that is not valid, finds nothing, and the other parts of the query are searched.
* A part of the index that cannot be read is passed over, and [`Truncated`](../../../groupdocs.search.results/searchresult/truncated) of the result is `true`.

### Examples

The following example demonstrates how to perform search using a query in object form.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

// Creating subquery 1
SearchQuery subquery1 = SearchQuery.CreateWordQuery("accommodation");
subquery1.SearchOptions = new SearchOptions(); // Setting search options only for subquery 1
subquery1.SearchOptions.FuzzySearch.Enabled = true; // Enabling the fuzzy search
subquery1.SearchOptions.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(3); // Setting maximum number of differences

// Creating subquery 2
SearchQuery subquery2 = SearchQuery.CreateNumericRangeQuery(1, 1000000);

// Creating subquery 3
SearchQuery subquery3 = SearchQuery.CreateRegexQuery(@"(.)\1");

// Combining subqueries into one query
SearchQuery query = SearchQuery.CreatePhraseSearchQuery(subquery1, subquery2, subquery3);

SearchResult result = index.Search(query); // Searching
```

### See Also

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchQuery](../../searchquery)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Search(SearchQuery, SearchOptions) {#search_2}

Searches in the index.

```csharp
public SearchResult Search(SearchQuery query, SearchOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| query | SearchQuery | The search query. |
| options | SearchOptions | The search options. |

### Return Value

The search result.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | The query is `null`. |
| ArgumentException | The query cannot be the root of a query: it is a wildcard of words, see [`CreateWildcardQuery`](../../searchquery/createwildcardquery). |
| ObjectDisposedException | The index is disposed. |

### Remarks

The errors of a search are reported by the [`ErrorOccurred`](../../../groupdocs.search.events/eventhub/erroroccurred) event of the index, and [`Warnings`](../../../groupdocs.search.results/searchresult/warnings) of the result tells them as well. The method throws an exception only for an argument that is not valid and for a disposed index.

* A query that cannot be parsed or used, search options that cannot be used together and a failure of the search give an empty result, which has no token of the next chunk in a search by chunks.
* A part of the query that cannot be used, for example a regular expression that is not valid, finds nothing, and the other parts of the query are searched.
* A part of the index that cannot be read is passed over, and [`Truncated`](../../../groupdocs.search.results/searchresult/truncated) of the result is `true`.

### Examples

The following example demonstrates how to perform search using a query in object form.

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

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchQuery](../../searchquery)
* class [SearchOptions](../../../groupdocs.search.options/searchoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Search(SearchImage, ImageSearchOptions) {#search}

Performs a reverse image search in the index.

```csharp
public ImageSearchResult Search(SearchImage image, ImageSearchOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| image | SearchImage | The image to search. |
| options | ImageSearchOptions | The image search options. |

### Return Value

The result of a reverse image search.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | The image is `null`. |
| ObjectDisposedException | The index is disposed. |

### Remarks

The result has the found images with the fewest mismatched bits first, at most [`MaxResultCount`](../../../groupdocs.search.options/imagesearchoptions/maxresultcount) of them. The images with the same number of mismatched bits are in the same order in every search while the index is not changed, so a result that the limit cuts has the same images.

### See Also

* class [ImageSearchResult](../../../groupdocs.search.results/imagesearchresult)
* class [SearchImage](../../../groupdocs.search.common/searchimage)
* class [ImageSearchOptions](../../../groupdocs.search.options/imagesearchoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
