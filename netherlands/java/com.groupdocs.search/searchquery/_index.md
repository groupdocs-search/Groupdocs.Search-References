---
title: "SearchQuery"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Stelt een zoekquery in objectvorm voor."
type: docs
weight: 25
url: /nl/java/com.groupdocs.search/searchquery/
---
**Inheritance:**
java.lang.Object
```
public abstract class SearchQuery
```

Stelt een zoekquery in objectvorm voor.


**Learn more**

* [Searching](../https://docs.groupdocs.com/display/searchjava/Searching)
* [Queries in text and object form](../https://docs.groupdocs.com/display/searchjava/Queries+in+text+and+object+form)
* [Nesting search queries in object form](../https://docs.groupdocs.com/display/searchjava/Nesting+search+queries+in+object+form)


Het voorbeeld toont een typisch gebruik van de klasse.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
 
Index index = new Index(indexFolder); // Index aanmaken in de opgegeven map
index.add(documentsFolder); // Documenten indexeren vanuit de opgegeven map
 
// Subquery maken voor datumreeks zoekopdracht
SearchQuery subquery1 = SearchQuery.createDateRangeQuery(new Date(2011, 6, 17), new Date(2013, 1, 1));
 
// Subquery maken voor wildcard met aantal gemiste woorden van 0 tot 2
SearchQuery subquery2 = SearchQuery.createWildcardQuery(0, 2);
 
// Subquery maken voor eenvoudig woord
SearchQuery subquery3 = SearchQuery.createWordQuery("birth");
subquery3.setSearchOptions(new SearchOptions()); // Zoekopties instellen alleen voor subquery 3
subquery3.getSearchOptions().getFuzzySearch().setEnabled(true);
subquery3.getSearchOptions().getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(1));
 
// Subqueries combineren tot één query
SearchQuery query = SearchQuery.createPhraseSearchQuery(subquery1, subquery2, subquery3);
 
// Zoekopties-object maken met verhoogde capaciteit voor gevonden voorkomens
SearchOptions options = new SearchOptions(); // Algemene zoekopties
options.setMaxOccurrenceCountPerTerm(1000000);
options.setMaxTotalOccurrenceCount(10000000);
 
SearchResult result = index.search(query, options); // Zoeken
 
```
 
````


## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getFieldName()](#getFieldName--) | Haalt de veldnaam op. |
|
|  | [getChildCount()](#getChildCount--) | Haalt het aantal subquery's op. |
|
|  | [getFirstChild()](#getFirstChild--) | Haalt de eerste subquery op. |
|
|  | [getSecondChild()](#getSecondChild--) | Haalt de tweede subquery op. |
|
|  | [getChild(int index)](#getChild-int-) | Haalt een subquery op op basis van een index. |
|
|  | [getSearchOptions()](#getSearchOptions--) | Haalt de zoekopties op of stelt ze in voor deze zoekquery. |
|
|  | [setSearchOptions(SearchOptions value)](#setSearchOptions-com.groupdocs.search.options.SearchOptions-) | Haalt de zoekopties op of stelt ze in voor deze zoekquery. |
|
|  | [toString()](#toString--) | Retourneert een  System.String  die de huidige  SearchQuery  instantie vertegenwoordigt. |
|
|  | [createWordQuery(String term)](#createWordQuery-java.lang.String-) | Maakt een eenvoudige woordquery. |
|
|  | [createWordPatternQuery(WordPattern pattern)](#createWordPatternQuery-com.groupdocs.search.common.WordPattern-) | Maakt een woordpatroonquery. |
|
|  | [createRegexQuery(String pattern)](#createRegexQuery-java.lang.String-) | Maakt een reguliere-expressiequery aan. |
|
|  | [createRegexQuery(String pattern, int options)](#createRegexQuery-java.lang.String-int-) | Maakt een reguliere-expressiequery aan. |
|
|  | [createNumericRangeQuery(long start, long end)](#createNumericRangeQuery-long-long-) | Maakt een numerieke bereikquery aan. |
|
|  | [createDateRangeQuery(Date start, Date end)](#createDateRangeQuery-java.util.Date-java.util.Date-) | Maakt een datum‑bereikquery aan. |
|
|  | [createPhraseSearchQuery(SearchQuery[] queries)](#createPhraseSearchQuery-com.groupdocs.search.SearchQuery...-) | Maakt een frase‑zoekquery aan. |
|
|  | [createAndQuery(SearchQuery[] queries)](#createAndQuery-com.groupdocs.search.SearchQuery---) | Maakt een gecombineerde query die alleen documenten vindt die voor elke oorspronkelijke query worden gevonden. |
|
|  | [createFieldQuery(String fieldName, SearchQuery query)](#createFieldQuery-java.lang.String-com.groupdocs.search.SearchQuery-) | Voegt een veld toe aan de opgegeven query. |
|
|  | [createNotQuery(SearchQuery query)](#createNotQuery-com.groupdocs.search.SearchQuery-) | Maakt een omgekeerde query die de overige documenten in een index vindt ten opzichte van diegene die voor de oorspronkelijke query worden gevonden. |
|
|  | [createAndQuery(SearchQuery leftQuery, SearchQuery rightQuery)](#createAndQuery-com.groupdocs.search.SearchQuery-com.groupdocs.search.SearchQuery-) | Maakt een gecombineerde query die alleen documenten vindt die voor elke oorspronkelijke query worden gevonden. |
|
|  | [createOrQuery(SearchQuery leftQuery, SearchQuery rightQuery)](#createOrQuery-com.groupdocs.search.SearchQuery-com.groupdocs.search.SearchQuery-) | Maakt een gecombineerde query die alle documenten vindt die minstens voor één van de oorspronkelijke query's worden gevonden. |
|
|  | [createOrQuery(SearchQuery[] queries)](#createOrQuery-com.groupdocs.search.SearchQuery---) | Maakt een gecombineerde query die alle documenten vindt die minstens voor één van de oorspronkelijke query's worden gevonden. |
|
|  | [createWildcardQuery(int count)](#createWildcardQuery-int-) | Maakt een wildcard voor de frase‑zoekopdracht. |
|
|  | [createWildcardQuery(int minCount, int maxCount)](#createWildcardQuery-int-int-) | Maakt een wildcard voor de frase‑zoekopdracht. |
|
### getFieldName() {#getFieldName--}
```
public String getFieldName()
```


Haalt de veldnaam op.


**Returns:**
java.lang.String - De veldnaam.

### getChildCount() {#getChildCount--}
```
public int getChildCount()
```


Haalt het aantal subquery's op.


**Returns:**
int - Het aantal onderliggende query's.

### getFirstChild() {#getFirstChild--}
```
public SearchQuery getFirstChild()
```


Haalt de eerste subquery op.


**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - The first child query.

### getSecondChild() {#getSecondChild--}
```
public SearchQuery getSecondChild()
```


Haalt de tweede subquery op.


**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - The second child query.

### getChild(int index) {#getChild-int-}
```
public abstract SearchQuery getChild(int index)
```


Haalt een subquery op op basis van een index.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | index | int | De index. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A child query corresponding the specified index.

### getSearchOptions() {#getSearchOptions--}
```
public final SearchOptions getSearchOptions()
```


Haalt de zoekopties op of stelt ze in voor deze zoekquery.


**Returns:**
[SearchOptions](../../com.groupdocs.search.options/searchoptions) - The search options.

### setSearchOptions(SearchOptions value) {#setSearchOptions-com.groupdocs.search.options.SearchOptions-}
```
public final void setSearchOptions(SearchOptions value)
```


Haalt de zoekopties op of stelt ze in voor deze zoekquery.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | value | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | De zoekopties. |
|

### toString() {#toString--}
```
public abstract String toString()
```


Retourneert een  System.String  die de huidige  SearchQuery  instantie vertegenwoordigt.


**Returns:**
java.lang.String - Een System.String die de huidige SearchQuery‑instantie vertegenwoordigt.

### createWordQuery(String term) {#createWordQuery-java.lang.String-}
```
public static SearchQuery createWordQuery(String term)
```


Maakt een eenvoudige woordquery.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | term | java.lang.String | De term om naar te zoeken. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A simple word query.

### createWordPatternQuery(WordPattern pattern) {#createWordPatternQuery-com.groupdocs.search.common.WordPattern-}
```
public static SearchQuery createWordPatternQuery(WordPattern pattern)
```


Maakt een woordpatroonquery.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | pattern | [WordPattern](../../com.groupdocs.search.common/wordpattern) | Het woordpatroon. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A word pattern query.

### createRegexQuery(String pattern) {#createRegexQuery-java.lang.String-}
```
public static SearchQuery createRegexQuery(String pattern)
```


Maakt een reguliere-expressiequery aan.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | pattern | java.lang.String | Het reguliere-expressiepatroon om te matchen. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A regular expression query.

### createRegexQuery(String pattern, int options) {#createRegexQuery-java.lang.String-int-}
```
public static SearchQuery createRegexQuery(String pattern, int options)
```


Maakt een reguliere-expressiequery aan.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | pattern | java.lang.String | Het reguliere-expressiepatroon om te matchen. |
|
|  | options | int | Een bitwise-combinatie van de enumeratiewaarden die de reguliere expressie wijzigen. Deze waarde moet de vlag  RegexOptions.IgnoreCase  bevatten. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A regular expression query.

### createNumericRangeQuery(long start, long end) {#createNumericRangeQuery-long-long-}
```
public static SearchQuery createNumericRangeQuery(long start, long end)
```


Maakt een numerieke bereikquery aan.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | start | long | De startwaarde van een bereik. |
|
|  | end | long | De eindwaarde van een bereik. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A numeric range query.

### createDateRangeQuery(Date start, Date end) {#createDateRangeQuery-java.util.Date-java.util.Date-}
```
public static SearchQuery createDateRangeQuery(Date start, Date end)
```


Maakt een datum‑bereikquery aan.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | start | java.util.Date | De startwaarde van een bereik. |
|
|  | end | java.util.Date | De eindwaarde van een bereik. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A date range query.

### createPhraseSearchQuery(SearchQuery[] queries) {#createPhraseSearchQuery-com.groupdocs.search.SearchQuery...-}
```
public static SearchQuery createPhraseSearchQuery(SearchQuery[] queries)
```


Maakt een frase‑zoekquery aan.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | queries | [SearchQuery\[\]](../../com.groupdocs.search/searchquery) | De onderliggende query's. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A phrase search query.

### createAndQuery(SearchQuery[] queries) {#createAndQuery-com.groupdocs.search.SearchQuery---}
```
public static SearchQuery createAndQuery(SearchQuery[] queries)
```


Maakt een gecombineerde query die alleen documenten vindt die voor elke oorspronkelijke query worden gevonden.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | queries | [SearchQuery\[\]](../../com.groupdocs.search/searchquery) | De veldnaam om in te zoeken. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A combined AND query.

### createFieldQuery(String fieldName, SearchQuery query) {#createFieldQuery-java.lang.String-com.groupdocs.search.SearchQuery-}
```
public static SearchQuery createFieldQuery(String fieldName, SearchQuery query)
```


Voegt een veld toe aan de opgegeven query.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | fieldName | java.lang.String | De veldnaam om in te zoeken. |
|
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | De query om het veld toe te voegen. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A query with the field to search in.

### createNotQuery(SearchQuery query) {#createNotQuery-com.groupdocs.search.SearchQuery-}
```
public static SearchQuery createNotQuery(SearchQuery query)
```


Maakt een omgekeerde query die de overige documenten in een index vindt ten opzichte van diegene die voor de oorspronkelijke query worden gevonden.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | De query om te inverteren. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A combined NOT query.

### createAndQuery(SearchQuery leftQuery, SearchQuery rightQuery) {#createAndQuery-com.groupdocs.search.SearchQuery-com.groupdocs.search.SearchQuery-}
```
public static SearchQuery createAndQuery(SearchQuery leftQuery, SearchQuery rightQuery)
```


Maakt een gecombineerde query die alleen documenten vindt die voor elke oorspronkelijke query worden gevonden.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | leftQuery | [SearchQuery](../../com.groupdocs.search/searchquery) | De linkerkindquery. |
|
|  | rightQuery | [SearchQuery](../../com.groupdocs.search/searchquery) | De rechterkindquery. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A combined AND query.

### createOrQuery(SearchQuery leftQuery, SearchQuery rightQuery) {#createOrQuery-com.groupdocs.search.SearchQuery-com.groupdocs.search.SearchQuery-}
```
public static SearchQuery createOrQuery(SearchQuery leftQuery, SearchQuery rightQuery)
```


Maakt een gecombineerde query die alle documenten vindt die minstens voor één van de oorspronkelijke query's worden gevonden.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | leftQuery | [SearchQuery](../../com.groupdocs.search/searchquery) | De linkerkindquery. |
|
|  | rightQuery | [SearchQuery](../../com.groupdocs.search/searchquery) | De rechterkindquery. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A combined OR query.

### createOrQuery(SearchQuery[] queries) {#createOrQuery-com.groupdocs.search.SearchQuery---}
```
public static SearchQuery createOrQuery(SearchQuery[] queries)
```


Maakt een gecombineerde query die alle documenten vindt die minstens voor één van de oorspronkelijke query's worden gevonden.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | queries | [SearchQuery\[\]](../../com.groupdocs.search/searchquery) | De onderliggende query's. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A combined OR query.

### createWildcardQuery(int count) {#createWildcardQuery-int-}
```
public static SearchQuery createWildcardQuery(int count)
```


Maakt een wildcard voor de frase‑zoekopdracht.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | count | int | Het aantal woorden in de wildcard. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A wildcard for the phrase search.

### createWildcardQuery(int minCount, int maxCount) {#createWildcardQuery-int-int-}
```
public static SearchQuery createWildcardQuery(int minCount, int maxCount)
```


Maakt een wildcard voor de frase‑zoekopdracht.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | minCount | int | Het minimum aantal woorden in de wildcard. |
|
|  | maxCount | int | Het maximum aantal woorden in de wildcard. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A wildcard for the phrase search.

