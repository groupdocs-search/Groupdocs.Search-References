---
title: "SearchQuery"
second_title: "GroupDocs.Search για Java API Reference"
description: "Αντιπροσωπεύει ένα ερώτημα αναζήτησης σε μορφή αντικειμένου."
type: docs
weight: 25
url: /el/java/com.groupdocs.search/searchquery/
---
**Inheritance:**
java.lang.Object
```
public abstract class SearchQuery
```

Αντιπροσωπεύει ένα ερώτημα αναζήτησης σε μορφή αντικειμένου.


**Learn more**

* [Searching](../https://docs.groupdocs.com/display/searchjava/Searching)
* [Queries in text and object form](../https://docs.groupdocs.com/display/searchjava/Queries+in+text+and+object+form)
* [Nesting search queries in object form](../https://docs.groupdocs.com/display/searchjava/Nesting+search+queries+in+object+form)


Το παράδειγμα δείχνει μια τυπική χρήση της κλάσης.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
 
Index index = new Index(indexFolder); // Δημιουργία ευρετηρίου στον καθορισμένο φάκελο
index.add(documentsFolder); // Καταχώρηση εγγράφων από τον καθορισμένο φάκελο
 
// Δημιουργία υποερωτήματος αναζήτησης εύρους ημερομηνιών
SearchQuery subquery1 = SearchQuery.createDateRangeQuery(new Date(2011, 6, 17), new Date(2013, 1, 1));
 
// Δημιουργία υποερωτήματος wildcard με αριθμό λείπωντων λέξεων από 0 έως 2
SearchQuery subquery2 = SearchQuery.createWildcardQuery(0, 2);
 
// Δημιουργία υποερωτήματος απλής λέξης
SearchQuery subquery3 = SearchQuery.createWordQuery("birth");
subquery3.setSearchOptions(new SearchOptions()); // Ρύθμιση επιλογών αναζήτησης μόνο για το υποερώτημα 3
subquery3.getSearchOptions().getFuzzySearch().setEnabled(true);
subquery3.getSearchOptions().getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(1));
 
// Συνδυασμός υποερωτημάτων σε ένα ερώτημα
SearchQuery query = SearchQuery.createPhraseSearchQuery(subquery1, subquery2, subquery3);
 
// Δημιουργία αντικειμένου επιλογών αναζήτησης με αυξημένη χωρητικότητα των ευρεθέντων εμφανίσεων
SearchOptions options = new SearchOptions(); // Γενικές επιλογές αναζήτησης
options.setMaxOccurrenceCountPerTerm(1000000);
options.setMaxTotalOccurrenceCount(10000000);
 
SearchResult result = index.search(query, options); // Αναζήτηση
 
```
 
````


## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getFieldName()](#getFieldName--) | Λαμβάνει το όνομα του πεδίου. |
|
|  | [getChildCount()](#getChildCount--) | Λαμβάνει τον αριθμό των θυγατρικών ερωτημάτων. |
|
|  | [getFirstChild()](#getFirstChild--) | Λαμβάνει το πρώτο θυγατρικό ερώτημα. |
|
|  | [getSecondChild()](#getSecondChild--) | Λαμβάνει το δεύτερο θυγατρικό ερώτημα. |
|
|  | [getChild(int index)](#getChild-int-) | Λαμβάνει ένα θυγατρικό ερώτημα με βάση έναν δείκτη. |
|
|  | [getSearchOptions()](#getSearchOptions--) | Λαμβάνει ή ορίζει τις επιλογές αναζήτησης αυτού του ερωτήματος αναζήτησης. |
|
|  | [setSearchOptions(SearchOptions value)](#setSearchOptions-com.groupdocs.search.options.SearchOptions-) | Λαμβάνει ή ορίζει τις επιλογές αναζήτησης αυτού του ερωτήματος αναζήτησης. |
|
|  | [toString()](#toString--) | Επιστρέφει ένα  System.String  που αντιπροσωπεύει την τρέχουσα  SearchQuery  παρουσία. |
|
|  | [createWordQuery(String term)](#createWordQuery-java.lang.String-) | Δημιουργεί ένα ερώτημα απλής λέξης. |
|
|  | [createWordPatternQuery(WordPattern pattern)](#createWordPatternQuery-com.groupdocs.search.common.WordPattern-) | Δημιουργεί ένα ερώτημα προτύπου λέξης. |
|
|  | [createRegexQuery(String pattern)](#createRegexQuery-java.lang.String-) | Δημιουργεί ένα ερώτημα κανονικής έκφρασης. |
|
|  | [createRegexQuery(String pattern, int options)](#createRegexQuery-java.lang.String-int-) | Δημιουργεί ένα ερώτημα κανονικής έκφρασης. |
|
|  | [createNumericRangeQuery(long start, long end)](#createNumericRangeQuery-long-long-) | Δημιουργεί ένα ερώτημα αριθμητικής περιοχής. |
|
|  | [createDateRangeQuery(Date start, Date end)](#createDateRangeQuery-java.util.Date-java.util.Date-) | Δημιουργεί ένα ερώτημα περιοχής ημερομηνίας. |
|
|  | [createPhraseSearchQuery(SearchQuery[] queries)](#createPhraseSearchQuery-com.groupdocs.search.SearchQuery...-) | Δημιουργεί ένα ερώτημα αναζήτησης φράσης. |
|
|  | [createAndQuery(SearchQuery[] queries)](#createAndQuery-com.groupdocs.search.SearchQuery---) | Δημιουργεί ένα συνδυασμένο ερώτημα που θα βρει μόνο έγγραφα που θα βρεθούν για κάθε αρχικό ερώτημα. |
|
|  | [createFieldQuery(String fieldName, SearchQuery query)](#createFieldQuery-java.lang.String-com.groupdocs.search.SearchQuery-) | Προσθέτει ένα πεδίο στο καθορισμένο ερώτημα. |
|
|  | [createNotQuery(SearchQuery query)](#createNotQuery-com.groupdocs.search.SearchQuery-) | Δημιουργεί ένα ανεστραμμένο ερώτημα που θα βρει τα υπόλοιπα έγγραφα σε ένα ευρετήριο έναντι αυτών που θα βρεθούν για το αρχικό ερώτημα. |
|
|  | [createAndQuery(SearchQuery leftQuery, SearchQuery rightQuery)](#createAndQuery-com.groupdocs.search.SearchQuery-com.groupdocs.search.SearchQuery-) | Δημιουργεί ένα συνδυασμένο ερώτημα που θα βρει μόνο έγγραφα που θα βρεθούν για κάθε αρχικό ερώτημα. |
|
|  | [createOrQuery(SearchQuery leftQuery, SearchQuery rightQuery)](#createOrQuery-com.groupdocs.search.SearchQuery-com.groupdocs.search.SearchQuery-) | Δημιουργεί ένα συνδυασμένο ερώτημα που θα βρει όλα τα έγγραφα που θα βρεθούν τουλάχιστον για ένα από τα αρχικά ερωτήματα. |
|
|  | [createOrQuery(SearchQuery[] queries)](#createOrQuery-com.groupdocs.search.SearchQuery---) | Δημιουργεί ένα συνδυασμένο ερώτημα που θα βρει όλα τα έγγραφα που θα βρεθούν τουλάχιστον για ένα από τα αρχικά ερωτήματα. |
|
|  | [createWildcardQuery(int count)](#createWildcardQuery-int-) | Δημιουργεί ένα μπαλαντέρ για την αναζήτηση φράσης. |
|
|  | [createWildcardQuery(int minCount, int maxCount)](#createWildcardQuery-int-int-) | Δημιουργεί ένα μπαλαντέρ για την αναζήτηση φράσης. |
|
### getFieldName() {#getFieldName--}
```
public String getFieldName()
```


Λαμβάνει το όνομα του πεδίου.


**Returns:**
java.lang.String - Το όνομα του πεδίου.

### getChildCount() {#getChildCount--}
```
public int getChildCount()
```


Λαμβάνει τον αριθμό των θυγατρικών ερωτημάτων.


**Returns:**
int - Ο αριθμός των θυγατρικών ερωτημάτων.

### getFirstChild() {#getFirstChild--}
```
public SearchQuery getFirstChild()
```


Λαμβάνει το πρώτο θυγατρικό ερώτημα.


**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - The first child query.

### getSecondChild() {#getSecondChild--}
```
public SearchQuery getSecondChild()
```


Λαμβάνει το δεύτερο θυγατρικό ερώτημα.


**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - The second child query.

### getChild(int index) {#getChild-int-}
```
public abstract SearchQuery getChild(int index)
```


Λαμβάνει ένα θυγατρικό ερώτημα με βάση έναν δείκτη.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | ευρετήριο | int | Το ευρετήριο. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A child query corresponding the specified index.

### getSearchOptions() {#getSearchOptions--}
```
public final SearchOptions getSearchOptions()
```


Λαμβάνει ή ορίζει τις επιλογές αναζήτησης αυτού του ερωτήματος αναζήτησης.


**Returns:**
[SearchOptions](../../com.groupdocs.search.options/searchoptions) - The search options.

### setSearchOptions(SearchOptions value) {#setSearchOptions-com.groupdocs.search.options.SearchOptions-}
```
public final void setSearchOptions(SearchOptions value)
```


Λαμβάνει ή ορίζει τις επιλογές αναζήτησης αυτού του ερωτήματος αναζήτησης.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | value | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | Οι επιλογές αναζήτησης. |
|

### toString() {#toString--}
```
public abstract String toString()
```


Επιστρέφει ένα  System.String  που αντιπροσωπεύει την τρέχουσα  SearchQuery  παρουσία.


**Returns:**
java.lang.String - Ένα System.String που αντιπροσωπεύει την τρέχουσα παρουσία του SearchQuery.

### createWordQuery(String term) {#createWordQuery-java.lang.String-}
```
public static SearchQuery createWordQuery(String term)
```


Δημιουργεί ένα ερώτημα απλής λέξης.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | όρος | java.lang.String | Ο όρος προς αναζήτηση. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A simple word query.

### createWordPatternQuery(WordPattern pattern) {#createWordPatternQuery-com.groupdocs.search.common.WordPattern-}
```
public static SearchQuery createWordPatternQuery(WordPattern pattern)
```


Δημιουργεί ένα ερώτημα προτύπου λέξης.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | pattern | [WordPattern](../../com.groupdocs.search.common/wordpattern) | Το μοτίβο λέξης. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A word pattern query.

### createRegexQuery(String pattern) {#createRegexQuery-java.lang.String-}
```
public static SearchQuery createRegexQuery(String pattern)
```


Δημιουργεί ένα ερώτημα κανονικής έκφρασης.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | pattern | java.lang.String | Το μοτίβο κανονικής έκφρασης για αντιστοίχιση. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A regular expression query.

### createRegexQuery(String pattern, int options) {#createRegexQuery-java.lang.String-int-}
```
public static SearchQuery createRegexQuery(String pattern, int options)
```


Δημιουργεί ένα ερώτημα κανονικής έκφρασης.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | pattern | java.lang.String | Το μοτίβο κανονικής έκφρασης για αντιστοίχιση. |
|
|  | options | int | Μια δυαδική συνδυαστική τιμή των τιμών της απαρίθμησης που τροποποιούν την κανονική έκφραση. Αυτή η τιμή πρέπει να περιέχει τη σημαία  RegexOptions.IgnoreCase . |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A regular expression query.

### createNumericRangeQuery(long start, long end) {#createNumericRangeQuery-long-long-}
```
public static SearchQuery createNumericRangeQuery(long start, long end)
```


Δημιουργεί ένα ερώτημα αριθμητικής περιοχής.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | αρχή | long | Η αρχική τιμή μιας περιοχής. |
|
|  | τέλος | long | Η τελική τιμή μιας περιοχής. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A numeric range query.

### createDateRangeQuery(Date start, Date end) {#createDateRangeQuery-java.util.Date-java.util.Date-}
```
public static SearchQuery createDateRangeQuery(Date start, Date end)
```


Δημιουργεί ένα ερώτημα περιοχής ημερομηνίας.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | αρχή | java.util.Date | Η αρχική τιμή μιας περιοχής. |
|
|  | τέλος | java.util.Date | Η τελική τιμή μιας περιοχής. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A date range query.

### createPhraseSearchQuery(SearchQuery[] queries) {#createPhraseSearchQuery-com.groupdocs.search.SearchQuery...-}
```
public static SearchQuery createPhraseSearchQuery(SearchQuery[] queries)
```


Δημιουργεί ένα ερώτημα αναζήτησης φράσης.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | queries | [SearchQuery\[\]](../../com.groupdocs.search/searchquery) | Τα θυγατρικά ερωτήματα. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A phrase search query.

### createAndQuery(SearchQuery[] queries) {#createAndQuery-com.groupdocs.search.SearchQuery---}
```
public static SearchQuery createAndQuery(SearchQuery[] queries)
```


Δημιουργεί ένα συνδυασμένο ερώτημα που θα βρει μόνο έγγραφα που θα βρεθούν για κάθε αρχικό ερώτημα.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | queries | [SearchQuery\[\]](../../com.groupdocs.search/searchquery) | Το όνομα του πεδίου για αναζήτηση. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A combined AND query.

### createFieldQuery(String fieldName, SearchQuery query) {#createFieldQuery-java.lang.String-com.groupdocs.search.SearchQuery-}
```
public static SearchQuery createFieldQuery(String fieldName, SearchQuery query)
```


Προσθέτει ένα πεδίο στο καθορισμένο ερώτημα.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | fieldName | java.lang.String | Το όνομα του πεδίου για αναζήτηση. |
|
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | Το ερώτημα για προσθήκη του πεδίου. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A query with the field to search in.

### createNotQuery(SearchQuery query) {#createNotQuery-com.groupdocs.search.SearchQuery-}
```
public static SearchQuery createNotQuery(SearchQuery query)
```


Δημιουργεί ένα ανεστραμμένο ερώτημα που θα βρει τα υπόλοιπα έγγραφα σε ένα ευρετήριο έναντι αυτών που θα βρεθούν για το αρχικό ερώτημα.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | Το ερώτημα για αντιστροφή. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A combined NOT query.

### createAndQuery(SearchQuery leftQuery, SearchQuery rightQuery) {#createAndQuery-com.groupdocs.search.SearchQuery-com.groupdocs.search.SearchQuery-}
```
public static SearchQuery createAndQuery(SearchQuery leftQuery, SearchQuery rightQuery)
```


Δημιουργεί ένα συνδυασμένο ερώτημα που θα βρει μόνο έγγραφα που θα βρεθούν για κάθε αρχικό ερώτημα.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | leftQuery | [SearchQuery](../../com.groupdocs.search/searchquery) | Το ερώτημα του αριστερού παιδιού. |
|
|  | rightQuery | [SearchQuery](../../com.groupdocs.search/searchquery) | Το ερώτημα του δεξιού παιδιού. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A combined AND query.

### createOrQuery(SearchQuery leftQuery, SearchQuery rightQuery) {#createOrQuery-com.groupdocs.search.SearchQuery-com.groupdocs.search.SearchQuery-}
```
public static SearchQuery createOrQuery(SearchQuery leftQuery, SearchQuery rightQuery)
```


Δημιουργεί ένα συνδυασμένο ερώτημα που θα βρει όλα τα έγγραφα που θα βρεθούν τουλάχιστον για ένα από τα αρχικά ερωτήματα.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | leftQuery | [SearchQuery](../../com.groupdocs.search/searchquery) | Το ερώτημα του αριστερού παιδιού. |
|
|  | rightQuery | [SearchQuery](../../com.groupdocs.search/searchquery) | Το ερώτημα του δεξιού παιδιού. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A combined OR query.

### createOrQuery(SearchQuery[] queries) {#createOrQuery-com.groupdocs.search.SearchQuery---}
```
public static SearchQuery createOrQuery(SearchQuery[] queries)
```


Δημιουργεί ένα συνδυασμένο ερώτημα που θα βρει όλα τα έγγραφα που θα βρεθούν τουλάχιστον για ένα από τα αρχικά ερωτήματα.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | queries | [SearchQuery\[\]](../../com.groupdocs.search/searchquery) | Τα θυγατρικά ερωτήματα. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A combined OR query.

### createWildcardQuery(int count) {#createWildcardQuery-int-}
```
public static SearchQuery createWildcardQuery(int count)
```


Δημιουργεί ένα μπαλαντέρ για την αναζήτηση φράσης.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | count | int | Ο αριθμός των λέξεων στο μπαλαντέρ. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A wildcard for the phrase search.

### createWildcardQuery(int minCount, int maxCount) {#createWildcardQuery-int-int-}
```
public static SearchQuery createWildcardQuery(int minCount, int maxCount)
```


Δημιουργεί ένα μπαλαντέρ για την αναζήτηση φράσης.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | minCount | int | Ο ελάχιστος αριθμός λέξεων στο μπαλαντέρ. |
|
|  | maxCount | int | Ο μέγιστος αριθμός λέξεων στο μπαλαντέρ. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A wildcard for the phrase search.

