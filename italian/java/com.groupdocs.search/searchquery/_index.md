---
title: "SearchQuery"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Rappresenta una query di ricerca in forma di oggetto."
type: docs
weight: 25
url: /it/java/com.groupdocs.search/searchquery/
---
**Inheritance:**
java.lang.Object
```
public abstract class SearchQuery
```

Rappresenta una query di ricerca in forma di oggetto.


**Learn more**

* [Searching](../https://docs.groupdocs.com/display/searchjava/Searching)
* [Queries in text and object form](../https://docs.groupdocs.com/display/searchjava/Queries+in+text+and+object+form)
* [Nesting search queries in object form](../https://docs.groupdocs.com/display/searchjava/Nesting+search+queries+in+object+form)


L'esempio dimostra un utilizzo tipico della classe.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
 
Index index = new Index(indexFolder); // Creazione dell'indice nella cartella specificata
index.add(documentsFolder); // Indicizzazione dei documenti dalla cartella specificata
 
// Creazione di una sottoquery di ricerca per intervallo di date
SearchQuery subquery1 = SearchQuery.createDateRangeQuery(new Date(2011, 6, 17), new Date(2013, 1, 1));
 
// Creazione di una sottoquery wildcard con numero di parole mancanti da 0 a 2
SearchQuery subquery2 = SearchQuery.createWildcardQuery(0, 2);
 
// Creazione di una sottoquery di parola semplice
SearchQuery subquery3 = SearchQuery.createWordQuery("birth");
subquery3.setSearchOptions(new SearchOptions()); // Impostazione delle opzioni di ricerca solo per la sottoquery 3
subquery3.getSearchOptions().getFuzzySearch().setEnabled(true);
subquery3.getSearchOptions().getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(1));
 
// Combinazione delle sottoquery in un'unica query
SearchQuery query = SearchQuery.createPhraseSearchQuery(subquery1, subquery2, subquery3);
 
// Creazione dell'oggetto opzioni di ricerca con capacità aumentata delle occorrenze trovate
SearchOptions options = new SearchOptions(); // Opzioni di ricerca complessive
options.setMaxOccurrenceCountPerTerm(1000000);
options.setMaxTotalOccurrenceCount(10000000);
 
SearchResult result = index.search(query, options); // Ricerca
 
```
 
````


## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getFieldName()](#getFieldName--) | Restituisce il nome del campo. |
|
|  | [getChildCount()](#getChildCount--) | Restituisce il numero di query figlie. |
|
|  | [getFirstChild()](#getFirstChild--) | Restituisce la prima query figlia. |
|
|  | [getSecondChild()](#getSecondChild--) | Restituisce la seconda query figlia. |
|
|  | [getChild(int index)](#getChild-int-) | Restituisce una query figlia mediante indice. |
|
|  | [getSearchOptions()](#getSearchOptions--) | Ottiene o imposta le opzioni di ricerca di questa query di ricerca. |
|
|  | [setSearchOptions(SearchOptions value)](#setSearchOptions-com.groupdocs.search.options.SearchOptions-) | Ottiene o imposta le opzioni di ricerca di questa query di ricerca. |
|
|  | [toString()](#toString--) | Restituisce una  System.String  che rappresenta l'istanza corrente di  SearchQuery . |
|
|  | [createWordQuery(String term)](#createWordQuery-java.lang.String-) | Crea una query di parola semplice. |
|
|  | [createWordPatternQuery(WordPattern pattern)](#createWordPatternQuery-com.groupdocs.search.common.WordPattern-) | Crea una query di modello di parola. |
|
|  | [createRegexQuery(String pattern)](#createRegexQuery-java.lang.String-) | Crea una query di espressione regolare. |
|
|  | [createRegexQuery(String pattern, int options)](#createRegexQuery-java.lang.String-int-) | Crea una query di espressione regolare. |
|
|  | [createNumericRangeQuery(long start, long end)](#createNumericRangeQuery-long-long-) | Crea una query di intervallo numerico. |
|
|  | [createDateRangeQuery(Date start, Date end)](#createDateRangeQuery-java.util.Date-java.util.Date-) | Crea una query di intervallo di date. |
|
|  | [createPhraseSearchQuery(SearchQuery[] queries)](#createPhraseSearchQuery-com.groupdocs.search.SearchQuery...-) | Crea una query di ricerca per frase. |
|
|  | [createAndQuery(SearchQuery[] queries)](#createAndQuery-com.groupdocs.search.SearchQuery---) | Crea una query combinata che troverà solo i documenti che verranno trovati per ciascuna query originale. |
|
|  | [createFieldQuery(String fieldName, SearchQuery query)](#createFieldQuery-java.lang.String-com.groupdocs.search.SearchQuery-) | Aggiunge un campo alla query specificata. |
|
|  | [createNotQuery(SearchQuery query)](#createNotQuery-com.groupdocs.search.SearchQuery-) | Crea una query invertita che troverà i documenti rimanenti in un indice rispetto a quelli che verranno trovati per la query originale. |
|
|  | [createAndQuery(SearchQuery leftQuery, SearchQuery rightQuery)](#createAndQuery-com.groupdocs.search.SearchQuery-com.groupdocs.search.SearchQuery-) | Crea una query combinata che troverà solo i documenti che verranno trovati per ciascuna query originale. |
|
|  | [createOrQuery(SearchQuery leftQuery, SearchQuery rightQuery)](#createOrQuery-com.groupdocs.search.SearchQuery-com.groupdocs.search.SearchQuery-) | Crea una query combinata che troverà tutti i documenti che verranno trovati almeno per una delle query originali. |
|
|  | [createOrQuery(SearchQuery[] queries)](#createOrQuery-com.groupdocs.search.SearchQuery---) | Crea una query combinata che troverà tutti i documenti che verranno trovati almeno per una delle query originali. |
|
|  | [createWildcardQuery(int count)](#createWildcardQuery-int-) | Crea un carattere jolly per la ricerca per frase. |
|
|  | [createWildcardQuery(int minCount, int maxCount)](#createWildcardQuery-int-int-) | Crea un carattere jolly per la ricerca per frase. |
|
### getFieldName() {#getFieldName--}
```
public String getFieldName()
```


Restituisce il nome del campo.


**Returns:**
java.lang.String - Il nome del campo.

### getChildCount() {#getChildCount--}
```
public int getChildCount()
```


Restituisce il numero di query figlie.


**Returns:**
int - Il numero di query figlie.

### getFirstChild() {#getFirstChild--}
```
public SearchQuery getFirstChild()
```


Restituisce la prima query figlia.


**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - The first child query.

### getSecondChild() {#getSecondChild--}
```
public SearchQuery getSecondChild()
```


Restituisce la seconda query figlia.


**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - The second child query.

### getChild(int index) {#getChild-int-}
```
public abstract SearchQuery getChild(int index)
```


Restituisce una query figlia mediante indice.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | indice | int | L'indice. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A child query corresponding the specified index.

### getSearchOptions() {#getSearchOptions--}
```
public final SearchOptions getSearchOptions()
```


Ottiene o imposta le opzioni di ricerca di questa query di ricerca.


**Returns:**
[SearchOptions](../../com.groupdocs.search.options/searchoptions) - The search options.

### setSearchOptions(SearchOptions value) {#setSearchOptions-com.groupdocs.search.options.SearchOptions-}
```
public final void setSearchOptions(SearchOptions value)
```


Ottiene o imposta le opzioni di ricerca di questa query di ricerca.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | value | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | Le opzioni di ricerca. |
|

### toString() {#toString--}
```
public abstract String toString()
```


Restituisce una  System.String  che rappresenta l'istanza corrente di  SearchQuery .


**Returns:**
java.lang.String - Una System.String che rappresenta l'istanza corrente di SearchQuery.

### createWordQuery(String term) {#createWordQuery-java.lang.String-}
```
public static SearchQuery createWordQuery(String term)
```


Crea una query di parola semplice.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | termine | java.lang.String | Il termine da cercare. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A simple word query.

### createWordPatternQuery(WordPattern pattern) {#createWordPatternQuery-com.groupdocs.search.common.WordPattern-}
```
public static SearchQuery createWordPatternQuery(WordPattern pattern)
```


Crea una query di modello di parola.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | pattern | [WordPattern](../../com.groupdocs.search.common/wordpattern) | Il modello di parola. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A word pattern query.

### createRegexQuery(String pattern) {#createRegexQuery-java.lang.String-}
```
public static SearchQuery createRegexQuery(String pattern)
```


Crea una query di espressione regolare.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | pattern | java.lang.String | Il modello di espressione regolare da corrispondere. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A regular expression query.

### createRegexQuery(String pattern, int options) {#createRegexQuery-java.lang.String-int-}
```
public static SearchQuery createRegexQuery(String pattern, int options)
```


Crea una query di espressione regolare.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | pattern | java.lang.String | Il modello di espressione regolare da corrispondere. |
|
|  | options | int | Una combinazione bitwise dei valori di enumerazione che modificano l'espressione regolare. Questo valore deve contenere il flag RegexOptions.IgnoreCase. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A regular expression query.

### createNumericRangeQuery(long start, long end) {#createNumericRangeQuery-long-long-}
```
public static SearchQuery createNumericRangeQuery(long start, long end)
```


Crea una query di intervallo numerico.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | inizio | long | Il valore di inizio di un intervallo. |
|
|  | fine | long | Il valore di fine di un intervallo. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A numeric range query.

### createDateRangeQuery(Date start, Date end) {#createDateRangeQuery-java.util.Date-java.util.Date-}
```
public static SearchQuery createDateRangeQuery(Date start, Date end)
```


Crea una query di intervallo di date.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | inizio | java.util.Date | Il valore di inizio di un intervallo. |
|
|  | fine | java.util.Date | Il valore di fine di un intervallo. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A date range query.

### createPhraseSearchQuery(SearchQuery[] queries) {#createPhraseSearchQuery-com.groupdocs.search.SearchQuery...-}
```
public static SearchQuery createPhraseSearchQuery(SearchQuery[] queries)
```


Crea una query di ricerca per frase.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | queries | [SearchQuery\[\]](../../com.groupdocs.search/searchquery) | Le query figlie. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A phrase search query.

### createAndQuery(SearchQuery[] queries) {#createAndQuery-com.groupdocs.search.SearchQuery---}
```
public static SearchQuery createAndQuery(SearchQuery[] queries)
```


Crea una query combinata che troverà solo i documenti che verranno trovati per ciascuna query originale.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | queries | [SearchQuery\[\]](../../com.groupdocs.search/searchquery) | Il nome del campo in cui cercare. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A combined AND query.

### createFieldQuery(String fieldName, SearchQuery query) {#createFieldQuery-java.lang.String-com.groupdocs.search.SearchQuery-}
```
public static SearchQuery createFieldQuery(String fieldName, SearchQuery query)
```


Aggiunge un campo alla query specificata.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | fieldName | java.lang.String | Il nome del campo in cui cercare. |
|
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | La query per aggiungere il campo. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A query with the field to search in.

### createNotQuery(SearchQuery query) {#createNotQuery-com.groupdocs.search.SearchQuery-}
```
public static SearchQuery createNotQuery(SearchQuery query)
```


Crea una query invertita che troverà i documenti rimanenti in un indice rispetto a quelli che verranno trovati per la query originale.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | La query da invertire. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A combined NOT query.

### createAndQuery(SearchQuery leftQuery, SearchQuery rightQuery) {#createAndQuery-com.groupdocs.search.SearchQuery-com.groupdocs.search.SearchQuery-}
```
public static SearchQuery createAndQuery(SearchQuery leftQuery, SearchQuery rightQuery)
```


Crea una query combinata che troverà solo i documenti che verranno trovati per ciascuna query originale.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | leftQuery | [SearchQuery](../../com.groupdocs.search/searchquery) | La query del figlio sinistro. |
|
|  | rightQuery | [SearchQuery](../../com.groupdocs.search/searchquery) | La query del figlio destro. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A combined AND query.

### createOrQuery(SearchQuery leftQuery, SearchQuery rightQuery) {#createOrQuery-com.groupdocs.search.SearchQuery-com.groupdocs.search.SearchQuery-}
```
public static SearchQuery createOrQuery(SearchQuery leftQuery, SearchQuery rightQuery)
```


Crea una query combinata che troverà tutti i documenti che verranno trovati almeno per una delle query originali.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | leftQuery | [SearchQuery](../../com.groupdocs.search/searchquery) | La query del figlio sinistro. |
|
|  | rightQuery | [SearchQuery](../../com.groupdocs.search/searchquery) | La query del figlio destro. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A combined OR query.

### createOrQuery(SearchQuery[] queries) {#createOrQuery-com.groupdocs.search.SearchQuery---}
```
public static SearchQuery createOrQuery(SearchQuery[] queries)
```


Crea una query combinata che troverà tutti i documenti che verranno trovati almeno per una delle query originali.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | queries | [SearchQuery\[\]](../../com.groupdocs.search/searchquery) | Le query figlie. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A combined OR query.

### createWildcardQuery(int count) {#createWildcardQuery-int-}
```
public static SearchQuery createWildcardQuery(int count)
```


Crea un carattere jolly per la ricerca per frase.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | count | int | Il numero di parole nel wildcard. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A wildcard for the phrase search.

### createWildcardQuery(int minCount, int maxCount) {#createWildcardQuery-int-int-}
```
public static SearchQuery createWildcardQuery(int minCount, int maxCount)
```


Crea un carattere jolly per la ricerca per frase.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | minCount | int | Il numero minimo di parole nel wildcard. |
|
|  | maxCount | int | Il numero massimo di parole nel wildcard. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A wildcard for the phrase search.

