---
title: "SearchQuery"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Représente une requête de recherche sous forme d'objet."
type: docs
weight: 25
url: /fr/java/com.groupdocs.search/searchquery/
---
**Inheritance:**
java.lang.Object
```
public abstract class SearchQuery
```

Représente une requête de recherche sous forme d'objet.


**Learn more**

* [Searching](../https://docs.groupdocs.com/display/searchjava/Searching)
* [Queries in text and object form](../https://docs.groupdocs.com/display/searchjava/Queries+in+text+and+object+form)
* [Nesting search queries in object form](../https://docs.groupdocs.com/display/searchjava/Nesting+search+queries+in+object+form)


L'exemple montre une utilisation typique de la classe.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
 
Index index = new Index(indexFolder); // Création de l'index dans le dossier spécifié
index.add(documentsFolder); // Indexation des documents depuis le dossier spécifié
 
// Création d'une sous-requête de recherche de plage de dates
SearchQuery subquery1 = SearchQuery.createDateRangeQuery(new Date(2011, 6, 17), new Date(2013, 1, 1));
 
// Création d'une sous-requête de joker avec un nombre de mots manquants de 0 à 2
SearchQuery subquery2 = SearchQuery.createWildcardQuery(0, 2);
 
// Création d'une sous-requête de mot simple
SearchQuery subquery3 = SearchQuery.createWordQuery(\"birth\");
subquery3.setSearchOptions(new SearchOptions()); // Définition des options de recherche uniquement pour la sous-requête 3
subquery3.getSearchOptions().getFuzzySearch().setEnabled(true);
subquery3.getSearchOptions().getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(1));
 
// Combinaison des sous-requêtes en une seule requête
SearchQuery query = SearchQuery.createPhraseSearchQuery(subquery1, subquery2, subquery3);
 
// Création d'un objet d'options de recherche avec une capacité accrue des occurrences trouvées
SearchOptions options = new SearchOptions(); // Options de recherche globales
options.setMaxOccurrenceCountPerTerm(1000000);
options.setMaxTotalOccurrenceCount(10000000);
 
SearchResult result = index.search(query, options); // Recherche
 
```
 
````


## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getFieldName()](#getFieldName--) | Obtient le nom du champ. |
|
|  | [getChildCount()](#getChildCount--) | Obtient le nombre de sous-requêtes. |
|
|  | [getFirstChild()](#getFirstChild--) | Obtient la première sous-requête. |
|
|  | [getSecondChild()](#getSecondChild--) | Obtient la deuxième sous-requête. |
|
|  | [getChild(int index)](#getChild-int-) | Obtient une sous-requête par indice. |
|
|  | [getSearchOptions()](#getSearchOptions--) | Obtient ou définit les options de recherche de cette requête seach. |
|
|  | [setSearchOptions(SearchOptions value)](#setSearchOptions-com.groupdocs.search.options.SearchOptions-) | Obtient ou définit les options de recherche de cette requête seach. |
|
|  | [toString()](#toString--) | Renvoie une  System.String  qui représente l'instance actuelle de  SearchQuery . |
|
|  | [createWordQuery(String term)](#createWordQuery-java.lang.String-) | Crée une requête de mot simple. |
|
|  | [createWordPatternQuery(WordPattern pattern)](#createWordPatternQuery-com.groupdocs.search.common.WordPattern-) | Crée une requête de motif de mot. |
|
|  | [createRegexQuery(String pattern)](#createRegexQuery-java.lang.String-) | Crée une requête d'expression régulière. |
|
|  | [createRegexQuery(String pattern, int options)](#createRegexQuery-java.lang.String-int-) | Crée une requête d'expression régulière. |
|
|  | [createNumericRangeQuery(long start, long end)](#createNumericRangeQuery-long-long-) | Crée une requête de plage numérique. |
|
|  | [createDateRangeQuery(Date start, Date end)](#createDateRangeQuery-java.util.Date-java.util.Date-) | Crée une requête de plage de dates. |
|
|  | [createPhraseSearchQuery(SearchQuery[] queries)](#createPhraseSearchQuery-com.groupdocs.search.SearchQuery...-) | Crée une requête de recherche de phrase. |
|
|  | [createAndQuery(SearchQuery[] queries)](#createAndQuery-com.groupdocs.search.SearchQuery---) | Crée une requête combinée qui ne trouvera que les documents qui seront trouvés pour chaque requête originale. |
|
|  | [createFieldQuery(String fieldName, SearchQuery query)](#createFieldQuery-java.lang.String-com.groupdocs.search.SearchQuery-) | Ajoute un champ à la requête spécifiée. |
|
|  | [createNotQuery(SearchQuery query)](#createNotQuery-com.groupdocs.search.SearchQuery-) | Crée une requête inversée qui trouvera les documents restants dans un index par rapport à ceux qui seront trouvés pour la requête originale. |
|
|  | [createAndQuery(SearchQuery leftQuery, SearchQuery rightQuery)](#createAndQuery-com.groupdocs.search.SearchQuery-com.groupdocs.search.SearchQuery-) | Crée une requête combinée qui ne trouvera que les documents qui seront trouvés pour chaque requête originale. |
|
|  | [createOrQuery(SearchQuery leftQuery, SearchQuery rightQuery)](#createOrQuery-com.groupdocs.search.SearchQuery-com.groupdocs.search.SearchQuery-) | Crée une requête combinée qui trouvera tous les documents qui seront trouvés au moins pour l'une des requêtes originales. |
|
|  | [createOrQuery(SearchQuery[] queries)](#createOrQuery-com.groupdocs.search.SearchQuery---) | Crée une requête combinée qui trouvera tous les documents qui seront trouvés au moins pour l'une des requêtes originales. |
|
|  | [createWildcardQuery(int count)](#createWildcardQuery-int-) | Crée un joker pour la recherche de phrase. |
|
|  | [createWildcardQuery(int minCount, int maxCount)](#createWildcardQuery-int-int-) | Crée un joker pour la recherche de phrase. |
|
### getFieldName() {#getFieldName--}
```
public String getFieldName()
```


Obtient le nom du champ.


**Returns:**
java.lang.String - Le nom du champ.

### getChildCount() {#getChildCount--}
```
public int getChildCount()
```


Obtient le nombre de sous-requêtes.


**Returns:**
int - Le nombre de requêtes enfants.

### getFirstChild() {#getFirstChild--}
```
public SearchQuery getFirstChild()
```


Obtient la première sous-requête.


**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - The first child query.

### getSecondChild() {#getSecondChild--}
```
public SearchQuery getSecondChild()
```


Obtient la deuxième sous-requête.


**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - The second child query.

### getChild(int index) {#getChild-int-}
```
public abstract SearchQuery getChild(int index)
```


Obtient une sous-requête par indice.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | index | int | L'index. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A child query corresponding the specified index.

### getSearchOptions() {#getSearchOptions--}
```
public final SearchOptions getSearchOptions()
```


Obtient ou définit les options de recherche de cette requête seach.


**Returns:**
[SearchOptions](../../com.groupdocs.search.options/searchoptions) - The search options.

### setSearchOptions(SearchOptions value) {#setSearchOptions-com.groupdocs.search.options.SearchOptions-}
```
public final void setSearchOptions(SearchOptions value)
```


Obtient ou définit les options de recherche de cette requête seach.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | value | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | Les options de recherche. |
|

### toString() {#toString--}
```
public abstract String toString()
```


Renvoie une  System.String  qui représente l'instance actuelle de  SearchQuery .


**Returns:**
java.lang.String - Un System.String qui représente l'instance actuelle de SearchQuery.

### createWordQuery(String term) {#createWordQuery-java.lang.String-}
```
public static SearchQuery createWordQuery(String term)
```


Crée une requête de mot simple.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | terme | java.lang.String | Le terme à rechercher. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A simple word query.

### createWordPatternQuery(WordPattern pattern) {#createWordPatternQuery-com.groupdocs.search.common.WordPattern-}
```
public static SearchQuery createWordPatternQuery(WordPattern pattern)
```


Crée une requête de motif de mot.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | pattern | [WordPattern](../../com.groupdocs.search.common/wordpattern) | Le modèle de mot. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A word pattern query.

### createRegexQuery(String pattern) {#createRegexQuery-java.lang.String-}
```
public static SearchQuery createRegexQuery(String pattern)
```


Crée une requête d'expression régulière.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | motif | java.lang.String | Le modèle d'expression régulière à faire correspondre. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A regular expression query.

### createRegexQuery(String pattern, int options) {#createRegexQuery-java.lang.String-int-}
```
public static SearchQuery createRegexQuery(String pattern, int options)
```


Crée une requête d'expression régulière.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | motif | java.lang.String | Le modèle d'expression régulière à faire correspondre. |
|
|  | options | int | Une combinaison bit à bit des valeurs d'énumération qui modifient l'expression régulière. Cette valeur doit contenir le drapeau RegexOptions.IgnoreCase. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A regular expression query.

### createNumericRangeQuery(long start, long end) {#createNumericRangeQuery-long-long-}
```
public static SearchQuery createNumericRangeQuery(long start, long end)
```


Crée une requête de plage numérique.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | début | long | La valeur de début d'une plage. |
|
|  | fin | long | La valeur de fin d'une plage. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A numeric range query.

### createDateRangeQuery(Date start, Date end) {#createDateRangeQuery-java.util.Date-java.util.Date-}
```
public static SearchQuery createDateRangeQuery(Date start, Date end)
```


Crée une requête de plage de dates.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | début | java.util.Date | La valeur de début d'une plage. |
|
|  | fin | java.util.Date | La valeur de fin d'une plage. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A date range query.

### createPhraseSearchQuery(SearchQuery[] queries) {#createPhraseSearchQuery-com.groupdocs.search.SearchQuery...-}
```
public static SearchQuery createPhraseSearchQuery(SearchQuery[] queries)
```


Crée une requête de recherche de phrase.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | queries | [SearchQuery\[\]](../../com.groupdocs.search/searchquery) | Les requêtes enfants. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A phrase search query.

### createAndQuery(SearchQuery[] queries) {#createAndQuery-com.groupdocs.search.SearchQuery---}
```
public static SearchQuery createAndQuery(SearchQuery[] queries)
```


Crée une requête combinée qui ne trouvera que les documents qui seront trouvés pour chaque requête originale.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | queries | [SearchQuery\[\]](../../com.groupdocs.search/searchquery) | Le nom du champ dans lequel rechercher. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A combined AND query.

### createFieldQuery(String fieldName, SearchQuery query) {#createFieldQuery-java.lang.String-com.groupdocs.search.SearchQuery-}
```
public static SearchQuery createFieldQuery(String fieldName, SearchQuery query)
```


Ajoute un champ à la requête spécifiée.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | fieldName | java.lang.String | Le nom du champ dans lequel rechercher. |
|
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | La requête pour ajouter le champ. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A query with the field to search in.

### createNotQuery(SearchQuery query) {#createNotQuery-com.groupdocs.search.SearchQuery-}
```
public static SearchQuery createNotQuery(SearchQuery query)
```


Crée une requête inversée qui trouvera les documents restants dans un index par rapport à ceux qui seront trouvés pour la requête originale.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | La requête à inverser. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A combined NOT query.

### createAndQuery(SearchQuery leftQuery, SearchQuery rightQuery) {#createAndQuery-com.groupdocs.search.SearchQuery-com.groupdocs.search.SearchQuery-}
```
public static SearchQuery createAndQuery(SearchQuery leftQuery, SearchQuery rightQuery)
```


Crée une requête combinée qui ne trouvera que les documents qui seront trouvés pour chaque requête originale.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | leftQuery | [SearchQuery](../../com.groupdocs.search/searchquery) | La requête enfant gauche. |
|
|  | rightQuery | [SearchQuery](../../com.groupdocs.search/searchquery) | La requête enfant droite. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A combined AND query.

### createOrQuery(SearchQuery leftQuery, SearchQuery rightQuery) {#createOrQuery-com.groupdocs.search.SearchQuery-com.groupdocs.search.SearchQuery-}
```
public static SearchQuery createOrQuery(SearchQuery leftQuery, SearchQuery rightQuery)
```


Crée une requête combinée qui trouvera tous les documents qui seront trouvés au moins pour l'une des requêtes originales.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | leftQuery | [SearchQuery](../../com.groupdocs.search/searchquery) | La requête enfant gauche. |
|
|  | rightQuery | [SearchQuery](../../com.groupdocs.search/searchquery) | La requête enfant droite. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A combined OR query.

### createOrQuery(SearchQuery[] queries) {#createOrQuery-com.groupdocs.search.SearchQuery---}
```
public static SearchQuery createOrQuery(SearchQuery[] queries)
```


Crée une requête combinée qui trouvera tous les documents qui seront trouvés au moins pour l'une des requêtes originales.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | queries | [SearchQuery\[\]](../../com.groupdocs.search/searchquery) | Les requêtes enfants. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A combined OR query.

### createWildcardQuery(int count) {#createWildcardQuery-int-}
```
public static SearchQuery createWildcardQuery(int count)
```


Crée un joker pour la recherche de phrase.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | count | int | Le nombre de mots dans le caractère générique. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A wildcard for the phrase search.

### createWildcardQuery(int minCount, int maxCount) {#createWildcardQuery-int-int-}
```
public static SearchQuery createWildcardQuery(int minCount, int maxCount)
```


Crée un joker pour la recherche de phrase.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | minCount | int | Le nombre minimum de mots dans le caractère générique. |
|
|  | maxCount | int | Le nombre maximum de mots dans le caractère générique. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A wildcard for the phrase search.

