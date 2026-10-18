---
title: "SearchQuery"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Stellt eine Suchabfrage in Objektform dar."
type: docs
weight: 25
url: /de/java/com.groupdocs.search/searchquery/
---
**Inheritance:**
java.lang.Object
```
public abstract class SearchQuery
```

Stellt eine Suchabfrage in Objektform dar.


**Learn more**

* [Searching](../https://docs.groupdocs.com/display/searchjava/Searching)
* [Queries in text and object form](../https://docs.groupdocs.com/display/searchjava/Queries+in+text+and+object+form)
* [Nesting search queries in object form](../https://docs.groupdocs.com/display/searchjava/Nesting+search+queries+in+object+form)


Das Beispiel demonstriert eine typische Verwendung der Klasse.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
 
Index index = new Index(indexFolder); // Erstellen des Index im angegebenen Ordner
index.add(documentsFolder); // Indizieren von Dokumenten aus dem angegebenen Ordner
 
// Erstellen einer Unterabfrage für die Datumsspanne-Suche
SearchQuery subquery1 = SearchQuery.createDateRangeQuery(new Date(2011, 6, 17), new Date(2013, 1, 1));
 
// Erstellen einer Unterabfrage für Wildcard mit einer Anzahl fehlender Wörter von 0 bis 2
SearchQuery subquery2 = SearchQuery.createWildcardQuery(0, 2);
 
// Erstellen einer Unterabfrage für ein einfaches Wort
SearchQuery subquery3 = SearchQuery.createWordQuery("birth");
subquery3.setSearchOptions(new SearchOptions()); // Festlegen der Suchoptionen nur für Unterabfrage 3
subquery3.getSearchOptions().getFuzzySearch().setEnabled(true);
subquery3.getSearchOptions().getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(1));
 
// Kombinieren von Unterabfragen zu einer Abfrage
SearchQuery query = SearchQuery.createPhraseSearchQuery(subquery1, subquery2, subquery3);
 
// Erstellen eines Suchoptionen-Objekts mit erhöhter Kapazität gefundener Vorkommen
SearchOptions options = new SearchOptions(); // Gesamte Suchoptionen
options.setMaxOccurrenceCountPerTerm(1000000);
options.setMaxTotalOccurrenceCount(10000000);
 
SearchResult result = index.search(query, options); // Suche
 
```
 
````


## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getFieldName()](#getFieldName--) | Liefert den Feldnamen. |
|
|  | [getChildCount()](#getChildCount--) | Liefert die Anzahl der Unterabfragen. |
|
|  | [getFirstChild()](#getFirstChild--) | Liefert die erste Unterabfrage. |
|
|  | [getSecondChild()](#getSecondChild--) | Liefert die zweite Unterabfrage. |
|
|  | [getChild(int index)](#getChild-int-) | Liefert eine Unterabfrage anhand eines Index. |
|
|  | [getSearchOptions()](#getSearchOptions--) | Liefert oder setzt die Suchoptionen dieser Suchabfrage. |
|
|  | [setSearchOptions(SearchOptions value)](#setSearchOptions-com.groupdocs.search.options.SearchOptions-) | Liefert oder setzt die Suchoptionen dieser Suchabfrage. |
|
|  | [toString()](#toString--) | Gibt einen  System.String  zurück, der die aktuelle  SearchQuery  Instanz darstellt. |
|
|  | [createWordQuery(String term)](#createWordQuery-java.lang.String-) | Erstellt eine einfache Wortabfrage. |
|
|  | [createWordPatternQuery(WordPattern pattern)](#createWordPatternQuery-com.groupdocs.search.common.WordPattern-) | Erstellt eine Wortmuster-Abfrage. |
|
|  | [createRegexQuery(String pattern)](#createRegexQuery-java.lang.String-) | Erstellt eine reguläre Ausdruck-Abfrage. |
|
|  | [createRegexQuery(String pattern, int options)](#createRegexQuery-java.lang.String-int-) | Erstellt eine reguläre Ausdruck-Abfrage. |
|
|  | [createNumericRangeQuery(long start, long end)](#createNumericRangeQuery-long-long-) | Erstellt eine numerische Bereichsabfrage. |
|
|  | [createDateRangeQuery(Date start, Date end)](#createDateRangeQuery-java.util.Date-java.util.Date-) | Erstellt eine Datumsbereichsabfrage. |
|
|  | [createPhraseSearchQuery(SearchQuery[] queries)](#createPhraseSearchQuery-com.groupdocs.search.SearchQuery...-) | Erstellt eine Phrasensuchabfrage. |
|
|  | [createAndQuery(SearchQuery[] queries)](#createAndQuery-com.groupdocs.search.SearchQuery---) | Erstellt eine kombinierte Abfrage, die nur Dokumente findet, die für jede ursprüngliche Abfrage gefunden werden. |
|
|  | [createFieldQuery(String fieldName, SearchQuery query)](#createFieldQuery-java.lang.String-com.groupdocs.search.SearchQuery-) | Fügt ein Feld zur angegebenen Abfrage hinzu. |
|
|  | [createNotQuery(SearchQuery query)](#createNotQuery-com.groupdocs.search.SearchQuery-) | Erstellt eine invertierte Abfrage, die die restlichen Dokumente in einem Index im Vergleich zu denen findet, die für die ursprüngliche Abfrage gefunden werden. |
|
|  | [createAndQuery(SearchQuery leftQuery, SearchQuery rightQuery)](#createAndQuery-com.groupdocs.search.SearchQuery-com.groupdocs.search.SearchQuery-) | Erstellt eine kombinierte Abfrage, die nur Dokumente findet, die für jede ursprüngliche Abfrage gefunden werden. |
|
|  | [createOrQuery(SearchQuery leftQuery, SearchQuery rightQuery)](#createOrQuery-com.groupdocs.search.SearchQuery-com.groupdocs.search.SearchQuery-) | Erstellt eine kombinierte Abfrage, die alle Dokumente findet, die mindestens für eine der ursprünglichen Abfragen gefunden werden. |
|
|  | [createOrQuery(SearchQuery[] queries)](#createOrQuery-com.groupdocs.search.SearchQuery---) | Erstellt eine kombinierte Abfrage, die alle Dokumente findet, die mindestens für eine der ursprünglichen Abfragen gefunden werden. |
|
|  | [createWildcardQuery(int count)](#createWildcardQuery-int-) | Erstellt ein Platzhalterzeichen für die Phrasensuche. |
|
|  | [createWildcardQuery(int minCount, int maxCount)](#createWildcardQuery-int-int-) | Erstellt ein Platzhalterzeichen für die Phrasensuche. |
|
### getFieldName() {#getFieldName--}
```
public String getFieldName()
```


Liefert den Feldnamen.


**Returns:**
java.lang.String - Der Feldname.

### getChildCount() {#getChildCount--}
```
public int getChildCount()
```


Liefert die Anzahl der Unterabfragen.


**Returns:**
int - Die Anzahl der untergeordneten Abfragen.

### getFirstChild() {#getFirstChild--}
```
public SearchQuery getFirstChild()
```


Liefert die erste Unterabfrage.


**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - The first child query.

### getSecondChild() {#getSecondChild--}
```
public SearchQuery getSecondChild()
```


Liefert die zweite Unterabfrage.


**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - The second child query.

### getChild(int index) {#getChild-int-}
```
public abstract SearchQuery getChild(int index)
```


Liefert eine Unterabfrage anhand eines Index.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Index | int | Der Index. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A child query corresponding the specified index.

### getSearchOptions() {#getSearchOptions--}
```
public final SearchOptions getSearchOptions()
```


Liefert oder setzt die Suchoptionen dieser Suchabfrage.


**Returns:**
[SearchOptions](../../com.groupdocs.search.options/searchoptions) - The search options.

### setSearchOptions(SearchOptions value) {#setSearchOptions-com.groupdocs.search.options.SearchOptions-}
```
public final void setSearchOptions(SearchOptions value)
```


Liefert oder setzt die Suchoptionen dieser Suchabfrage.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | value | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | Die Suchoptionen. |
|

### toString() {#toString--}
```
public abstract String toString()
```


Gibt einen  System.String  zurück, der die aktuelle  SearchQuery  Instanz darstellt.


**Returns:**
java.lang.String - Ein  System.String  der die aktuelle  SearchQuery  Instanz darstellt.

### createWordQuery(String term) {#createWordQuery-java.lang.String-}
```
public static SearchQuery createWordQuery(String term)
```


Erstellt eine einfache Wortabfrage.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Begriff | java.lang.String | Der zu suchende Begriff. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A simple word query.

### createWordPatternQuery(WordPattern pattern) {#createWordPatternQuery-com.groupdocs.search.common.WordPattern-}
```
public static SearchQuery createWordPatternQuery(WordPattern pattern)
```


Erstellt eine Wortmuster-Abfrage.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | pattern | [WordPattern](../../com.groupdocs.search.common/wordpattern) | Das Wortmuster. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A word pattern query.

### createRegexQuery(String pattern) {#createRegexQuery-java.lang.String-}
```
public static SearchQuery createRegexQuery(String pattern)
```


Erstellt eine reguläre Ausdruck-Abfrage.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | pattern | java.lang.String | Das reguläre Ausdrucksmuster zum Abgleichen. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A regular expression query.

### createRegexQuery(String pattern, int options) {#createRegexQuery-java.lang.String-int-}
```
public static SearchQuery createRegexQuery(String pattern, int options)
```


Erstellt eine reguläre Ausdruck-Abfrage.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | pattern | java.lang.String | Das reguläre Ausdrucksmuster zum Abgleichen. |
|
|  | options | int | Eine bitweise Kombination der Aufzählungswerte, die den regulären Ausdruck modifizieren. Dieser Wert muss das  RegexOptions.IgnoreCase  Flag enthalten. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A regular expression query.

### createNumericRangeQuery(long start, long end) {#createNumericRangeQuery-long-long-}
```
public static SearchQuery createNumericRangeQuery(long start, long end)
```


Erstellt eine numerische Bereichsabfrage.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Start | long | Der Startwert eines Bereichs. |
|
|  | Ende | long | Der Endwert eines Bereichs. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A numeric range query.

### createDateRangeQuery(Date start, Date end) {#createDateRangeQuery-java.util.Date-java.util.Date-}
```
public static SearchQuery createDateRangeQuery(Date start, Date end)
```


Erstellt eine Datumsbereichsabfrage.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Start | java.util.Date | Der Startwert eines Bereichs. |
|
|  | Ende | java.util.Date | Der Endwert eines Bereichs. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A date range query.

### createPhraseSearchQuery(SearchQuery[] queries) {#createPhraseSearchQuery-com.groupdocs.search.SearchQuery...-}
```
public static SearchQuery createPhraseSearchQuery(SearchQuery[] queries)
```


Erstellt eine Phrasensuchabfrage.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | queries | [SearchQuery\[\]](../../com.groupdocs.search/searchquery) | Die untergeordneten Abfragen. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A phrase search query.

### createAndQuery(SearchQuery[] queries) {#createAndQuery-com.groupdocs.search.SearchQuery---}
```
public static SearchQuery createAndQuery(SearchQuery[] queries)
```


Erstellt eine kombinierte Abfrage, die nur Dokumente findet, die für jede ursprüngliche Abfrage gefunden werden.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | queries | [SearchQuery\[\]](../../com.groupdocs.search/searchquery) | Der Feldname, in dem gesucht wird. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A combined AND query.

### createFieldQuery(String fieldName, SearchQuery query) {#createFieldQuery-java.lang.String-com.groupdocs.search.SearchQuery-}
```
public static SearchQuery createFieldQuery(String fieldName, SearchQuery query)
```


Fügt ein Feld zur angegebenen Abfrage hinzu.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | fieldName | java.lang.String | Der Feldname, in dem gesucht wird. |
|
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | Die Abfrage, um das Feld hinzuzufügen. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A query with the field to search in.

### createNotQuery(SearchQuery query) {#createNotQuery-com.groupdocs.search.SearchQuery-}
```
public static SearchQuery createNotQuery(SearchQuery query)
```


Erstellt eine invertierte Abfrage, die die restlichen Dokumente in einem Index im Vergleich zu denen findet, die für die ursprüngliche Abfrage gefunden werden.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | Die Abfrage zum Invertieren. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A combined NOT query.

### createAndQuery(SearchQuery leftQuery, SearchQuery rightQuery) {#createAndQuery-com.groupdocs.search.SearchQuery-com.groupdocs.search.SearchQuery-}
```
public static SearchQuery createAndQuery(SearchQuery leftQuery, SearchQuery rightQuery)
```


Erstellt eine kombinierte Abfrage, die nur Dokumente findet, die für jede ursprüngliche Abfrage gefunden werden.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | leftQuery | [SearchQuery](../../com.groupdocs.search/searchquery) | Die linke Kindabfrage. |
|
|  | rightQuery | [SearchQuery](../../com.groupdocs.search/searchquery) | Die rechte Kindabfrage. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A combined AND query.

### createOrQuery(SearchQuery leftQuery, SearchQuery rightQuery) {#createOrQuery-com.groupdocs.search.SearchQuery-com.groupdocs.search.SearchQuery-}
```
public static SearchQuery createOrQuery(SearchQuery leftQuery, SearchQuery rightQuery)
```


Erstellt eine kombinierte Abfrage, die alle Dokumente findet, die mindestens für eine der ursprünglichen Abfragen gefunden werden.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | leftQuery | [SearchQuery](../../com.groupdocs.search/searchquery) | Die linke Kindabfrage. |
|
|  | rightQuery | [SearchQuery](../../com.groupdocs.search/searchquery) | Die rechte Kindabfrage. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A combined OR query.

### createOrQuery(SearchQuery[] queries) {#createOrQuery-com.groupdocs.search.SearchQuery---}
```
public static SearchQuery createOrQuery(SearchQuery[] queries)
```


Erstellt eine kombinierte Abfrage, die alle Dokumente findet, die mindestens für eine der ursprünglichen Abfragen gefunden werden.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | queries | [SearchQuery\[\]](../../com.groupdocs.search/searchquery) | Die untergeordneten Abfragen. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A combined OR query.

### createWildcardQuery(int count) {#createWildcardQuery-int-}
```
public static SearchQuery createWildcardQuery(int count)
```


Erstellt ein Platzhalterzeichen für die Phrasensuche.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | count | int | Die Anzahl der Wörter im Platzhalter. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A wildcard for the phrase search.

### createWildcardQuery(int minCount, int maxCount) {#createWildcardQuery-int-int-}
```
public static SearchQuery createWildcardQuery(int minCount, int maxCount)
```


Erstellt ein Platzhalterzeichen für die Phrasensuche.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | minCount | int | Die minimale Anzahl der Wörter im Platzhalter. |
|
|  | maxCount | int | Die maximale Anzahl der Wörter im Platzhalter. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A wildcard for the phrase search.

