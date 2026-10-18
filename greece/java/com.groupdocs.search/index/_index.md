---
title: "Index"
second_title: "GroupDocs.Search για Java API Reference"
description: "Αντιπροσωπεύει τη κύρια κλάση για την ευρετηρίαση εγγράφων και την αναζήτηση σε αυτά."
type: docs
weight: 17
url: /el/java/com.groupdocs.search/index/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.io.Closeable
```
public class Index implements Closeable
```

Αντιπροσωπεύει τη κύρια κλάση για την ευρετηρίαση εγγράφων και την αναζήτηση σε αυτά.


**Learn more**

* [Creating an index](../https://docs.groupdocs.com/display/searchjava/Creating+an+index)
* [Indexing](../https://docs.groupdocs.com/display/searchjava/Indexing)
* [Searching](../https://docs.groupdocs.com/display/searchjava/Searching)


Το παράδειγμα δείχνει μια τυπική χρήση της κλάσης.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // Δημιουργία ευρετηρίου στον καθορισμένο φάκελο
index.add(documentsFolder); // Καταχώρηση εγγράφων από τον καθορισμένο φάκελο
SearchResult result = index.search(query); // Αναζήτηση στο ευρετήριο
 
```
 
````


## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [Index()](#Index--) | Αρχικοποιεί μια νέα παρουσία της  Index  κλάσης στη μνήμη. |
|
|  | [Index(IndexSettings settings)](#Index-com.groupdocs.search.IndexSettings-) | Αρχικοποιεί μια νέα παρουσία της  Index  κλάσης στη μνήμη με συγκεκριμένες ρυθμίσεις ευρετηρίου. |
|
|  | [Index(String indexFolder)](#Index-java.lang.String-) | Αρχικοποιεί μια νέα παρουσία της  Index  κλάσης. |
|
|  | [Index(String indexFolder, IndexSettings settings)](#Index-java.lang.String-com.groupdocs.search.IndexSettings-) | Αρχικοποιεί μια νέα παρουσία της |
Index
κλάσης.
|
|  | [Index(String indexFolder, boolean overwriteIfExists)](#Index-java.lang.String-boolean-) | Αρχικοποιεί μια νέα παρουσία της |
Index
κλάσης.
|
|  | [Index(String indexFolder, IndexSettings settings, boolean overwriteIfExists)](#Index-java.lang.String-com.groupdocs.search.IndexSettings-boolean-) | Αρχικοποιεί μια νέα παρουσία της |
Index
κλάσης.
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getEvents()](#getEvents--) | Λαμβάνει το κέντρο γεγονότων για την εγγραφή σε γεγονότα. |
|
|  | [getIndexInfo()](#getIndexInfo--) | Αποκτά τις βασικές πληροφορίες για το ευρετήριο. |
|
|  | [getRepository()](#getRepository--) | Αποκτά το αντικείμενο αποθετηρίου του ευρετηρίου εάν το ευρετήριο περιέχεται σε αυτό. |
|
|  | [getIndexSettings()](#getIndexSettings--) | Αποκτά τις ρυθμίσεις του ευρετηρίου. |
|
|  | [getDictionaries()](#getDictionaries--) | Αποκτά το αποθετήριο λεξικού. |
|
|  | [close()](#close--) | Απελευθερώνει όλους τους πόρους που χρησιμοποιούνται από το |
Index
.
|
|  | [add(String path)](#add-java.lang.String-) | Εκτελεί λειτουργία ευρετηρίου. |
|
|  | [add(String path, IndexingOptions options)](#add-java.lang.String-com.groupdocs.search.options.IndexingOptions-) | Εκτελεί λειτουργία ευρετηρίου. |
|
|  | [add(String[] paths)](#add-java.lang.String---) | Εκτελεί λειτουργία ευρετηρίου. |
|
|  | [add(String[] paths, IndexingOptions options)](#add-java.lang.String---com.groupdocs.search.options.IndexingOptions-) | Εκτελεί λειτουργία ευρετηρίου. |
|
|  | [add(Document[] documents, IndexingOptions options)](#add-com.groupdocs.search.Document---com.groupdocs.search.options.IndexingOptions-) | Εκτελεί λειτουργία ευρετηρίου. |
|
|  | [add(ExtractedData[] data, IndexingOptions options)](#add-com.groupdocs.search.ExtractedData---com.groupdocs.search.options.IndexingOptions-) | Εκτελεί λειτουργία ευρετηρίου. |
|
|  | [update()](#update--) | Επαναευρετηρίζει έγγραφα που έχουν αλλάξει ή διαγραφεί από την τελευταία ενημέρωση. |
|
|  | [update(UpdateOptions options)](#update-com.groupdocs.search.options.UpdateOptions-) | Επαναευρετηρίζει έγγραφα που έχουν αλλάξει ή διαγραφεί από την τελευταία ενημέρωση. |
|
|  | [getIndexingReports()](#getIndexingReports--) | Λαμβάνει τις αναφορές για τις λειτουργίες ευρετηρίασης. |
|
|  | [getSearchReports()](#getSearchReports--) | Λαμβάνει τις αναφορές για τις λειτουργίες αναζήτησης. |
|
|  | [search(String query)](#search-java.lang.String-) | Αναζητά στο ευρετήριο. |
|
|  | [search(String query, SearchOptions options)](#search-java.lang.String-com.groupdocs.search.options.SearchOptions-) | Αναζητά στο ευρετήριο. |
|
|  | [search(SearchQuery query)](#search-com.groupdocs.search.SearchQuery-) | Αναζητά στο ευρετήριο. |
|
|  | [search(SearchQuery query, SearchOptions options)](#search-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-) | Αναζητά στο ευρετήριο. |
|
|  | [search(SearchImage image, ImageSearchOptions options)](#search-com.groupdocs.search.common.SearchImage-com.groupdocs.search.options.ImageSearchOptions-) | Εκτελεί αντίστροφη αναζήτηση εικόνας στο ευρετήριο. |
|
|  | [searchNext(ChunkSearchToken chunkSearchToken)](#searchNext-com.groupdocs.search.common.ChunkSearchToken-) | Συνεχίζει την αναζήτηση τμημάτων που ξεκίνησε με τη μέθοδο Search. |
|
|  | [searchNext(ChunkSearchToken chunkSearchToken, Cancellation cancellation)](#searchNext-com.groupdocs.search.common.ChunkSearchToken-com.groupdocs.search.common.Cancellation-) | Συνεχίζει την αναζήτηση τμημάτων που ξεκίνησε με τη μέθοδο Search. |
|
|  | [optimize()](#optimize--) | Μειώνει τον αριθμό των τμημάτων του ευρετηρίου συγχωνεύοντάς τα μεταξύ τους. |
|
|  | [optimize(MergeOptions options)](#optimize-com.groupdocs.search.options.MergeOptions-) | Μειώνει τον αριθμό των τμημάτων του ευρετηρίου συγχωνεύοντάς τα μεταξύ τους. |
|
|  | [merge(Index index, MergeOptions options)](#merge-com.groupdocs.search.Index-com.groupdocs.search.options.MergeOptions-) | Συγχωνεύει το καθορισμένο ευρετήριο με το τρέχον ευρετήριο. |
|
|  | [merge(IndexRepository repository, MergeOptions options)](#merge-com.groupdocs.search.IndexRepository-com.groupdocs.search.options.MergeOptions-) | Συγχωνεύει ευρετήρια από το καθορισμένο αποθετήριο ευρετηρίων στο τρέχον ευρετήριο. |
|
|  | [highlight(FoundDocument document, Highlighter highlighter)](#highlight-com.groupdocs.search.results.FoundDocument-com.groupdocs.search.highlighters.Highlighter-) | Δημιουργεί κείμενο μορφοποιημένο σε HTML με επισημασμένους εντοπισμένους όρους. |
|
|  | [highlight(FoundDocument document, Highlighter highlighter, HighlightOptions options)](#highlight-com.groupdocs.search.results.FoundDocument-com.groupdocs.search.highlighters.Highlighter-com.groupdocs.search.options.HighlightOptions-) | Δημιουργεί κείμενο μορφοποιημένο σε HTML με επισημασμένους εντοπισμένους όρους. |
|
|  | [getIndexedDocuments()](#getIndexedDocuments--) | Λαμβάνει έναν πίνακα με όλα τα ευρετηριασμένα έγγραφα. |
|
|  | [getIndexedDocumentItems(DocumentInfo documentInfo)](#getIndexedDocumentItems-com.groupdocs.search.results.DocumentInfo-) | Λαμβάνει έναν πίνακα με στοιχεία εγγράφου. |
|
|  | [GetIndexedDocument(String documentKey)](#GetIndexedDocument-java.lang.String-) | Λαμβάνει ένα ευρετηριασμένο έγγραφο με βάση το κλειδί του εγγράφου. |
|
|  | [getDocumentText(DocumentInfo documentInfo, OutputAdapter adapter)](#getDocumentText-com.groupdocs.search.results.DocumentInfo-com.groupdocs.search.common.OutputAdapter-) | Δημιουργεί το κείμενο ενός ευρετηριασμένου εγγράφου και το περνά μέσω ενός προσαρμογέα εξόδου. |
|
|  | [getDocumentText(DocumentInfo documentInfo, OutputAdapter adapter, TextOptions options)](#getDocumentText-com.groupdocs.search.results.DocumentInfo-com.groupdocs.search.common.OutputAdapter-com.groupdocs.search.options.TextOptions-) | Δημιουργεί κείμενο μορφοποιημένο σε HTML για το ευρετηριασμένο έγγραφο και το μεταφέρει μέσω του προσαρμογέα εξόδου. |
|
|  | [getIndexedPaths()](#getIndexedPaths--) | Λαμβάνει έναν πίνακα με ευρετηριασμένες διαδρομές - έγγραφα ή φακέλους. |
|
|  | [delete(String[] paths, UpdateOptions options)](#delete-java.lang.String---com.groupdocs.search.options.UpdateOptions-) | Διαγράφει ευρετηριασμένα αρχεία ή φακέλους από το ευρετήριο. |
|
|  | [delete(UpdateOptions options, String[] documentKeys)](#delete-com.groupdocs.search.options.UpdateOptions-java.lang.String---) | Διαγράφει έγγραφα που έχουν ευρετηριαστεί από ροές ή δομές. |
|
|  | [notifyIndex(Notification notification)](#notifyIndex-com.groupdocs.search.Notification-) | Περνά το καθορισμένο αντικείμενο ειδοποίησης στο ευρετήριο για να εκτελέσει την ειδοποίηση. |
|
|  | [changeAttributes(AttributeChangeBatch batch)](#changeAttributes-com.groupdocs.search.common.AttributeChangeBatch-) | Εφαρμόζει την καθορισμένη δέσμη αλλαγών ιδιοτήτων στα ευρετηριασμένα έγγραφα χωρίς επανευρετηρίαση κατά τη λειτουργία ενημέρωσης. |
|
|  | [getAttributes(String path)](#getAttributes-java.lang.String-) | Λαμβάνει όλες τις ιδιότητες που σχετίζονται με το καθορισμένο ευρετηριασμένο έγγραφο. |
|
|  | [loadIntoMemoryCompletely(String indexFolder)](#loadIntoMemoryCompletely-java.lang.String-) | Φορτώνει ολόκληρο το ευρετήριο στη μνήμη. |
|
|  | [loadIntoMemoryCompletely(String indexFolder, IndexSettings settings)](#loadIntoMemoryCompletely-java.lang.String-com.groupdocs.search.IndexSettings-) | Φορτώνει ολόκληρο το ευρετήριο στη μνήμη. |
|
### Index() {#Index--}
```
public Index()
```


Αρχικοποιεί μια νέα παρουσία της  Index  κλάσης στη μνήμη.


Το παράδειγμα δείχνει πώς να δημιουργήσετε ευρετήριο στη μνήμη χωρίς αποθήκευση αρχείων στο δίσκο.

````
 ```

Index index = new Index();
 
```
 
````



### Index(IndexSettings settings) {#Index-com.groupdocs.search.IndexSettings-}
```
public Index(IndexSettings settings)
```


Αρχικοποιεί μια νέα παρουσία της  Index  κλάσης στη μνήμη με συγκεκριμένες ρυθμίσεις ευρετηρίου.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | Το αντικείμενο ρυθμίσεων ευρετηρίου. |


Το παράδειγμα δείχνει πώς να δημιουργήσετε ευρετήριο στη μνήμη χωρίς αποθήκευση αρχείων στο δίσκο με συγκεκριμένες ρυθμίσεις ευρετηρίου.

````
 ```

IndexSettings settings = new IndexSettings();
settings.setIndexType(IndexType.CompactIndex);
Index index = new Index(settings);
 
```
 
````

|

### Index(String indexFolder) {#Index-java.lang.String-}
```
public Index(String indexFolder)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης  Index  . Δημιουργεί ένα νέο ή ανοίγει ένα υπάρχον ευρετήριο στο δίσκο.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | indexFolder | java.lang.String | Η διαδρομή φακέλου του ευρετηρίου. |


Το παράδειγμα δείχνει πώς να δημιουργήσετε ένα ευρετήριο σε δίσκο ή να ανοίξετε ένα υπάρχον ευρετήριο.

````
 ```

String indexFolder = "c:\\MyIndex\\";
Index index = new Index(indexFolder);
 
```
 
````

|

### Index(String indexFolder, IndexSettings settings) {#Index-java.lang.String-com.groupdocs.search.IndexSettings-}
```
public Index(String indexFolder, IndexSettings settings)
```


Αρχικοποιεί μια νέα παρουσία της
Index
κλάσης.
Δημιουργεί ένα νέο ευρετήριο με συγκεκριμένες ρυθμίσεις ή ανοίγει ένα υπάρχον ευρετήριο στο δίσκο.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | indexFolder | java.lang.String | Η διαδρομή φακέλου του ευρετηρίου. |
|
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | Το αντικείμενο ρυθμίσεων ευρετηρίου. |

Το παράδειγμα δείχνει πώς να δημιουργήσετε ένα ευρετήριο σε δίσκο με συγκεκριμένες ρυθμίσεις ευρετηρίου.

````
 ```

String indexFolder = "c:\\MyIndex\\";
IndexSettings settings = new IndexSettings();
settings.setIndexType(IndexType.CompactIndex);
Index index = new Index(indexFolder, settings);
 
```
 
````

|

### Index(String indexFolder, boolean overwriteIfExists) {#Index-java.lang.String-boolean-}
```
public Index(String indexFolder, boolean overwriteIfExists)
```


Αρχικοποιεί μια νέα παρουσία της
Index
κλάσης.
Φορτώνει ένα υπάρχον ευρετήριο από το δίσκο εάν
overwriteIfExists
είναι
false
;
Δημιουργεί ένα νέο ευρετήριο στο δίσκο διαφορετικά.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | indexFolder | java.lang.String | Η διαδρομή φακέλου του ευρετηρίου. |
|
|  | overwriteIfExists | boolean | Η σημαία για την αντικατάσταση του φακέλου ευρετηρίου. |

Το παράδειγμα δείχνει πώς να δημιουργήσετε ένα νέο ευρετήριο σε φάκελο που ήδη περιέχει άλλο ευρετήριο.

````
 ```

String indexFolder = "c:\\MyIndex\\";
Index index = new Index(indexFolder, true);
 
```
 
````

|

### Index(String indexFolder, IndexSettings settings, boolean overwriteIfExists) {#Index-java.lang.String-com.groupdocs.search.IndexSettings-boolean-}
```
public Index(String indexFolder, IndexSettings settings, boolean overwriteIfExists)
```


Αρχικοποιεί μια νέα παρουσία της
Index
κλάσης.
Φορτώνει ένα υπάρχον ευρετήριο από το δίσκο εάν
overwriteIfExists
είναι
false
;
Δημιουργεί ένα νέο ευρετήριο στο δίσκο με συγκεκριμένες ρυθμίσεις ευρετηρίου διαφορετικά.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | indexFolder | java.lang.String | Η διαδρομή φακέλου του ευρετηρίου. |
|
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | Το αντικείμενο ρυθμίσεων ευρετηρίου. |
|
|  | overwriteIfExists | boolean | Η σημαία για την αντικατάσταση του φακέλου ευρετηρίου. |

Το παράδειγμα δείχνει πώς να δημιουργήσετε ένα ευρετήριο σε δίσκο με συγκεκριμένες ρυθμίσεις ευρετηρίου.

````
 ```

String indexFolder = "c:\\MyIndex\\";
IndexSettings settings = new IndexSettings();
settings.setIndexType(IndexType.CompactIndex);
Index index = new Index(indexFolder, settings, true);
 
```
 
````

|

### getEvents() {#getEvents--}
```
public final EventHub getEvents()
```


Λαμβάνει το κέντρο γεγονότων για την εγγραφή σε γεγονότα.


**Returns:**
[EventHub](../../com.groupdocs.search.events/eventhub) - The event hub for subscribing to events.

### getIndexInfo() {#getIndexInfo--}
```
public final IndexInfo getIndexInfo()
```


Αποκτά τις βασικές πληροφορίες για το ευρετήριο.


**Returns:**
[IndexInfo](../../com.groupdocs.search.common/indexinfo) - The basic information on the index.

### getRepository() {#getRepository--}
```
public final IndexRepository getRepository()
```


Αποκτά το αντικείμενο αποθετηρίου του ευρετηρίου εάν το ευρετήριο περιέχεται σε αυτό.


**Returns:**
[IndexRepository](../../com.groupdocs.search/indexrepository) - The index repository object.

### getIndexSettings() {#getIndexSettings--}
```
public final IndexSettings getIndexSettings()
```


Αποκτά τις ρυθμίσεις του ευρετηρίου.


**Returns:**
[IndexSettings](../../com.groupdocs.search/indexsettings) - The index settings.

### getDictionaries() {#getDictionaries--}
```
public final DictionaryRepository getDictionaries()
```


Αποκτά το αποθετήριο λεξικού.


**Returns:**
[DictionaryRepository](../../com.groupdocs.search.dictionaries/dictionaryrepository) - The dictionary repository.

### close() {#close--}
```
public final void close()
```


Απελευθερώνει όλους τους πόρους που χρησιμοποιούνται από το
Index
.


### add(String path) {#add-java.lang.String-}
```
public final void add(String path)
```


Εκτελεί λειτουργία ευρετηρίου.
Προσθέτει ένα αρχείο ή φάκελο με απόλυτη ή σχετική διαδρομή.
Τα έγγραφα από όλους τους υποφακέλους θα ευρετηριαστούν.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | path | java.lang.String | Η διαδρομή προς ένα αρχείο ή φάκελο που θα ευρετηριαστεί. |

Το παράδειγμα δείχνει πώς να προσθέσετε έγγραφα σε ένα ευρετήριο.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String folderPath = "c:\\MyDocuments\\";
String filePath = "c:\\Documents\\MyFile.txt";
Index index = new Index(indexFolder); // Δημιουργία ευρετηρίου στον καθορισμένο φάκελο
index.add(folderPath); // Δημιουργία ευρετηρίου εγγράφων στον καθορισμένο φάκελο
index.add(filePath); // Δημιουργία ευρετηρίου του καθορισμένου εγγράφου
 
```
 
````

|

### add(String path, IndexingOptions options) {#add-java.lang.String-com.groupdocs.search.options.IndexingOptions-}
```
public final void add(String path, IndexingOptions options)
```


Εκτελεί λειτουργία ευρετηρίου.
Προσθέτει ένα αρχείο ή φάκελο με απόλυτη ή σχετική διαδρομή.
Τα έγγραφα από όλους τους υποφακέλους θα ευρετηριαστούν.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | path | java.lang.String | Η διαδρομή προς ένα αρχείο ή φάκελο που θα ευρετηριαστεί. |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | Οι επιλογές δεικτοδότησης. |

Το παράδειγμα δείχνει πώς να προσθέσετε έγγραφα σε ένα ευρετήριο με συγκεκριμένες επιλογές δεικτοδότησης.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String folderPath = "c:\\MyDocuments\\";
String filePath = "c:\\Documents\\MyFile.txt";
Index index = new Index(indexFolder); // Δημιουργία ευρετηρίου στον καθορισμένο φάκελο
IndexingOptions options = new IndexingOptions();
options.setThreads(2); // Ορισμός του αριθμού των νημάτων ευρετηρίου
index.add(folderPath, options); // Δημιουργία ευρετηρίου εγγράφων στον καθορισμένο φάκελο
index.add(filePath, options); // Δημιουργία ευρετηρίου του καθορισμένου εγγράφου
 
```
 
````

|

### add(String[] paths) {#add-java.lang.String---}
```
public final void add(String[] paths)
```


Εκτελεί λειτουργία ευρετηρίου.
Προσθέτει αρχεία ή φακέλους με απόλυτη ή σχετική διαδρομή.
Τα έγγραφα από όλους τους υποφακέλους θα ευρετηριαστούν.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | paths | java.lang.String[] | Οι διαδρομές προς αρχεία ή φακέλους που θα δεικτοδοτηθούν. |

Το παράδειγμα δείχνει πώς να προσθέσετε έγγραφα σε ένα ευρετήριο.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String folderPath = "c:\\MyDocuments\\";
String filePath = "c:\\Documents\\MyFile.txt";
Index index = new Index(indexFolder); // Δημιουργία ευρετηρίου στον καθορισμένο φάκελο
String[] paths = new String[] { folderPath, filePath };
index.add(paths); // Δημιουργία ευρετηρίου εγγράφων στις καθορισμένες διαδρομές
 
```
 
````

|

### add(String[] paths, IndexingOptions options) {#add-java.lang.String---com.groupdocs.search.options.IndexingOptions-}
```
public final void add(String[] paths, IndexingOptions options)
```


Εκτελεί λειτουργία ευρετηρίου.
Προσθέτει αρχεία ή φακέλους με απόλυτη ή σχετική διαδρομή.
Τα έγγραφα από όλους τους υποφακέλους θα ευρετηριαστούν.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | paths | java.lang.String[] | Οι διαδρομές προς αρχεία ή φακέλους που θα δεικτοδοτηθούν. |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | Οι επιλογές δεικτοδότησης. |

Το παράδειγμα δείχνει πώς να προσθέσετε έγγραφα σε ένα ευρετήριο με συγκεκριμένες επιλογές δεικτοδότησης.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String folderPath = "c:\\MyDocuments\\";
String filePath = "c:\\Documents\\MyFile.txt";
Index index = new Index(indexFolder); // Δημιουργία ευρετηρίου στον καθορισμένο φάκελο
IndexingOptions options = new IndexingOptions();
options.setThreads(2); // Ορισμός του αριθμού των νημάτων ευρετηρίου
String[] paths = new String[] { folderPath, filePath };
index.add(paths, options); // Δημιουργία ευρετηρίου εγγράφων στις καθορισμένες διαδρομές
 
```
 
````

|

### add(Document[] documents, IndexingOptions options) {#add-com.groupdocs.search.Document---com.groupdocs.search.options.IndexingOptions-}
```
public final void add(Document[] documents, IndexingOptions options)
```


Εκτελεί λειτουργία ευρετηρίου.
Προσθέτει έγγραφα από το σύστημα αρχείων, τη ροή ή τη δομή.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | documents | [Document\[\]](../../com.groupdocs.search/document) | Τα έγγραφα από το σύστημα αρχείων, τη ροή ή τη δομή. |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | Οι επιλογές δεικτοδότησης. |
|

### add(ExtractedData[] data, IndexingOptions options) {#add-com.groupdocs.search.ExtractedData---com.groupdocs.search.options.IndexingOptions-}
```
public final void add(ExtractedData[] data, IndexingOptions options)
```


Εκτελεί λειτουργία ευρετηρίου.
Προσθέτει τα εξαγόμενα δεδομένα στο ευρετήριο.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | data | [ExtractedData\[\]](../../com.groupdocs.search/extracteddata) | Τα εξαγόμενα δεδομένα. |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | Οι επιλογές δεικτοδότησης. |
|

### update() {#update--}
```
public final void update()
```


Επαναευρετηρίζει έγγραφα που έχουν αλλάξει ή διαγραφεί από την τελευταία ενημέρωση.
Προσθέτει νέα αρχεία που έχουν προστεθεί στους δεικτοδοτημένους φακέλους.

Το παράδειγμα δείχνει πώς να ενημερώσετε ένα ευρετήριο.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Δημιουργία ευρετηρίου στον καθορισμένο φάκελο
index.add(documentsFolder); // Καταχώρηση εγγράφων από τον καθορισμένο φάκελο
// Διαγραφή εγγράφων από το φάκελο εγγράφων ή τροποποίηση τους ή προσθήκη νέων εγγράφων στο φάκελο
index.update(); // Ενημέρωση του ευρετηρίου
 
```
 
````



### update(UpdateOptions options) {#update-com.groupdocs.search.options.UpdateOptions-}
```
public final void update(UpdateOptions options)
```


Επαναευρετηρίζει έγγραφα που έχουν αλλάξει ή διαγραφεί από την τελευταία ενημέρωση.
Προσθέτει νέα αρχεία που έχουν προστεθεί στους δεικτοδοτημένους φακέλους.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | options | [UpdateOptions](../../com.groupdocs.search.options/updateoptions) | Οι επιλογές ενημέρωσης. |

Το παράδειγμα δείχνει πώς να ενημερώσετε ένα ευρετήριο με συγκεκριμένες επιλογές ενημέρωσης.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Δημιουργία ευρετηρίου στον καθορισμένο φάκελο
index.add(documentsFolder); // Καταχώρηση εγγράφων από τον καθορισμένο φάκελο
// Διαγραφή εγγράφων από το φάκελο εγγράφων ή τροποποίηση τους ή προσθήκη νέων εγγράφων στο φάκελο
UpdateOptions options = new UpdateOptions();
options.setThreads(2); // Ορισμός του αριθμού των νημάτων ευρετηρίου
index.update(options); // Ενημέρωση του ευρετηρίου
 
```
 
````

|

### getIndexingReports() {#getIndexingReports--}
```
public final IndexingReport[] getIndexingReports()
```


Λαμβάνει τις αναφορές για τις λειτουργίες ευρετηρίασης.


**Returns:**
com.groupdocs.search.common.IndexingReport[] - Οι αναφορές δεικτοδότησης.

Το παράδειγμα δείχνει πώς να λάβετε τις αναφορές δεικτοδότησης.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Δημιουργία ευρετηρίου στον καθορισμένο φάκελο
index.add(documentsFolder); // Καταχώρηση εγγράφων από τον καθορισμένο φάκελο
IndexingReport[] reports = index.getIndexingReports(); // Λήψη αναφορών δεικτοδότησης
 
```
 
````


### getSearchReports() {#getSearchReports--}
```
public final SearchReport[] getSearchReports()
```


Λαμβάνει τις αναφορές για τις λειτουργίες αναζήτησης.


**Returns:**
com.groupdocs.search.common.SearchReport[] - Οι αναφορές αναζήτησης.

Το παράδειγμα δείχνει πώς να λάβετε τις αναφορές αναζήτησης.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query1 = "Einstein";
String query2 = "Newton";
Index index = new Index(indexFolder); // Δημιουργία ευρετηρίου στον καθορισμένο φάκελο
index.add(documentsFolder); // Καταχώρηση εγγράφων από τον καθορισμένο φάκελο
SearchResult result1 = index.search(query1); // Αναζήτηση
SearchResult result2 = index.search(query2);
SearchResult result3 = index.search(query1 + " & " + query2);
SearchReport[] reports = index.getSearchReports(); // Λήψη αναφορών αναζήτησης
 
```
 
````


### search(String query) {#search-java.lang.String-}
```
public final SearchResult search(String query)
```


Αναζητά στο ευρετήριο.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | query | java.lang.String | Το ερώτημα αναζήτησης. |

Το παρακάτω παράδειγμα δείχνει πώς να εκτελέσετε απλή αναζήτηση.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // Δημιουργία ευρετηρίου στον καθορισμένο φάκελο
index.add(documentsFolder); // Καταχώρηση εγγράφων από τον καθορισμένο φάκελο
SearchResult result = index.search(query); // Αναζήτηση
 
```
 
````

Το παρακάτω παράδειγμα δείχνει πώς να εκτελέσετε αναζήτηση Regex.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Δημιουργία ευρετηρίου στον καθορισμένο φάκελο
index.add(documentsFolder); // Καταχώρηση εγγράφων από τον καθορισμένο φάκελο
String query = "^[0-9]{3,}"; // Το σύμβολο καροτέ στην αρχή του ερωτήματος αναζήτησης ενημερώνει το ευρετήριο ότι πρόκειται για ερώτημα Regex
SearchResult result = index.search(query); // Αναζήτηση
 
```
 
````

Το παρακάτω παράδειγμα δείχνει πώς να εκτελέσετε φασετοποιημένη αναζήτηση.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Δημιουργία ευρετηρίου στον καθορισμένο φάκελο
index.add(documentsFolder); // Καταχώρηση εγγράφων από τον καθορισμένο φάκελο
String query = "content:Newton"; // Η λέξη πριν από το άνω-κάτω τελεία στο ερώτημα υποδηλώνει το όνομα πεδίου του εγγράφου προς αναζήτηση
SearchResult result = index.search(query); // Αναζήτηση
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(String query, SearchOptions options) {#search-java.lang.String-com.groupdocs.search.options.SearchOptions-}
```
public final SearchResult search(String query, SearchOptions options)
```


Αναζητά στο ευρετήριο.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | query | java.lang.String | Το ερώτημα αναζήτησης. |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | Οι επιλογές αναζήτησης. |

Το παρακάτω παράδειγμα δείχνει πώς να εκτελέσετε ασαφή αναζήτηση.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Δημιουργία ευρετηρίου στον καθορισμένο φάκελο
index.add(documentsFolder); // Καταχώρηση εγγράφων από τον καθορισμένο φάκελο
SearchOptions options = new SearchOptions();
options.getFuzzySearch().setEnabled(true); // Ενεργοποίηση της ασαφούς αναζήτησης
options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(1)); // Ορισμός του αριθμού των πιθανών διαφορών για κάθε λέξη
// Τα διπλά εισαγωγικά στην αρχή και το τέλος ενημερώνουν το ευρετήριο ότι πρόκειται για ερώτημα αναζήτησης φράσης
String query = "\"The Pursuit of Happiness\"";
SearchResult result = index.search(query, options); // Αναζήτηση
 
```
 
````

Το παρακάτω παράδειγμα δείχνει πώς να εκτελέσετε αναζήτηση συνωνύμων.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Δημιουργία ευρετηρίου στον καθορισμένο φάκελο
index.add(documentsFolder); // Καταχώρηση εγγράφων από τον καθορισμένο φάκελο
SearchOptions options = new SearchOptions();
options.setUseSynonymSearch(true); // Ενεργοποίηση της αναζήτησης συνωνύμων
String query = "cry";
SearchResult result = index.search(query, options); // Αναζήτηση
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(SearchQuery query) {#search-com.groupdocs.search.SearchQuery-}
```
public final SearchResult search(SearchQuery query)
```


Αναζητά στο ευρετήριο.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | Το ερώτημα αναζήτησης. |

Το παρακάτω παράδειγμα δείχνει πώς να εκτελέσετε αναζήτηση χρησιμοποιώντας ερώτημα σε μορφή αντικειμένου.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Δημιουργία ευρετηρίου στον καθορισμένο φάκελο
index.add(documentsFolder); // Καταχώρηση εγγράφων από τον καθορισμένο φάκελο
// Δημιουργία υποερωτήματος 1
SearchQuery subquery1 = SearchQuery.createWordQuery("accommodation");
subquery1.setSearchOptions(new SearchOptions()); // Ορισμός επιλογών αναζήτησης μόνο για το υποερώτημα 1
subquery1.getSearchOptions().getFuzzySearch().setEnabled(true); // Ενεργοποίηση της ασαφούς αναζήτησης
subquery1.getSearchOptions().getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(3)); // Ορισμός μέγιστου αριθμού διαφορών
// Δημιουργία υποερωτήματος 2
SearchQuery subquery2 = SearchQuery.createNumericRangeQuery(1, 1000000);
// Δημιουργία υποερωτήματος 3
SearchQuery subquery3 = SearchQuery.createRegexQuery("(.)\\1");
// Συνδυασμός υποερωτημάτων σε ένα ερώτημα
SearchQuery query = SearchQuery.createPhraseSearchQuery(subquery1, subquery2, subquery3);
SearchResult result = index.search(query); // Αναζήτηση
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(SearchQuery query, SearchOptions options) {#search-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-}
```
public final SearchResult search(SearchQuery query, SearchOptions options)
```


Αναζητά στο ευρετήριο.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | Το ερώτημα αναζήτησης. |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | Οι επιλογές αναζήτησης. |

Το παρακάτω παράδειγμα δείχνει πώς να εκτελέσετε αναζήτηση χρησιμοποιώντας ερώτημα σε μορφή αντικειμένου.

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

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(SearchImage image, ImageSearchOptions options) {#search-com.groupdocs.search.common.SearchImage-com.groupdocs.search.options.ImageSearchOptions-}
```
public final ImageSearchResult search(SearchImage image, ImageSearchOptions options)
```


Εκτελεί αντίστροφη αναζήτηση εικόνας στο ευρετήριο.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | image | [SearchImage](../../com.groupdocs.search.common/searchimage) | Η εικόνα για αναζήτηση. |
|
|  | options | [ImageSearchOptions](../../com.groupdocs.search.options/imagesearchoptions) | Οι επιλογές αναζήτησης εικόνας. |
|

**Returns:**
[ImageSearchResult](../../com.groupdocs.search.results/imagesearchresult) - The result of a reverse image search.

### searchNext(ChunkSearchToken chunkSearchToken) {#searchNext-com.groupdocs.search.common.ChunkSearchToken-}
```
public final SearchResult searchNext(ChunkSearchToken chunkSearchToken)
```


Συνεχίζει την αναζήτηση τμημάτων που ξεκίνησε με τη μέθοδο Search.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | chunkSearchToken | [ChunkSearchToken](../../com.groupdocs.search.common/chunksearchtoken) | Το διακριτικό αναζήτησης τμημάτων. |

Το παράδειγμα δείχνει πώς να εκτελέσετε αναζήτηση τμημάτων.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // Δημιουργία ευρετηρίου στον καθορισμένο φάκελο
index.add(documentsFolder); // Καταχώρηση εγγράφων από τον καθορισμένο φάκελο
SearchOptions options = new SearchOptions();
options.setChunkSearch(true); // Ενεργοποίηση αναζήτησης τμημάτων
SearchResult result = index.search(query, options); // Έναρξη αναζήτησης τμημάτων
System.out.println("Αριθμός εγγράφων: " + result.getDocumentCount());
System.out.println("Αριθμός εμφανίσεων: " + result.getOccurrenceCount());
while (result.getNextChunkSearchToken() != null) {
result = index.searchNext(result.getNextChunkSearchToken()); // Συνέχιση αναζήτησης τμημάτων
System.out.println("Αριθμός εγγράφων: " + result.getDocumentCount());
System.out.println("Αριθμός εμφανίσεων: " + result.getOccurrenceCount());
}
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### searchNext(ChunkSearchToken chunkSearchToken, Cancellation cancellation) {#searchNext-com.groupdocs.search.common.ChunkSearchToken-com.groupdocs.search.common.Cancellation-}
```
public final SearchResult searchNext(ChunkSearchToken chunkSearchToken, Cancellation cancellation)
```


Συνεχίζει την αναζήτηση τμημάτων που ξεκίνησε με τη μέθοδο Search.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | chunkSearchToken | [ChunkSearchToken](../../com.groupdocs.search.common/chunksearchtoken) | Το διακριτικό αναζήτησης τμημάτων. |
|
|  | cancellation | [Cancellation](../../com.groupdocs.search.common/cancellation) | Το αντικείμενο ακύρωσης. |

Το παράδειγμα δείχνει πώς να εκτελέσετε αναζήτηση χρησιμοποιώντας ερώτημα σε μορφή αντικειμένου.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // Δημιουργία ευρετηρίου στον καθορισμένο φάκελο
index.add(documentsFolder); // Καταχώρηση εγγράφων από τον καθορισμένο φάκελο
Cancellation cancellation = new Cancellation(); // Αυτό το αντικείμενο ακύρωσης διακόπτει όλες τις συνέχειες της αναζήτησης εάν ακυρωθεί
SearchOptions options = new SearchOptions();
options.setChunkSearch(true); // Ενεργοποίηση αναζήτησης τμημάτων
options.setCancellation(cancellation);
SearchResult result = index.search(query, options); // Έναρξη αναζήτησης τμημάτων
System.out.println("Αριθμός εγγράφων: " + result.getDocumentCount());
System.out.println("Αριθμός εμφανίσεων: " + result.getOccurrenceCount());
while (result.getNextChunkSearchToken() != null) {
result = index.searchNext(result.getNextChunkSearchToken(), cancellation); // Συνέχιση αναζήτησης τμημάτων
System.out.println("Αριθμός εγγράφων: " + result.getDocumentCount());
System.out.println("Αριθμός εμφανίσεων: " + result.getOccurrenceCount());
}
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### optimize() {#optimize--}
```
public final void optimize()
```


Μειώνει τον αριθμό των τμημάτων του ευρετηρίου συγχωνεύοντάς τα μεταξύ τους.
Αυτή η λειτουργία βελτιώνει την απόδοση της αναζήτησης.

Το παράδειγμα δείχνει πώς να συγχωνεύσετε τμήματα ενός ευρετηρίου.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder1 = "c:\\MyDocuments1\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
String documentsFolder3 = "c:\\MyDocuments3\\";
Index index = new Index(indexFolder); // Δημιουργία ευρετηρίου στον καθορισμένο φάκελο
index.add(documentsFolder1); // Καταχώρηση εγγράφων από τον καθορισμένο φάκελο
index.add(documentsFolder2); // Κάθε κλήση στο AddToIndex δημιουργεί τουλάχιστον ένα νέο τμήμα στο ευρετήριο
index.add(documentsFolder3);
// Συγχώνευση τμημάτων του ευρετηρίου
index.optimize();
 
```
 
````



### optimize(MergeOptions options) {#optimize-com.groupdocs.search.options.MergeOptions-}
```
public final void optimize(MergeOptions options)
```


Μειώνει τον αριθμό των τμημάτων του ευρετηρίου συγχωνεύοντάς τα μεταξύ τους.
Αυτή η λειτουργία βελτιώνει την απόδοση της αναζήτησης.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | options | [MergeOptions](../../com.groupdocs.search.options/mergeoptions) | Οι επιλογές συγχώνευσης. |

Το παράδειγμα δείχνει πώς να συγχωνεύσετε τμήματα ενός ευρετηρίου με συγκεκριμένες επιλογές συγχώνευσης.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder1 = "c:\\MyDocuments1\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
String documentsFolder3 = "c:\\MyDocuments3\\";
Index index = new Index(indexFolder); // Δημιουργία ευρετηρίου στον καθορισμένο φάκελο
index.add(documentsFolder1); // Καταχώρηση εγγράφων από τον καθορισμένο φάκελο
index.add(documentsFolder2); // Κάθε κλήση στο AddToIndex δημιουργεί τουλάχιστον ένα νέο τμήμα στο ευρετήριο
index.add(documentsFolder3);
MergeOptions options = new MergeOptions();
options.setAsync(true); // Ασύγχρονη λειτουργία
options.setCancellation(new Cancellation()); // Δημιουργία αντικειμένου ακύρωσης
// Συγχώνευση τμημάτων του ευρετηρίου
index.optimize(options); // Αυτή η μέθοδος θα επιστρέψει πριν ολοκληρωθεί η λειτουργία
options.getCancellation().cancelAfter(10000); // Ορισμός μέγιστης διάρκειας της λειτουργίας σε 10 δευτερόλεπτα
 
```
 
````

|

### merge(Index index, MergeOptions options) {#merge-com.groupdocs.search.Index-com.groupdocs.search.options.MergeOptions-}
```
public final void merge(Index index, MergeOptions options)
```


Συγχωνεύει το καθορισμένο ευρετήριο με το τρέχον ευρετήριο.
Σημειώστε ότι το άλλο ευρετήριο δεν θα αλλάξει.


Εάν το άλλο ευρετήριο έχει προηγούμενη έκδοση, πρέπει να ενημερωθεί πριν από τη συγχώνευση με
IndexUpdater
.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | index | [Index](../../com.groupdocs.search/index) | Το ευρετήριο στο οποίο θα γίνει η συγχώνευση. |
|
|  | options | [MergeOptions](../../com.groupdocs.search.options/mergeoptions) | Οι επιλογές συγχώνευσης. |

Το παράδειγμα δείχνει πώς να συγχωνεύσετε ένα ευρετήριο στο τρέχον ευρετήριο.

````
 ```

String indexFolder1 = "c:\\MyIndex1\\";
String indexFolder2 = "c:\\MyIndex2\\";
String documentsFolder1 = "c:\\MyDocuments1\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
Index index1 = new Index(indexFolder1); // Δημιουργία index1
index1.add(documentsFolder1); // Καταχώρηση εγγράφων
Index index2 = new Index(indexFolder2); // Δημιουργία index2
index2.add(documentsFolder2); // Καταχώρηση εγγράφων
MergeOptions options = new MergeOptions();
options.setCancellation(new Cancellation()); // Δημιουργία αντικειμένου ακύρωσης
// Συγχώνευση index2 στο index1. Σημειώστε ότι τα αρχεία του index2 δεν θα αλλάξουν.
index1.merge(index2, options);
 
```
 
````

|

### merge(IndexRepository repository, MergeOptions options) {#merge-com.groupdocs.search.IndexRepository-com.groupdocs.search.options.MergeOptions-}
```
public final void merge(IndexRepository repository, MergeOptions options)
```


Συγχωνεύει ευρετήρια από το καθορισμένο αποθετήριο ευρετηρίων στο τρέχον ευρετήριο.
Σημειώστε ότι οι δείκτες στο αποθετήριο δεν θα αλλάξουν.


Εάν άλλοι δείκτες έχουν προηγούμενη έκδοση, πρέπει να ενημερωθούν πριν από τη συγχώνευση με
IndexUpdater
.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | repository | [IndexRepository](../../com.groupdocs.search/indexrepository) | Το αποθετήριο δεικτών για συγχώνευση. |
|
|  | options | [MergeOptions](../../com.groupdocs.search.options/mergeoptions) | Οι επιλογές συγχώνευσης. |

Το παράδειγμα δείχνει πώς να συγχωνεύσετε ένα αποθετήριο δεικτών στον τρέχοντα δείκτη.

````
 ```

String indexFolder1 = "c:\\MyIndex1\\";
String indexFolder2 = "c:\\MyIndex2\\";
String indexFolder3 = "c:\\MyIndex3\\";
String documentsFolder1 = "c:\\MyDocuments1\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
String documentsFolder3 = "c:\\MyDocuments3\\";
Index index1 = new Index(indexFolder1); // Δημιουργία index1
index1.add(documentsFolder1); // Καταχώρηση εγγράφων
IndexRepository repository = new IndexRepository(); // Δημιουργία αποθετηρίου δεικτών
Index index2 = repository.create(indexFolder2); // Δημιουργία index2
index2.add(documentsFolder2); // Καταχώρηση εγγράφων
Index index3 = repository.create(indexFolder3); // Δημιουργία index3
index3.add(documentsFolder3); // Καταχώριση εγγράφων
MergeOptions options = new MergeOptions();
options.setCancellation(new Cancellation()); // Δημιουργία αντικειμένου ακύρωσης
// Συγχώνευση όλων των δεικτών στο αποθετήριο δεικτών στο index1. Σημειώστε ότι τα index2 και index3 δεν θα αλλάξουν.
index1.merge(repository, options);
 
```
 
````

|

### highlight(FoundDocument document, Highlighter highlighter) {#highlight-com.groupdocs.search.results.FoundDocument-com.groupdocs.search.highlighters.Highlighter-}
```
public final void highlight(FoundDocument document, Highlighter highlighter)
```


Δημιουργεί κείμενο μορφοποιημένο σε HTML με επισημασμένους εντοπισμένους όρους.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | document | [FoundDocument](../../com.groupdocs.search.results/founddocument) | Το ευρεθέν έγγραφο. |
|
|  | highlighter | [Highlighter](../../com.groupdocs.search.highlighters/highlighter) | Ο επισημαστής αποτελεσμάτων αναζήτησης. |

Το παράδειγμα δείχνει πώς να επισημάνετε εμφανίσεις σε κείμενο μορφοποιημένο σε HTML.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentFolder = "c:\\MyDocuments\\";
// Δημιουργία ενός δείκτη
Index index = new Index(indexFolder);
// Καταχώριση εγγράφων από τον καθορισμένο φάκελο
index.add(documentFolder);
// Αναζήτηση της λέξης 'eternity'
SearchResult result = index.search("eternity");
// Επισημάνετε εμφανίσεις στο κείμενο
if (result.getDocumentCount() > 0) {
FoundDocument document = result.getFoundDocument(0); // Λήψη του πρώτου ευρεθέντος εγγράφου
OutputAdapter outputAdapter = new FileOutputAdapter("c:\\Highlighted.html"); // Δημιουργία προσαρμογέα εξόδου στο αρχείο
Highlighter highlighter = new HtmlHighlighter(outputAdapter); // Δημιουργία του αντικειμένου highlighter
index.highlight(document, highlighter); // Δημιουργία κειμένου μορφοποιημένου σε HTML με επισημασμένες εμφανίσεις
}
 
```
 
````

|

### highlight(FoundDocument document, Highlighter highlighter, HighlightOptions options) {#highlight-com.groupdocs.search.results.FoundDocument-com.groupdocs.search.highlighters.Highlighter-com.groupdocs.search.options.HighlightOptions-}
```
public final void highlight(FoundDocument document, Highlighter highlighter, HighlightOptions options)
```


Δημιουργεί κείμενο μορφοποιημένο σε HTML με επισημασμένους εντοπισμένους όρους.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | document | [FoundDocument](../../com.groupdocs.search.results/founddocument) | Το ευρεθέν έγγραφο. |
|
|  | highlighter | [Highlighter](../../com.groupdocs.search.highlighters/highlighter) | Ο επισημαστής αποτελεσμάτων αναζήτησης. |
|
|  | options | [HighlightOptions](../../com.groupdocs.search.options/highlightoptions) | Οι επιλογές επισήμανσης. |

Το παράδειγμα δείχνει πώς να επισημάνετε εμφανίσεις σε κείμενο μορφοποιημένο σε HTML.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentFolder = "c:\\MyDocuments\\";
// Δημιουργία ενός δείκτη
Index index = new Index(indexFolder);
// Καταχώριση εγγράφων από τον καθορισμένο φάκελο
index.add(documentFolder);
// Αναζήτηση της λέξης 'eternity'
SearchResult result = index.search("eternity");
// Επισημάνετε εμφανίσεις στο κείμενο
if (result.getDocumentCount() > 0) {
FoundDocument document = result.getFoundDocument(0); // Λήψη του πρώτου ευρεθέντος εγγράφου
OutputAdapter outputAdapter = new FileOutputAdapter("c:\\Highlighted.html"); // Δημιουργία προσαρμογέα εξόδου στο αρχείο
Highlighter highlighter = new HtmlHighlighter(outputAdapter); // Δημιουργία του αντικειμένου highlighter
HighlightOptions options = new HighlightOptions(); // Δημιουργία του αντικειμένου επιλογών επισήμανσης
options.setTermsBefore(5);
options.setTermsAfter(5);
options.setTermsTotal(15);
index.highlight(document, highlighter, options); // Δημιουργία κειμένου μορφοποιημένου σε HTML με επισημασμένες εμφανίσεις
}
 
```
 
````

|

### getIndexedDocuments() {#getIndexedDocuments--}
```
public final DocumentInfo[] getIndexedDocuments()
```


Λαμβάνει έναν πίνακα με όλα τα ευρετηριασμένα έγγραφα.


**Returns:**
com.groupdocs.search.results.DocumentInfo[] - Ένας πίνακας όλων των ευρετηριασμένων εγγράφων.

Το παράδειγμα δείχνει πώς να λάβετε μια λίστα με ευρετηριασμένα έγγραφα από ένα ευρετήριο.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Δημιουργία ευρετηρίου στον καθορισμένο φάκελο
Index index = new Index(indexFolder);
// Καταχώριση εγγράφων από τον καθορισμένο φάκελο
index.add(documentsFolder);
// Λήψη λίστας ευρετηριασμένων εγγράφων
DocumentInfo[] documents = index.getIndexedDocuments();
 
```
 
````


### getIndexedDocumentItems(DocumentInfo documentInfo) {#getIndexedDocumentItems-com.groupdocs.search.results.DocumentInfo-}
```
public final DocumentInfo[] getIndexedDocumentItems(DocumentInfo documentInfo)
```


Λαμβάνει έναν πίνακα με στοιχεία εγγράφου.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | documentInfo | [DocumentInfo](../../com.groupdocs.search.results/documentinfo) | Πληροφορίες εγγράφου. |

Το παράδειγμα δείχνει πώς να λάβετε μια λίστα με στοιχεία ενός ευρετηριασμένου εγγράφου από ένα ευρετήριο.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Δημιουργία ευρετηρίου στον καθορισμένο φάκελο
Index index = new Index(indexFolder);
// Καταχώριση εγγράφων από τον καθορισμένο φάκελο
index.add(documentsFolder);
// Λήψη λίστας ευρετηριασμένων εγγράφων
DocumentInfo[] documents = index.getIndexedDocuments();
for (int i = 0; i < documents.length; i++) {
DocumentInfo document = documents[i];
System.out.println(document.getFilePath());
DocumentInfo[] items = index.getIndexedDocumentItems(document); // Λήψη λίστας στοιχείων εγγράφου
for (int j = 0; j < items.length; j++) {
DocumentInfo item = items[j];
System.out.println("\t" + item.getInnerPath());
}
}
 
```
 
````

|

**Returns:**
com.groupdocs.search.results.DocumentInfo[] - Ένας πίνακας στοιχείων εγγράφου.

### GetIndexedDocument(String documentKey) {#GetIndexedDocument-java.lang.String-}
```
public DocumentInfo GetIndexedDocument(String documentKey)
```


Λαμβάνει ένα ευρετηριασμένο έγγραφο με βάση το κλειδί του εγγράφου.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | documentKey | java.lang.String | Το κλειδί του εγγράφου. |
|

**Returns:**
[DocumentInfo](../../com.groupdocs.search.results/documentinfo) - The indexed document.

### getDocumentText(DocumentInfo documentInfo, OutputAdapter adapter) {#getDocumentText-com.groupdocs.search.results.DocumentInfo-com.groupdocs.search.common.OutputAdapter-}
```
public final void getDocumentText(DocumentInfo documentInfo, OutputAdapter adapter)
```


Δημιουργεί το κείμενο ενός ευρετηριασμένου εγγράφου και το περνά μέσω ενός προσαρμογέα εξόδου.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | documentInfo | [DocumentInfo](../../com.groupdocs.search.results/documentinfo) | Οι πληροφορίες του ευρετηριασμένου εγγράφου. |
|
|  | adapter | [OutputAdapter](../../com.groupdocs.search.common/outputadapter) | Ο προσαρμογέας εξόδου. |

Το παράδειγμα δείχνει πώς να λάβετε το κείμενο ενός ευρετηριασμένου εγγράφου από ένα ευρετήριο.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Δημιουργία ευρετηρίου στον καθορισμένο φάκελο
Index index = new Index(indexFolder);
// Καταχώριση εγγράφων από τον καθορισμένο φάκελο
index.add(documentsFolder);
// Λήψη λίστας ευρετηριασμένων εγγράφων
DocumentInfo[] documents = index.getIndexedDocuments();
// Λήψη κειμένου εγγράφου
if (documents.length > 0) {
FileOutputAdapter outputAdapter = new FileOutputAdapter("C:\\Text.html");
index.getDocumentText(documents[0], outputAdapter);
}
 
```
 
````

|

### getDocumentText(DocumentInfo documentInfo, OutputAdapter adapter, TextOptions options) {#getDocumentText-com.groupdocs.search.results.DocumentInfo-com.groupdocs.search.common.OutputAdapter-com.groupdocs.search.options.TextOptions-}
```
public final void getDocumentText(DocumentInfo documentInfo, OutputAdapter adapter, TextOptions options)
```


Δημιουργεί κείμενο μορφοποιημένο σε HTML για το ευρετηριασμένο έγγραφο και το μεταφέρει μέσω του προσαρμογέα εξόδου.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | documentInfo | [DocumentInfo](../../com.groupdocs.search.results/documentinfo) | Οι πληροφορίες του ευρετηριασμένου εγγράφου. |
|
|  | adapter | [OutputAdapter](../../com.groupdocs.search.common/outputadapter) | Ο προσαρμογέας εξόδου. |
|
|  | options | [TextOptions](../../com.groupdocs.search.options/textoptions) | Οι επιλογές ανάκτησης κειμένου. |
|

### getIndexedPaths() {#getIndexedPaths--}
```
public final String[] getIndexedPaths()
```


Λαμβάνει έναν πίνακα με ευρετηριασμένες διαδρομές - έγγραφα ή φακέλους.


**Returns:**
java.lang.String[] - Ένας πίνακας διαδρομών που έχουν ευρετηριαστεί.

### delete(String[] paths, UpdateOptions options) {#delete-java.lang.String---com.groupdocs.search.options.UpdateOptions-}
```
public final DeleteResult delete(String[] paths, UpdateOptions options)
```


Διαγράφει αρχεία ή φακέλους που έχουν ευρετηριαστεί από το ευρετήριο. Στη συνέχεια ενημερώνει το ευρετήριο χωρίς τις διαγραμμένες διαδρομές.
Σημειώστε ότι ένα μεμονωμένο έγγραφο δεν μπορεί να διαγραφεί από το ευρετήριο εάν προστέθηκε στο ευρετήριο ως μέρος ενός φακέλου.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | paths | java.lang.String[] | Οι διαδρομές προς αρχεία ή φακέλους που θα διαγραφούν. |
|
|  | options | [UpdateOptions](../../com.groupdocs.search.options/updateoptions) | Οι επιλογές ενημέρωσης. |

Το παράδειγμα δείχνει πώς να διαγράψετε διαδρομές που έχουν ευρετηριαστεί από ένα ευρετήριο.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder1 = "c:\\MyDocuments\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
// Δημιουργία ευρετηρίου στον καθορισμένο φάκελο
Index index = new Index(indexFolder);
// Ευρετηρίαση εγγράφων από τους καθορισμένους φακέλους
index.add(documentsFolder1);
index.add(documentsFolder2);
// Λήψη διαδρομών που έχουν ευρετηριαστεί από το ευρετήριο
String[] indexedPaths1 = index.getIndexedPaths();
// Εγγραφή των διαδρομών που έχουν ευρετηριαστεί στην κονσόλα
System.out.println("Διαδρομές ευρετηρίου:");
for (String path : indexedPaths1) {
System.out.println("\t" + path);
}
// Διαγραφή διαδρομής ευρετηρίου από το ευρετήριο
DeleteResult deleteResult = index.delete(new String[] { documentsFolder1 }, new UpdateOptions());
// Λήψη διαδρομών που έχουν ευρετηριαστεί μετά τη διαγραφή
String[] indexedPaths2 = index.getIndexedPaths();
System.out.println("\nΔιαγραμμένες διαδρομές: " + deleteResult.getSuccessCount());
System.out.println("\nIndexed paths:");
for (String path : indexedPaths2) {
System.out.println("\t" + path);
}
 
```
 
````

|

**Returns:**
[DeleteResult](../../com.groupdocs.search.results/deleteresult) - An object describing the result of deleting files or folders from the index.

### delete(UpdateOptions options, String[] documentKeys) {#delete-com.groupdocs.search.options.UpdateOptions-java.lang.String---}
```
public final DeleteResult delete(UpdateOptions options, String[] documentKeys)
```


Διαγράφει έγγραφα που έχουν ευρετηριαστεί από ροές ή δομές. Στη συνέχεια ενημερώνει το ευρετήριο χωρίς τα διαγραμμένα έγγραφα.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | options | [UpdateOptions](../../com.groupdocs.search.options/updateoptions) | Οι επιλογές ενημέρωσης. |
|
|  | documentKeys | java.lang.String[] | Τα κλειδιά των εγγράφων που προστέθηκαν από ροές ή δομές. |
|

**Returns:**
[DeleteResult](../../com.groupdocs.search.results/deleteresult) - An object describing the result of deleting documents from the index.

### notifyIndex(Notification notification) {#notifyIndex-com.groupdocs.search.Notification-}
```
public final boolean notifyIndex(Notification notification)
```


Περνά το καθορισμένο αντικείμενο ειδοποίησης στο ευρετήριο για να εκτελέσει την ειδοποίηση.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | notification | [Notification](../../com.groupdocs.search/notification) | Το αντικείμενο ειδοποίησης. |
|

**Returns:**
boolean - Επιστρέφει  true  εάν η ειδοποίηση εκτελέστηκε επιτυχώς· διαφορετικά  false .

### changeAttributes(AttributeChangeBatch batch) {#changeAttributes-com.groupdocs.search.common.AttributeChangeBatch-}
```
public final void changeAttributes(AttributeChangeBatch batch)
```


Εφαρμόζει την καθορισμένη δέσμη αλλαγών ιδιοτήτων στα ευρετηριασμένα έγγραφα χωρίς επανευρετηρίαση κατά τη λειτουργία ενημέρωσης.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | batch | [AttributeChangeBatch](../../com.groupdocs.search.common/attributechangebatch) | Η παρτίδα αλλαγής ιδιότητας. |
|

### getAttributes(String path) {#getAttributes-java.lang.String-}
```
public final String[] getAttributes(String path)
```


Λαμβάνει όλες τις ιδιότητες που σχετίζονται με το καθορισμένο ευρετηριασμένο έγγραφο.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | path | java.lang.String | Η διαδρομή του εγγράφου. |
|

**Returns:**
java.lang.String[] - Ιδιότητες που σχετίζονται με το έγγραφο.

### loadIntoMemoryCompletely(String indexFolder) {#loadIntoMemoryCompletely-java.lang.String-}
```
public static Index loadIntoMemoryCompletely(String indexFolder)
```


Φορτώνει ολόκληρο το ευρετήριο στη μνήμη.
Οποιεσδήποτε αλλαγές στο ευρετήριο δεν αποθηκεύονται αυτόματα στον αρχικό φάκελο.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | indexFolder | java.lang.String | Η διαδρομή φακέλου του ευρετηρίου. |
|

**Returns:**
[Index](../../com.groupdocs.search/index) - The loaded in-memory index.

### loadIntoMemoryCompletely(String indexFolder, IndexSettings settings) {#loadIntoMemoryCompletely-java.lang.String-com.groupdocs.search.IndexSettings-}
```
public static Index loadIntoMemoryCompletely(String indexFolder, IndexSettings settings)
```


Φορτώνει ολόκληρο το ευρετήριο στη μνήμη.
Οποιεσδήποτε αλλαγές στο ευρετήριο δεν αποθηκεύονται αυτόματα στον αρχικό φάκελο.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | indexFolder | java.lang.String | Η διαδρομή φακέλου του ευρετηρίου. |
|
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | Το αντικείμενο ρυθμίσεων ευρετηρίου. |
|

**Returns:**
[Index](../../com.groupdocs.search/index) - The loaded in-memory index.

