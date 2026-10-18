---
title: "IndexSettings"
second_title: "GroupDocs.Search για Java API Reference"
description: "Αντιπροσωπεύει τις ρυθμίσεις του ευρετηρίου που επιτρέπουν την προσαρμογή των λειτουργιών ευρετηρίασης."
type: docs
weight: 19
url: /el/java/com.groupdocs.search/indexsettings/
---
**Inheritance:**
java.lang.Object
```
public class IndexSettings
```

Αντιπροσωπεύει τις ρυθμίσεις του ευρετηρίου που επιτρέπουν την προσαρμογή των λειτουργιών ευρετηρίασης.


**Learn more**

* [Search index settings](../https://docs.groupdocs.com/display/searchjava/Search+index+settings)


Το παράδειγμα δείχνει μια τυπική χρήση της κλάσης.

````
 ```

String indexFolder = "c:\\MyIndex\\";
IndexSettings settings = new IndexSettings();
settings.setIndexType(IndexType.CompactIndex); // Ορισμός του τύπου ευρετηρίου
Index index = new Index(indexFolder, settings); // Δημιουργία ενός ευρετηρίου
 
```
 
````


## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [IndexSettings()](#IndexSettings--) | Αρχικοποιεί μια νέα παρουσία της κλάσης  IndexSettings  . |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getInMemoryIndex()](#getInMemoryIndex--) | Λαμβάνει μια τιμή που υποδεικνύει εάν το ευρετήριο αποθηκεύεται στη μνήμη ή στο δίσκο. |
|
|  | [getUseStopWords()](#getUseStopWords--) | Λαμβάνει μια τιμή που υποδεικνύει εάν θα χρησιμοποιηθούν λέξεις-σταματητές ή όχι. |
|
|  | [setUseStopWords(boolean value)](#setUseStopWords-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν θα χρησιμοποιηθούν λέξεις-σταματητές ή όχι. |
|
|  | [getMaxIndexingReportCount()](#getMaxIndexingReportCount--) | Λαμβάνει τον μέγιστο αριθμό αναφορών ευρετηρίου. |
|
|  | [setMaxIndexingReportCount(int value)](#setMaxIndexingReportCount-int-) | Ορίζει τον μέγιστο αριθμό αναφορών ευρετηρίου. |
|
|  | [getMaxSearchReportCount()](#getMaxSearchReportCount--) | Λαμβάνει τον μέγιστο αριθμό αναφορών αναζήτησης. |
|
|  | [setMaxSearchReportCount(int value)](#setMaxSearchReportCount-int-) | Ορίζει τον μέγιστο αριθμό αναφορών αναζήτησης. |
|
|  | [getUseCharacterReplacements()](#getUseCharacterReplacements--) | Λαμβάνει μια τιμή που υποδεικνύει εάν θα χρησιμοποιηθούν αντικαταστάσεις χαρακτήρων ή όχι. |
|
|  | [setUseCharacterReplacements(boolean value)](#setUseCharacterReplacements-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν θα χρησιμοποιηθούν αντικαταστάσεις χαρακτήρων ή όχι. |
|
|  | [getDocumentFilter()](#getDocumentFilter--) | Λαμβάνει ένα φίλτρο εγγράφου. |
|
|  | [setDocumentFilter(DocumentFilter value)](#setDocumentFilter-com.groupdocs.search.DocumentFilter-) | Ορίζει ένα φίλτρο εγγράφου. |
|
|  | [getTextStorageSettings()](#getTextStorageSettings--) | Λαμβάνει τις ρυθμίσεις αποθήκευσης κειμένου. |
|
|  | [setTextStorageSettings(TextStorageSettings value)](#setTextStorageSettings-com.groupdocs.search.options.TextStorageSettings-) | Ορίζει τις ρυθμίσεις αποθήκευσης κειμένου. |
|
|  | [getIndexType()](#getIndexType--) | Λαμβάνει τον τύπο ευρετηρίου. |
|
|  | [setIndexType(IndexType value)](#setIndexType-com.groupdocs.search.options.IndexType-) | Ορίζει τον τύπο ευρετηρίου. |
|
|  | [getSearchThreads()](#getSearchThreads--) | Λαμβάνει τον αριθμό των νημάτων που χρησιμοποιούνται για την αναζήτηση. |
|
|  | [setSearchThreads(NumberOfThreads value)](#setSearchThreads-com.groupdocs.search.options.NumberOfThreads-) | Ορίζει τον αριθμό των νημάτων που χρησιμοποιούνται για την αναζήτηση. |
|
|  | [getCustomExtractors()](#getCustomExtractors--) | Λαμβάνει τη συλλογή προσαρμοσμένων εξαγωγέων. |
|
|  | [getLogger()](#getLogger--) | Λαμβάνει έναν καταγραφέα που χρησιμοποιείται για την καταγραφή συμβάντων και σφαλμάτων στο ευρετήριο. |
|
|  | [setLogger(ILogger value)](#setLogger-com.groupdocs.search.common.ILogger-) | Ορίζει έναν καταγραφέα που χρησιμοποιείται για την καταγραφή συμβάντων και σφαλμάτων στο ευρετήριο. |
|
### IndexSettings() {#IndexSettings--}
```
public IndexSettings()
```


Αρχικοποιεί μια νέα παρουσία της κλάσης  IndexSettings  .


### getInMemoryIndex() {#getInMemoryIndex--}
```
public final boolean getInMemoryIndex()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν το ευρετήριο αποθηκεύεται στη μνήμη ή στο δίσκο.


**Returns:**
boolean - Μια τιμή που υποδεικνύει αν το ευρετήριο αποθηκεύεται στη μνήμη ή στο δίσκο.

### getUseStopWords() {#getUseStopWords--}
```
public final boolean getUseStopWords()
```


Λαμβάνει μια τιμή που υποδεικνύει αν θα χρησιμοποιηθούν λέξεις-σταματητές ή όχι. Η προεπιλεγμένη τιμή είναι  true .


**Returns:**
boolean - Μια τιμή που υποδεικνύει αν θα χρησιμοποιηθούν λέξεις-σταματητές ή όχι.

### setUseStopWords(boolean value) {#setUseStopWords-boolean-}
```
public final void setUseStopWords(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει αν θα χρησιμοποιηθούν λέξεις-σταματητές ή όχι. Η προεπιλεγμένη τιμή είναι  true .


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | τιμή | boolean | Μια τιμή που υποδεικνύει αν θα χρησιμοποιηθούν λέξεις-σταματητές ή όχι. |
|

### getMaxIndexingReportCount() {#getMaxIndexingReportCount--}
```
public final int getMaxIndexingReportCount()
```


Λαμβάνει τον μέγιστο αριθμό αναφορών ευρετηρίου. Η προεπιλεγμένη τιμή είναι  5 .


**Returns:**
int - Ο μέγιστος αριθμός αναφορών ευρετηρίου.

### setMaxIndexingReportCount(int value) {#setMaxIndexingReportCount-int-}
```
public final void setMaxIndexingReportCount(int value)
```


Ορίζει τον μέγιστο αριθμό αναφορών ευρετηρίου. Η προεπιλεγμένη τιμή είναι  5 .


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | τιμή | int | Ο μέγιστος αριθμός αναφορών ευρετηρίου. |
|

### getMaxSearchReportCount() {#getMaxSearchReportCount--}
```
public final int getMaxSearchReportCount()
```


Λαμβάνει τον μέγιστο αριθμό αναφορών αναζήτησης. Η προεπιλεγμένη τιμή είναι  10 .


**Returns:**
int - Ο μέγιστος αριθμός αναφορών αναζήτησης.

### setMaxSearchReportCount(int value) {#setMaxSearchReportCount-int-}
```
public final void setMaxSearchReportCount(int value)
```


Ορίζει τον μέγιστο αριθμό αναφορών αναζήτησης. Η προεπιλεγμένη τιμή είναι  10 .


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | τιμή | int | Ο μέγιστος αριθμός αναφορών αναζήτησης. |
|

### getUseCharacterReplacements() {#getUseCharacterReplacements--}
```
public final boolean getUseCharacterReplacements()
```


Λαμβάνει μια τιμή που υποδεικνύει αν θα χρησιμοποιηθούν αντικαταστάσεις χαρακτήρων ή όχι. Η προεπιλεγμένη τιμή είναι  false .


**Returns:**
boolean - Μια τιμή που υποδεικνύει αν θα χρησιμοποιηθούν αντικαταστάσεις χαρακτήρων ή όχι.

### setUseCharacterReplacements(boolean value) {#setUseCharacterReplacements-boolean-}
```
public final void setUseCharacterReplacements(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει αν θα χρησιμοποιηθούν αντικαταστάσεις χαρακτήρων ή όχι. Η προεπιλεγμένη τιμή είναι  false .


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | τιμή | boolean | Μια τιμή που υποδεικνύει αν θα χρησιμοποιηθούν αντικαταστάσεις χαρακτήρων ή όχι. |
|

### getDocumentFilter() {#getDocumentFilter--}
```
public final DocumentFilter getDocumentFilter()
```


Λαμβάνει ένα φίλτρο εγγράφου. Το  DocumentFilter  λειτουργεί με τη λογική ένταξης. Χρησιμοποιήστε την κλάση  DocumentFilter  για τη δημιουργία ενός στιγμιότυπου φίλτρου εγγράφου. Η προεπιλεγμένη τιμή είναι  null , που σημαίνει ότι όλα τα προστιθέμενα έγγραφα ευρετηριάζονται.


**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - The document filter.

Το παράδειγμα δείχνει πώς να ορίσετε το φίλτρο εγγράφου.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Δημιουργία φίλτρου που παραλείπει έγγραφα με επεκτάσεις '.doc', '.docx', '.rtf'
IndexSettings settings = new IndexSettings();
DocumentFilter fileExtensionFilter = DocumentFilter.createFileExtension(".doc", ".docx", ".rtf"); // Δημιουργία φίλτρου κατά επέκταση αρχείου
DocumentFilter invertedFilter = DocumentFilter.createNot(fileExtensionFilter); // Αντιστροφή φίλτρου κατά επέκταση αρχείου
settings.setDocumentFilter(invertedFilter);
// Δημιουργία ευρετηρίου στον καθορισμένο φάκελο
Index index = new Index(indexFolder, settings);
// Ευρετηρίαση εγγράφων
index.add(documentsFolder);
// Αναζήτηση
SearchResult result = index.search("Einstein");
 
```
 
````


### setDocumentFilter(DocumentFilter value) {#setDocumentFilter-com.groupdocs.search.DocumentFilter-}
```
public final void setDocumentFilter(DocumentFilter value)
```


Ορίζει ένα φίλτρο εγγράφου. Το DocumentFilter λειτουργεί με λογική ένταξης. Χρησιμοποιήστε την κλάση GroupDocs.Search.Options.DocumentFilter για τη δημιουργία στιγμιοτύπων φίλτρου εγγράφου. Η προεπιλεγμένη τιμή είναι null, που σημαίνει ότι όλα τα προστιθέμενα έγγραφα ευρετηριάζονται.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | value | [DocumentFilter](../../com.groupdocs.search/documentfilter) | Το φίλτρο εγγράφου. |

Το παράδειγμα δείχνει πώς να ορίσετε το φίλτρο εγγράφου.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Δημιουργία φίλτρου που παραλείπει έγγραφα με επεκτάσεις '.doc', '.docx', '.rtf'
IndexSettings settings = new IndexSettings();
DocumentFilter fileExtensionFilter = DocumentFilter.createFileExtension(".doc", ".docx", ".rtf"); // Δημιουργία φίλτρου κατά επέκταση αρχείου
DocumentFilter invertedFilter = DocumentFilter.createNot(fileExtensionFilter); // Αντιστροφή φίλτρου κατά επέκταση αρχείου
settings.setDocumentFilter(invertedFilter);
// Δημιουργία ευρετηρίου στον καθορισμένο φάκελο
Index index = new Index(indexFolder, settings);
// Ευρετηρίαση εγγράφων
index.add(documentsFolder);
// Αναζήτηση
SearchResult result = index.search("Einstein");
 
```
 
````

|

### getTextStorageSettings() {#getTextStorageSettings--}
```
public final TextStorageSettings getTextStorageSettings()
```


Λαμβάνει τις ρυθμίσεις αποθήκευσης κειμένου. Η προεπιλεγμένη τιμή είναι null, που σημαίνει ότι τα κείμενα των εγγράφων δεν αποθηκεύονται.


**Returns:**
[TextStorageSettings](../../com.groupdocs.search.options/textstoragesettings) - The text storage settings.

Το παράδειγμα δείχνει πώς να ορίσετε τις ρυθμίσεις αποθήκευσης κειμένου.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Δημιουργία στιγμιοτύπου ρυθμίσεων ευρετηρίου
IndexSettings settings = new IndexSettings();
settings.setTextStorageSettings(new TextStorageSettings(Compression.High)); // Ορισμός υψηλού επιπέδου συμπίεσης για την αποθήκευση κειμένου του ευρετηρίου
// Δημιουργία ευρετηρίου στον καθορισμένο φάκελο
Index index = new Index(indexFolder, settings);
// Ευρετηρίαση εγγράφων
index.add(documentsFolder);
// Αναζήτηση
SearchResult result = index.search("Einstein");
 
```
 
````


### setTextStorageSettings(TextStorageSettings value) {#setTextStorageSettings-com.groupdocs.search.options.TextStorageSettings-}
```
public final void setTextStorageSettings(TextStorageSettings value)
```


Ορίζει τις ρυθμίσεις αποθήκευσης κειμένου. Η προεπιλεγμένη τιμή είναι null, που σημαίνει ότι τα κείμενα των εγγράφων δεν αποθηκεύονται.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | value | [TextStorageSettings](../../com.groupdocs.search.options/textstoragesettings) | Οι ρυθμίσεις αποθήκευσης κειμένου. |

Το παράδειγμα δείχνει πώς να ορίσετε τις ρυθμίσεις αποθήκευσης κειμένου.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Δημιουργία στιγμιοτύπου ρυθμίσεων ευρετηρίου
IndexSettings settings = new IndexSettings();
settings.setTextStorageSettings(new TextStorageSettings(Compression.High)); // Ορισμός υψηλού επιπέδου συμπίεσης για την αποθήκευση κειμένου του ευρετηρίου
// Δημιουργία ευρετηρίου στον καθορισμένο φάκελο
Index index = new Index(indexFolder, settings);
// Ευρετηρίαση εγγράφων
index.add(documentsFolder);
// Αναζήτηση
SearchResult result = index.search("Einstein");
 
```
 
````

|

### getIndexType() {#getIndexType--}
```
public final IndexType getIndexType()
```


Λαμβάνει τον τύπο ευρετηρίου. Η προεπιλεγμένη τιμή είναι GroupDocs.Search.Options.IndexType.NormalIndex.


**Returns:**
[IndexType](../../com.groupdocs.search.options/indextype) - The index type.

### setIndexType(IndexType value) {#setIndexType-com.groupdocs.search.options.IndexType-}
```
public final void setIndexType(IndexType value)
```


Ορίζει τον τύπο ευρετηρίου. Η προεπιλεγμένη τιμή είναι GroupDocs.Search.Options.IndexType.NormalIndex.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | value | [IndexType](../../com.groupdocs.search.options/indextype) | Ο τύπος ευρετηρίου. |
|

### getSearchThreads() {#getSearchThreads--}
```
public final NumberOfThreads getSearchThreads()
```


Λαμβάνει τον αριθμό των νημάτων που χρησιμοποιούνται για την αναζήτηση. Η προεπιλεγμένη τιμή είναι GroupDocs.Search.Options.NumberOfThreads.Default, που σημαίνει ότι η αναζήτηση θα εκτελείται χρησιμοποιώντας αριθμό νημάτων ίσο με τον αριθμό των πυρήνων του επεξεργαστή.


**Returns:**
[NumberOfThreads](../../com.groupdocs.search.options/numberofthreads) - The number of threads used for the search.

### setSearchThreads(NumberOfThreads value) {#setSearchThreads-com.groupdocs.search.options.NumberOfThreads-}
```
public final void setSearchThreads(NumberOfThreads value)
```


Ορίζει τον αριθμό των νημάτων που χρησιμοποιούνται για την αναζήτηση. Η προεπιλεγμένη τιμή είναι GroupDocs.Search.Options.NumberOfThreads.Default, που σημαίνει ότι η αναζήτηση θα εκτελείται χρησιμοποιώντας αριθμό νημάτων ίσο με τον αριθμό των πυρήνων του επεξεργαστή.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | value | [NumberOfThreads](../../com.groupdocs.search.options/numberofthreads) | Ο αριθμός των νημάτων που χρησιμοποιούνται για την αναζήτηση. |
|

### getCustomExtractors() {#getCustomExtractors--}
```
public final CustomExtractorCollection getCustomExtractors()
```


Λαμβάνει τη συλλογή προσαρμοσμένων εξαγωγέων. Το πλήρες παράδειγμα υλοποίησης ενός προσαρμοσμένου εξαγωγέα παρουσιάζεται στην τεκμηρίωση για τη διεπαφή GroupDocs.Search.Common.IFieldExtractor.


**Returns:**
[CustomExtractorCollection](../../com.groupdocs.search.common/customextractorcollection) - The custom extractor collection.

### getLogger() {#getLogger--}
```
public final ILogger getLogger()
```


Λαμβάνει έναν καταγραφέα που χρησιμοποιείται για την καταγραφή συμβάντων και σφαλμάτων στο ευρετήριο. Σημειώστε ότι ο καταγραφέας δεν αποθηκεύεται και πρέπει να δημιουργείται και να ανατίθεται κάθε φορά που το ευρετήριο δημιουργείται ή φορτώνεται.


**Returns:**
[ILogger](../../com.groupdocs.search.common/ilogger) - A logger that is used for logging events and errors in the index.

### setLogger(ILogger value) {#setLogger-com.groupdocs.search.common.ILogger-}
```
public final void setLogger(ILogger value)
```


Ορίζει έναν καταγραφέα που χρησιμοποιείται για την καταγραφή συμβάντων και σφαλμάτων στο ευρετήριο. Σημειώστε ότι ο καταγραφέας δεν αποθηκεύεται και πρέπει να δημιουργείται και να εκχωρείται κάθε φορά που το ευρετήριο δημιουργείται ή φορτώνεται.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | value | [ILogger](../../com.groupdocs.search.common/ilogger) | Ένας καταγραφέας που χρησιμοποιείται για την καταγραφή συμβάντων και σφαλμάτων στο ευρετήριο. |
|

