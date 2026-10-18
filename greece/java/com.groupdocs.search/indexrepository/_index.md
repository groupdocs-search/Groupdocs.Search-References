---
title: "IndexRepository"
second_title: "GroupDocs.Search για Java API Reference"
description: "Αντιπροσωπεύει ένα δοχείο για τη συνένωση πολλαπλών ευρετηρίων και την εκτέλεση κοινών λειτουργιών σε αυτά."
type: docs
weight: 18
url: /el/java/com.groupdocs.search/indexrepository/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.io.Closeable
```
public class IndexRepository implements Closeable
```

Αντιπροσωπεύει ένα δοχείο για τη συνένωση πολλαπλών ευρετηρίων και την εκτέλεση κοινών λειτουργιών σε αυτά.


**Learn more**

* [Search index repository](../https://docs.groupdocs.com/display/searchjava/Search+index+repository)


Το παράδειγμα δείχνει μια τυπική χρήση της κλάσης.

````
 ```

String indexFolder1 = "c:\\MyIndex\\";
String indexFolder2 = "c:\\MyIndex\\";
String query = "Einstein";
IndexRepository repository = new IndexRepository();
repository.addToRepository(indexFolder1); // Φόρτωση ενός υπάρχοντος ευρετηρίου
repository.addToRepository(indexFolder2); // Φόρτωση ενός άλλου υπάρχοντος ευρετηρίου
SearchResult result = repository.search(query); // Αναζήτηση στα ευρετήρια του αποθετηρίου
 
```
 
````


## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [IndexRepository()](#IndexRepository--) | Αρχικοποιεί μια νέα παρουσία της |
IndexRepository
κλάσης.
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getEvents()](#getEvents--) | Λαμβάνει το κέντρο γεγονότων για την εγγραφή σε γεγονότα. |
|
|  | [getIndexes()](#getIndexes--) | Λαμβάνει τα ευρετήρια που περιέχονται σε αυτό |
IndexRepository
.
|
|  | [close()](#close--) | Απελευθερώνει όλους τους πόρους που χρησιμοποιούνται από το |
IndexRepository
.
|
|  | [create()](#create--) | Δημιουργεί ένα νέο ευρετήριο στη μνήμη. |
|
|  | [create(IndexSettings settings)](#create-com.groupdocs.search.IndexSettings-) | Δημιουργεί ένα νέο ευρετήριο στη μνήμη. |
|
|  | [create(String indexFolder)](#create-java.lang.String-) | Δημιουργεί ένα νέο ευρετήριο στον δίσκο. |
|
|  | [create(String indexFolder, IndexSettings settings)](#create-java.lang.String-com.groupdocs.search.IndexSettings-) | Δημιουργεί ένα νέο ευρετήριο στον δίσκο. |
|
|  | [addToRepository(Index index)](#addToRepository-com.groupdocs.search.Index-) | Προσθέτει ένα ευρετήριο στο αποθετήριο ευρετηρίων. |
|
|  | [addToRepository(String indexFolder)](#addToRepository-java.lang.String-) | Ανοίγει και προσθέτει ένα ευρετήριο στο αποθετήριο ευρετηρίων. |
|
|  | [update()](#update--) | Ενημερώνει όλα τα ευρετήρια στο αποθετήριο. |
|
|  | [update(UpdateOptions options)](#update-com.groupdocs.search.options.UpdateOptions-) | Ενημερώνει όλα τα ευρετήρια στο αποθετήριο. |
|
|  | [search(String query)](#search-java.lang.String-) | Αναζητά σε όλα τα ευρετήρια του αποθετηρίου. |
|
|  | [search(String query, SearchOptions options)](#search-java.lang.String-com.groupdocs.search.options.SearchOptions-) | Αναζητά σε όλα τα ευρετήρια του αποθετηρίου. |
|
|  | [search(SearchQuery query)](#search-com.groupdocs.search.SearchQuery-) | Αναζητά σε όλα τα ευρετήρια του αποθετηρίου. |
|
|  | [search(SearchQuery query, SearchOptions options)](#search-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-) | Αναζητά σε όλα τα ευρετήρια του αποθετηρίου. |
|
### IndexRepository() {#IndexRepository--}
```
public IndexRepository()
```


Αρχικοποιεί μια νέα παρουσία της
IndexRepository
κλάσης.


### getEvents() {#getEvents--}
```
public final EventHub getEvents()
```


Λαμβάνει το κέντρο γεγονότων για την εγγραφή σε γεγονότα.


**Returns:**
[EventHub](../../com.groupdocs.search.events/eventhub) - The event hub for subscribing to events.

### getIndexes() {#getIndexes--}
```
public final Index[] getIndexes()
```


Λαμβάνει τα ευρετήρια που περιέχονται σε αυτό
IndexRepository
.


**Returns:**
com.groupdocs.search.Index[] - Τα ευρετήρια.

### close() {#close--}
```
public final void close()
```


Απελευθερώνει όλους τους πόρους που χρησιμοποιούνται από το
IndexRepository
.


### create() {#create--}
```
public final Index create()
```


Δημιουργεί ένα νέο ευρετήριο στη μνήμη.


**Returns:**
[Index](../../com.groupdocs.search/index) - The created index.

Το παράδειγμα δείχνει πώς να δημιουργήσετε ένα ευρετήριο στη μνήμη μέσω του αποθετηρίου ευρετηρίων.

````
 ```

IndexRepository indexRepository = new IndexRepository();
Index index = indexRepository.create();
 
```
 
````


### create(IndexSettings settings) {#create-com.groupdocs.search.IndexSettings-}
```
public final Index create(IndexSettings settings)
```


Δημιουργεί ένα νέο ευρετήριο στη μνήμη.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | Οι ρυθμίσεις του ευρετηρίου. |

Το παράδειγμα δείχνει πώς να δημιουργήσετε ένα ευρετήριο στη μνήμη μέσω του αποθετηρίου ευρετηρίων.

````
 ```

IndexRepository indexRepository = new IndexRepository();
IndexSettings settings = new IndexSettings();
settings.setUseStopWords(false); // Απενεργοποίηση χρήσης λέξεων-σταματημάτων κατά την ευρετηρίαση
Index index = indexRepository.create(settings);
 
```
 
````

|

**Returns:**
[Index](../../com.groupdocs.search/index) - The created index.

### create(String indexFolder) {#create-java.lang.String-}
```
public final Index create(String indexFolder)
```


Δημιουργεί ένα νέο ευρετήριο στον δίσκο.
Ο φάκελος του ευρετηρίου θα καθαριστεί πριν από τη δημιουργία του ευρετηρίου.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | indexFolder | java.lang.String | Ο φάκελος του ευρετηρίου. |

Το παράδειγμα δείχνει πώς να δημιουργήσετε ένα ευρετήριο στον δίσκο μέσω του αποθετηρίου ευρετηρίων.

````
 ```

String indexFolder = "c:\\MyIndex\\";
IndexRepository indexRepository = new IndexRepository();
Index index = indexRepository.create(indexFolder);
 
```
 
````

|

**Returns:**
[Index](../../com.groupdocs.search/index) - The created index.

### create(String indexFolder, IndexSettings settings) {#create-java.lang.String-com.groupdocs.search.IndexSettings-}
```
public final Index create(String indexFolder, IndexSettings settings)
```


Δημιουργεί ένα νέο ευρετήριο στον δίσκο.
Ο φάκελος του ευρετηρίου θα καθαριστεί πριν από τη δημιουργία του ευρετηρίου.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | indexFolder | java.lang.String | Ο φάκελος του ευρετηρίου. |
|
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | Οι ρυθμίσεις του ευρετηρίου. |

Το παράδειγμα δείχνει πώς να δημιουργήσετε ένα ευρετήριο στον δίσκο μέσω του αποθετηρίου ευρετηρίων.

````
 ```

String indexFolder = "c:\\MyIndex\\";
IndexRepository indexRepository = new IndexRepository();
IndexSettings settings = new IndexSettings();
settings.setUseStopWords(false); // Απενεργοποίηση χρήσης λέξεων-σταματημάτων κατά την ευρετηρίαση
Index index = indexRepository.create(indexFolder, settings);
 
```
 
````

|

**Returns:**
[Index](../../com.groupdocs.search/index) - The created index.

### addToRepository(Index index) {#addToRepository-com.groupdocs.search.Index-}
```
public final void addToRepository(Index index)
```


Προσθέτει ένα ευρετήριο στο αποθετήριο ευρετηρίων.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | index | [Index](../../com.groupdocs.search/index) | Το ευρετήριο προς προσθήκη. |

Το παράδειγμα δείχνει πώς να προσθέσετε ένα ευρετήριο στο αποθετήριο ευρετηρίων.

````
 ```

Index index = new Index();
IndexRepository indexRepository = new IndexRepository();
indexRepository.addToRepository(index);
 
```
 
````

|

### addToRepository(String indexFolder) {#addToRepository-java.lang.String-}
```
public final void addToRepository(String indexFolder)
```


Ανοίγει και προσθέτει ένα ευρετήριο στο αποθετήριο ευρετηρίων.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | indexFolder | java.lang.String | Ο φάκελος του ευρετηρίου. |

Το παράδειγμα δείχνει πώς να προσθέσετε ένα ευρετήριο στο αποθετήριο ευρετηρίων.

````
 ```

String indexFolder = "c:\\MyIndex\\";
IndexRepository indexRepository = new IndexRepository();
indexRepository.addToRepository(indexFolder);
 
```
 
````

|

### update() {#update--}
```
public final void update()
```


Ενημερώνει όλα τα ευρετήρια στο αποθετήριο.

Το παράδειγμα δείχνει πώς να ενημερώσετε τα ευρετήρια στο αποθετήριο.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // Δημιουργία ευρετηρίου
index.add(documentsFolder); // Καταχώρηση εγγράφων
// Διαγραφή εγγράφων από το φάκελο εγγράφων ή τροποποίηση τους ή προσθήκη νέων εγγράφων στο φάκελο
repository.update();
 
```
 
````



### update(UpdateOptions options) {#update-com.groupdocs.search.options.UpdateOptions-}
```
public final void update(UpdateOptions options)
```


Ενημερώνει όλα τα ευρετήρια στο αποθετήριο.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | options | [UpdateOptions](../../com.groupdocs.search.options/updateoptions) | Οι επιλογές ενημέρωσης. |

Το παράδειγμα δείχνει πώς να ενημερώσετε τα ευρετήρια στο αποθετήριο.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // Δημιουργία ευρετηρίου
index.add(documentsFolder); // Καταχώρηση εγγράφων
// Διαγραφή εγγράφων από το φάκελο εγγράφων ή τροποποίηση τους ή προσθήκη νέων εγγράφων στο φάκελο
UpdateOptions options = new UpdateOptions();
options.setThreads(2); // Ορισμός του αριθμού των νημάτων ευρετηρίου
repository.update(options);
 
```
 
````

|

### search(String query) {#search-java.lang.String-}
```
public final SearchResult search(String query)
```


Αναζητά σε όλα τα ευρετήρια του αποθετηρίου.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | query | java.lang.String | Το ερώτημα αναζήτησης. |

Το παράδειγμα δείχνει πώς να εκτελέσετε αναζήτηση στο αποθετήριο ευρετηρίων.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // Δημιουργία ευρετηρίου
index.add(documentsFolder); // Καταχώρηση εγγράφων
SearchResult result = repository.search(query); // Αναζήτηση
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(String query, SearchOptions options) {#search-java.lang.String-com.groupdocs.search.options.SearchOptions-}
```
public final SearchResult search(String query, SearchOptions options)
```


Αναζητά σε όλα τα ευρετήρια του αποθετηρίου.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | query | java.lang.String | Το ερώτημα αναζήτησης. |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | Οι επιλογές αναζήτησης. |

Το παράδειγμα δείχνει πώς να εκτελέσετε αναζήτηση στο αποθετήριο ευρετηρίων.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // Δημιουργία ευρετηρίου
index.add(documentsFolder); // Καταχώρηση εγγράφων
SearchOptions options = new SearchOptions();
options.setUseCaseSensitiveSearch(true); // Ορισμός σημαίας για αναζήτηση με διάκριση πεζών-κεφαλαίων
SearchResult result = repository.search(query, options); // Αναζήτηση
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(SearchQuery query) {#search-com.groupdocs.search.SearchQuery-}
```
public final SearchResult search(SearchQuery query)
```


Αναζητά σε όλα τα ευρετήρια του αποθετηρίου.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | Το ερώτημα αναζήτησης. |

Το παράδειγμα δείχνει πώς να εκτελέσετε αναζήτηση στο αποθετήριο ευρετηρίων.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // Δημιουργία ευρετηρίου
index.add(documentsFolder); // Καταχώρηση εγγράφων
SearchQuery query = SearchQuery.createWordQuery("Einstein"); // Δημιουργία ερωτήματος αναζήτησης σε μορφή αντικειμένου
SearchResult result = repository.search(query); // Αναζήτηση
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(SearchQuery query, SearchOptions options) {#search-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-}
```
public final SearchResult search(SearchQuery query, SearchOptions options)
```


Αναζητά σε όλα τα ευρετήρια του αποθετηρίου.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | Το ερώτημα αναζήτησης. |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | Οι επιλογές αναζήτησης. |

Το παράδειγμα δείχνει πώς να εκτελέσετε αναζήτηση στο αποθετήριο ευρετηρίων.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // Δημιουργία ευρετηρίου
index.add(documentsFolder); // Καταχώρηση εγγράφων
SearchOptions options = new SearchOptions();
options.setUseCaseSensitiveSearch(true); // Ορισμός σημαίας για αναζήτηση με διάκριση πεζών-κεφαλαίων
SearchQuery query = SearchQuery.createWordQuery("Einstein"); // Δημιουργία ερωτήματος αναζήτησης σε μορφή αντικειμένου
SearchResult result = repository.search(query, options); // Αναζήτηση
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

