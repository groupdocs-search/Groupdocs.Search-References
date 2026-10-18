---
title: "SearchQuery"
second_title: "GroupDocs.Search för Java API-referens"
description: "Representerar en sökfråga i objektform."
type: docs
weight: 25
url: /sv/java/com.groupdocs.search/searchquery/
---
**Inheritance:**
java.lang.Object
```
public abstract class SearchQuery
```

Representerar en sökfråga i objektform.


**Learn more**

* [Searching](../https://docs.groupdocs.com/display/searchjava/Searching)
* [Queries in text and object form](../https://docs.groupdocs.com/display/searchjava/Queries+in+text+and+object+form)
* [Nesting search queries in object form](../https://docs.groupdocs.com/display/searchjava/Nesting+search+queries+in+object+form)


Exemplet demonstrerar ett typiskt användningssätt av klassen.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
 
Index index = new Index(indexFolder); // Skapar index i den angivna mappen
index.add(documentsFolder); // Indexerar dokument från den angivna mappen
 
// Skapar delfråga för datumintervallssökning
SearchQuery subquery1 = SearchQuery.createDateRangeQuery(new Date(2011, 6, 17), new Date(2013, 1, 1));
 
// Skapar delfråga för jokertecken med antal missade ord från 0 till 2
SearchQuery subquery2 = SearchQuery.createWildcardQuery(0, 2);
 
// Skapar delfråga för enkelt ord
SearchQuery subquery3 = SearchQuery.createWordQuery("birth");
subquery3.setSearchOptions(new SearchOptions()); // Ställer in sökalternativ endast för delfråga 3
subquery3.getSearchOptions().getFuzzySearch().setEnabled(true);
subquery3.getSearchOptions().getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(1));
 
// Kombinerar delfrågor till en fråga
SearchQuery query = SearchQuery.createPhraseSearchQuery(subquery1, subquery2, subquery3);
 
// Skapar sökalternativobjekt med ökad kapacitet för funna förekomster
SearchOptions options = new SearchOptions(); // Övergripande sökalternativ
options.setMaxOccurrenceCountPerTerm(1000000);
options.setMaxTotalOccurrenceCount(10000000);
 
SearchResult result = index.search(query, options); // Söker
 
```
 
````


## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getFieldName()](#getFieldName--) | Hämtar fältnamnet. |
|
|  | [getChildCount()](#getChildCount--) | Hämtar antalet underfrågor. |
|
|  | [getFirstChild()](#getFirstChild--) | Hämtar den första underfrågan. |
|
|  | [getSecondChild()](#getSecondChild--) | Hämtar den andra underfrågan. |
|
|  | [getChild(int index)](#getChild-int-) | Hämtar en underfråga efter ett index. |
|
|  | [getSearchOptions()](#getSearchOptions--) | Hämtar eller anger sökalternativen för denna sökfråga. |
|
|  | [setSearchOptions(SearchOptions value)](#setSearchOptions-com.groupdocs.search.options.SearchOptions-) | Hämtar eller anger sökalternativen för denna sökfråga. |
|
|  | [toString()](#toString--) | Returnerar en  System.String  som representerar den aktuella  SearchQuery  -instansen. |
|
|  | [createWordQuery(String term)](#createWordQuery-java.lang.String-) | Skapar en enkel ordfråga. |
|
|  | [createWordPatternQuery(WordPattern pattern)](#createWordPatternQuery-com.groupdocs.search.common.WordPattern-) | Skapar en ordmönsterfråga. |
|
|  | [createRegexQuery(String pattern)](#createRegexQuery-java.lang.String-) | Skapar en fråga med reguljärt uttryck. |
|
|  | [createRegexQuery(String pattern, int options)](#createRegexQuery-java.lang.String-int-) | Skapar en fråga med reguljärt uttryck. |
|
|  | [createNumericRangeQuery(long start, long end)](#createNumericRangeQuery-long-long-) | Skapar en numerisk intervallfråga. |
|
|  | [createDateRangeQuery(Date start, Date end)](#createDateRangeQuery-java.util.Date-java.util.Date-) | Skapar en datumintervallfråga. |
|
|  | [createPhraseSearchQuery(SearchQuery[] queries)](#createPhraseSearchQuery-com.groupdocs.search.SearchQuery...-) | Skapar en fras-sökfråga. |
|
|  | [createAndQuery(SearchQuery[] queries)](#createAndQuery-com.groupdocs.search.SearchQuery---) | Skapar en kombinerad fråga som endast hittar dokument som hittas för varje ursprunglig fråga. |
|
|  | [createFieldQuery(String fieldName, SearchQuery query)](#createFieldQuery-java.lang.String-com.groupdocs.search.SearchQuery-) | Lägger till ett fält i den angivna frågan. |
|
|  | [createNotQuery(SearchQuery query)](#createNotQuery-com.groupdocs.search.SearchQuery-) | Skapar en inverterad fråga som hittar de återstående dokumenten i ett index i förhållande till de som hittas för den ursprungliga frågan. |
|
|  | [createAndQuery(SearchQuery leftQuery, SearchQuery rightQuery)](#createAndQuery-com.groupdocs.search.SearchQuery-com.groupdocs.search.SearchQuery-) | Skapar en kombinerad fråga som endast hittar dokument som hittas för varje ursprunglig fråga. |
|
|  | [createOrQuery(SearchQuery leftQuery, SearchQuery rightQuery)](#createOrQuery-com.groupdocs.search.SearchQuery-com.groupdocs.search.SearchQuery-) | Skapar en kombinerad fråga som hittar alla dokument som hittas åtminstone av en av de ursprungliga frågorna. |
|
|  | [createOrQuery(SearchQuery[] queries)](#createOrQuery-com.groupdocs.search.SearchQuery---) | Skapar en kombinerad fråga som hittar alla dokument som hittas åtminstone av en av de ursprungliga frågorna. |
|
|  | [createWildcardQuery(int count)](#createWildcardQuery-int-) | Skapar ett jokertecken för fras-sökning. |
|
|  | [createWildcardQuery(int minCount, int maxCount)](#createWildcardQuery-int-int-) | Skapar ett jokertecken för fras-sökning. |
|
### getFieldName() {#getFieldName--}
```
public String getFieldName()
```


Hämtar fältnamnet.


**Returns:**
java.lang.String - Fältnamnet.

### getChildCount() {#getChildCount--}
```
public int getChildCount()
```


Hämtar antalet underfrågor.


**Returns:**
int - Antalet underfrågor.

### getFirstChild() {#getFirstChild--}
```
public SearchQuery getFirstChild()
```


Hämtar den första underfrågan.


**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - The first child query.

### getSecondChild() {#getSecondChild--}
```
public SearchQuery getSecondChild()
```


Hämtar den andra underfrågan.


**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - The second child query.

### getChild(int index) {#getChild-int-}
```
public abstract SearchQuery getChild(int index)
```


Hämtar en underfråga efter ett index.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | index | int | Indexet. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A child query corresponding the specified index.

### getSearchOptions() {#getSearchOptions--}
```
public final SearchOptions getSearchOptions()
```


Hämtar eller anger sökalternativen för denna sökfråga.


**Returns:**
[SearchOptions](../../com.groupdocs.search.options/searchoptions) - The search options.

### setSearchOptions(SearchOptions value) {#setSearchOptions-com.groupdocs.search.options.SearchOptions-}
```
public final void setSearchOptions(SearchOptions value)
```


Hämtar eller anger sökalternativen för denna sökfråga.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | value | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | Sökalternativen. |
|

### toString() {#toString--}
```
public abstract String toString()
```


Returnerar en  System.String  som representerar den aktuella  SearchQuery  -instansen.


**Returns:**
java.lang.String - En System.String som representerar den aktuella SearchQuery-instansen.

### createWordQuery(String term) {#createWordQuery-java.lang.String-}
```
public static SearchQuery createWordQuery(String term)
```


Skapar en enkel ordfråga.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | term | java.lang.String | Termen att söka efter. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A simple word query.

### createWordPatternQuery(WordPattern pattern) {#createWordPatternQuery-com.groupdocs.search.common.WordPattern-}
```
public static SearchQuery createWordPatternQuery(WordPattern pattern)
```


Skapar en ordmönsterfråga.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | pattern | [WordPattern](../../com.groupdocs.search.common/wordpattern) | Mönstret för ordet. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A word pattern query.

### createRegexQuery(String pattern) {#createRegexQuery-java.lang.String-}
```
public static SearchQuery createRegexQuery(String pattern)
```


Skapar en fråga med reguljärt uttryck.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | pattern | java.lang.String | Det reguljära uttrycksmönstret att matcha. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A regular expression query.

### createRegexQuery(String pattern, int options) {#createRegexQuery-java.lang.String-int-}
```
public static SearchQuery createRegexQuery(String pattern, int options)
```


Skapar en fråga med reguljärt uttryck.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | pattern | java.lang.String | Det reguljära uttrycksmönstret att matcha. |
|
|  | options | int | En bitvis kombination av uppräkningens värden som modifierar reguljärt uttryck. Detta värde måste innehålla flaggan  RegexOptions.IgnoreCase. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A regular expression query.

### createNumericRangeQuery(long start, long end) {#createNumericRangeQuery-long-long-}
```
public static SearchQuery createNumericRangeQuery(long start, long end)
```


Skapar en numerisk intervallfråga.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | start | long | Startvärdet för ett intervall. |
|
|  | end | long | Slutvärdet för ett intervall. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A numeric range query.

### createDateRangeQuery(Date start, Date end) {#createDateRangeQuery-java.util.Date-java.util.Date-}
```
public static SearchQuery createDateRangeQuery(Date start, Date end)
```


Skapar en datumintervallfråga.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | start | java.util.Date | Startvärdet för ett intervall. |
|
|  | end | java.util.Date | Slutvärdet för ett intervall. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A date range query.

### createPhraseSearchQuery(SearchQuery[] queries) {#createPhraseSearchQuery-com.groupdocs.search.SearchQuery...-}
```
public static SearchQuery createPhraseSearchQuery(SearchQuery[] queries)
```


Skapar en fras-sökfråga.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | queries | [SearchQuery\[\]](../../com.groupdocs.search/searchquery) | Underfrågorna. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A phrase search query.

### createAndQuery(SearchQuery[] queries) {#createAndQuery-com.groupdocs.search.SearchQuery---}
```
public static SearchQuery createAndQuery(SearchQuery[] queries)
```


Skapar en kombinerad fråga som endast hittar dokument som hittas för varje ursprunglig fråga.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | queries | [SearchQuery\[\]](../../com.groupdocs.search/searchquery) | Fältnamnet att söka i. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A combined AND query.

### createFieldQuery(String fieldName, SearchQuery query) {#createFieldQuery-java.lang.String-com.groupdocs.search.SearchQuery-}
```
public static SearchQuery createFieldQuery(String fieldName, SearchQuery query)
```


Lägger till ett fält i den angivna frågan.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | fieldName | java.lang.String | Fältnamnet att söka i. |
|
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | Frågan för att lägga till fältet. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A query with the field to search in.

### createNotQuery(SearchQuery query) {#createNotQuery-com.groupdocs.search.SearchQuery-}
```
public static SearchQuery createNotQuery(SearchQuery query)
```


Skapar en inverterad fråga som hittar de återstående dokumenten i ett index i förhållande till de som hittas för den ursprungliga frågan.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | Frågan för att invertera. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A combined NOT query.

### createAndQuery(SearchQuery leftQuery, SearchQuery rightQuery) {#createAndQuery-com.groupdocs.search.SearchQuery-com.groupdocs.search.SearchQuery-}
```
public static SearchQuery createAndQuery(SearchQuery leftQuery, SearchQuery rightQuery)
```


Skapar en kombinerad fråga som endast hittar dokument som hittas för varje ursprunglig fråga.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | leftQuery | [SearchQuery](../../com.groupdocs.search/searchquery) | Den vänstra barnfrågan. |
|
|  | rightQuery | [SearchQuery](../../com.groupdocs.search/searchquery) | Den högra barnfrågan. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A combined AND query.

### createOrQuery(SearchQuery leftQuery, SearchQuery rightQuery) {#createOrQuery-com.groupdocs.search.SearchQuery-com.groupdocs.search.SearchQuery-}
```
public static SearchQuery createOrQuery(SearchQuery leftQuery, SearchQuery rightQuery)
```


Skapar en kombinerad fråga som hittar alla dokument som hittas åtminstone av en av de ursprungliga frågorna.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | leftQuery | [SearchQuery](../../com.groupdocs.search/searchquery) | Den vänstra barnfrågan. |
|
|  | rightQuery | [SearchQuery](../../com.groupdocs.search/searchquery) | Den högra barnfrågan. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A combined OR query.

### createOrQuery(SearchQuery[] queries) {#createOrQuery-com.groupdocs.search.SearchQuery---}
```
public static SearchQuery createOrQuery(SearchQuery[] queries)
```


Skapar en kombinerad fråga som hittar alla dokument som hittas åtminstone av en av de ursprungliga frågorna.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | queries | [SearchQuery\[\]](../../com.groupdocs.search/searchquery) | Underfrågorna. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A combined OR query.

### createWildcardQuery(int count) {#createWildcardQuery-int-}
```
public static SearchQuery createWildcardQuery(int count)
```


Skapar ett jokertecken för fras-sökning.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | count | int | Antalet ord i jokertecknet. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A wildcard for the phrase search.

### createWildcardQuery(int minCount, int maxCount) {#createWildcardQuery-int-int-}
```
public static SearchQuery createWildcardQuery(int minCount, int maxCount)
```


Skapar ett jokertecken för fras-sökning.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | minCount | int | Det minsta antalet ord i jokertecknet. |
|
|  | maxCount | int | Det största antalet ord i jokertecknet. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A wildcard for the phrase search.

