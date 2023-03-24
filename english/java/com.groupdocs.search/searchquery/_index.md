---
title: SearchQuery
second_title: GroupDocs.Search for Java API Reference
description: Represents a search query in object form.
type: docs
weight: 27
url: /java/com.groupdocs.search/searchquery/
---
**Inheritance:**
java.lang.Object
```
public abstract class SearchQuery
```

Represents a search query in object form.

**Learn more**

 *  [Searching][]
 *  [Queries in text and object form][]
 *  [Nesting search queries in object form][]

The example demonstrates a typical usage of the class.

```

 String indexFolder = "c:\\MyIndex\\";
 String documentsFolder = "c:\\MyDocuments\\";
 Index index = new Index(indexFolder); // Creating index in the specified folder
 index.add(documentsFolder); // Indexing documents from the specified folder
 // Creating subquery of date range search
 SearchQuery subquery1 = SearchQuery.createDateRangeQuery(new Date(2011, 6, 17), new Date(2013, 1, 1));
 // Creating subquery of wildcard with number of missed words from 0 to 2
 SearchQuery subquery2 = SearchQuery.createWildcardQuery(0, 2);
 // Creating subquery of simple word
 SearchQuery subquery3 = SearchQuery.createWordQuery("birth");
 subquery3.setSearchOptions(new SearchOptions()); // Setting search options only for subquery 3
 subquery3.getSearchOptions().getFuzzySearch().setEnabled(true);
 subquery3.getSearchOptions().getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(1));
 // Combining subqueries into one query
 SearchQuery query = SearchQuery.createPhraseSearchQuery(subquery1, subquery2, subquery3);
 // Creating search options object with increased capacity of found occurrences
 SearchOptions options = new SearchOptions(); // Overall search options
 options.setMaxOccurrenceCountPerTerm(1000000);
 options.setMaxTotalOccurrenceCount(10000000);
 SearchResult result = index.search(query, options); // Searching
 
```


[Searching]: https://docs.groupdocs.com/display/searchjava/Searching
[Queries in text and object form]: https://docs.groupdocs.com/display/searchjava/Queries+in+text+and+object+form
[Nesting search queries in object form]: https://docs.groupdocs.com/display/searchjava/Nesting+search+queries+in+object+form
## Methods

| Method | Description |
| --- | --- |
| [getFieldName()](#getFieldName--) | Gets the field name. |
| [getChildCount()](#getChildCount--) | Gets the number of child queries. |
| [getFirstChild()](#getFirstChild--) | Gets the first child query. |
| [getSecondChild()](#getSecondChild--) | Gets the second child query. |
| [getChild(int index)](#getChild-int-) | Gets a child query by an index. |
| [getSearchOptions()](#getSearchOptions--) | Gets the search options of this seach query. |
| [setSearchOptions(SearchOptions value)](#setSearchOptions-com.groupdocs.search.options.SearchOptions-) | Sets the search options of this seach query. |
| [toString()](#toString--) | Returns a String that represents the current  SearchQuery  instance. |
| [createWordQuery(String term)](#createWordQuery-java.lang.String-) | Creates a simple word query. |
| [createWordPatternQuery(WordPattern pattern)](#createWordPatternQuery-com.groupdocs.search.common.WordPattern-) | Creates a word pattern query. |
| [createRegexQuery(String pattern)](#createRegexQuery-java.lang.String-) | Creates a regular expression query. |
| [createRegexQuery(String pattern, int options)](#createRegexQuery-java.lang.String-int-) | Creates a regular expression query. |
| [createNumericRangeQuery(long start, long end)](#createNumericRangeQuery-long-long-) | Creates a numeric range query. |
| [createDateRangeQuery(Date start, Date end)](#createDateRangeQuery-java.util.Date-java.util.Date-) | Creates a date range query. |
| [createPhraseSearchQuery(SearchQuery[] queries)](#createPhraseSearchQuery-com.groupdocs.search.SearchQuery...-) | Creates a phrase search query. |
| [createFieldQuery(String fieldName, SearchQuery query)](#createFieldQuery-java.lang.String-com.groupdocs.search.SearchQuery-) | Adds a field to the specified query. |
| [createNotQuery(SearchQuery query)](#createNotQuery-com.groupdocs.search.SearchQuery-) | Creates an inverted query that will find the rest documents in an index against ones which will be found for the original query. |
| [createAndQuery(SearchQuery leftQuery, SearchQuery rightQuery)](#createAndQuery-com.groupdocs.search.SearchQuery-com.groupdocs.search.SearchQuery-) | Creates a combined query that will find only documents which will be found for each original query. |
| [createOrQuery(SearchQuery leftQuery, SearchQuery rightQuery)](#createOrQuery-com.groupdocs.search.SearchQuery-com.groupdocs.search.SearchQuery-) | Creates a combined query that will find all the documents which will be found at least for one of the original queries. |
| [createWildcardQuery(int count)](#createWildcardQuery-int-) | Creates a wildcard for the phrase search. |
| [createWildcardQuery(int minCount, int maxCount)](#createWildcardQuery-int-int-) | Creates a wildcard for the phrase search. |
### getFieldName() {#getFieldName--}
```
public String getFieldName()
```


Gets the field name.

**Returns:**
java.lang.String - The field name.
### getChildCount() {#getChildCount--}
```
public int getChildCount()
```


Gets the number of child queries.

**Returns:**
int - The number of child queries.
### getFirstChild() {#getFirstChild--}
```
public SearchQuery getFirstChild()
```


Gets the first child query.

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - The first child query.
### getSecondChild() {#getSecondChild--}
```
public SearchQuery getSecondChild()
```


Gets the second child query.

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - The second child query.
### getChild(int index) {#getChild-int-}
```
public abstract SearchQuery getChild(int index)
```


Gets a child query by an index.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The index. |

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A child query corresponding the specified index.
### getSearchOptions() {#getSearchOptions--}
```
public final SearchOptions getSearchOptions()
```


Gets the search options of this seach query.

**Returns:**
[SearchOptions](../../com.groupdocs.search.options/searchoptions) - The search options.
### setSearchOptions(SearchOptions value) {#setSearchOptions-com.groupdocs.search.options.SearchOptions-}
```
public final void setSearchOptions(SearchOptions value)
```


Sets the search options of this seach query.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | The search options. |

### toString() {#toString--}
```
public abstract String toString()
```


Returns a String that represents the current  SearchQuery  instance.

**Returns:**
java.lang.String - A String that represents the current  SearchQuery  instance.
### createWordQuery(String term) {#createWordQuery-java.lang.String-}
```
public static SearchQuery createWordQuery(String term)
```


Creates a simple word query.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| term | java.lang.String | The term to search for. |

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A simple word query.
### createWordPatternQuery(WordPattern pattern) {#createWordPatternQuery-com.groupdocs.search.common.WordPattern-}
```
public static SearchQuery createWordPatternQuery(WordPattern pattern)
```


Creates a word pattern query.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pattern | [WordPattern](../../com.groupdocs.search.common/wordpattern) | The word pattern. |

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A word pattern query.
### createRegexQuery(String pattern) {#createRegexQuery-java.lang.String-}
```
public static SearchQuery createRegexQuery(String pattern)
```


Creates a regular expression query.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pattern | java.lang.String | The regular expression pattern to match. |

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A regular expression query.
### createRegexQuery(String pattern, int options) {#createRegexQuery-java.lang.String-int-}
```
public static SearchQuery createRegexQuery(String pattern, int options)
```


Creates a regular expression query.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pattern | java.lang.String | The regular expression pattern to match. |
| options | int | A bitwise combination of the enumeration values that modify the regular expression. This value must contain  RegexOptions.IgnoreCase  flag. |

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A regular expression query.
### createNumericRangeQuery(long start, long end) {#createNumericRangeQuery-long-long-}
```
public static SearchQuery createNumericRangeQuery(long start, long end)
```


Creates a numeric range query.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| start | long | The start value of a range. |
| end | long | The end value of a range. |

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A numeric range query.
### createDateRangeQuery(Date start, Date end) {#createDateRangeQuery-java.util.Date-java.util.Date-}
```
public static SearchQuery createDateRangeQuery(Date start, Date end)
```


Creates a date range query.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| start | java.util.Date | The start value of a range. |
| end | java.util.Date | The end value of a range. |

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A date range query.
### createPhraseSearchQuery(SearchQuery[] queries) {#createPhraseSearchQuery-com.groupdocs.search.SearchQuery...-}
```
public static SearchQuery createPhraseSearchQuery(SearchQuery[] queries)
```


Creates a phrase search query.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| queries | [SearchQuery\[\]](../../com.groupdocs.search/searchquery) | The child queries. |

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A phrase search query.
### createFieldQuery(String fieldName, SearchQuery query) {#createFieldQuery-java.lang.String-com.groupdocs.search.SearchQuery-}
```
public static SearchQuery createFieldQuery(String fieldName, SearchQuery query)
```


Adds a field to the specified query.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fieldName | java.lang.String | The field name to search in. |
| query | [SearchQuery](../../com.groupdocs.search/searchquery) | The query to add the field. |

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A query with the field to search in.
### createNotQuery(SearchQuery query) {#createNotQuery-com.groupdocs.search.SearchQuery-}
```
public static SearchQuery createNotQuery(SearchQuery query)
```


Creates an inverted query that will find the rest documents in an index against ones which will be found for the original query.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| query | [SearchQuery](../../com.groupdocs.search/searchquery) | The query to invert. |

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A combined NOT query.
### createAndQuery(SearchQuery leftQuery, SearchQuery rightQuery) {#createAndQuery-com.groupdocs.search.SearchQuery-com.groupdocs.search.SearchQuery-}
```
public static SearchQuery createAndQuery(SearchQuery leftQuery, SearchQuery rightQuery)
```


Creates a combined query that will find only documents which will be found for each original query.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| leftQuery | [SearchQuery](../../com.groupdocs.search/searchquery) | The left child query. |
| rightQuery | [SearchQuery](../../com.groupdocs.search/searchquery) | The right child query. |

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A combined AND query.
### createOrQuery(SearchQuery leftQuery, SearchQuery rightQuery) {#createOrQuery-com.groupdocs.search.SearchQuery-com.groupdocs.search.SearchQuery-}
```
public static SearchQuery createOrQuery(SearchQuery leftQuery, SearchQuery rightQuery)
```


Creates a combined query that will find all the documents which will be found at least for one of the original queries.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| leftQuery | [SearchQuery](../../com.groupdocs.search/searchquery) | The left child query. |
| rightQuery | [SearchQuery](../../com.groupdocs.search/searchquery) | The right child query. |

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A combined OR query.
### createWildcardQuery(int count) {#createWildcardQuery-int-}
```
public static SearchQuery createWildcardQuery(int count)
```


Creates a wildcard for the phrase search.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| count | int | The number of words in the wildcard. |

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A wildcard for the phrase search.
### createWildcardQuery(int minCount, int maxCount) {#createWildcardQuery-int-int-}
```
public static SearchQuery createWildcardQuery(int minCount, int maxCount)
```


Creates a wildcard for the phrase search.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| minCount | int | The minimum number of words in the wildcard. |
| maxCount | int | The maximum number of words in the wildcard. |

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A wildcard for the phrase search.
