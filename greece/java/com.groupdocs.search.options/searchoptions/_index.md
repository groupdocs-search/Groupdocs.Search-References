---
title: "SearchOptions"
second_title: "GroupDocs.Search για Java API Reference"
description: "Παρέχει επιλογές για τη λειτουργία αναζήτησης."
type: docs
weight: 34
url: /el/java/com.groupdocs.search.options/searchoptions/
---
**Inheritance:**
java.lang.Object
```
public class SearchOptions
```

Παρέχει επιλογές για τη λειτουργία αναζήτησης.


**Learn more**

* [Search options](../https://docs.groupdocs.com/display/searchjava/Search+options)

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [SearchOptions()](#SearchOptions--) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης  SearchOptions . |
|
|  | [SearchOptions(Object data)](#SearchOptions-java.lang.Object-) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης  SearchOptions . |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getUseSynonymSearch()](#getUseSynonymSearch--) | Λαμβάνει τη σημαία χρήσης συνωνύμων στην αναζήτηση. |
|
|  | [setUseSynonymSearch(boolean value)](#setUseSynonymSearch-boolean-) | Ορίζει τη σημαία χρήσης συνωνύμων στην αναζήτηση. |
|
|  | [getUseHomophoneSearch()](#getUseHomophoneSearch--) | Λαμβάνει τη σημαία χρήσης ομόηχων στην αναζήτηση. |
|
|  | [setUseHomophoneSearch(boolean value)](#setUseHomophoneSearch-boolean-) | Ορίζει τη σημαία χρήσης ομόηχων στην αναζήτηση. |
|
|  | [getUseWordFormsSearch()](#getUseWordFormsSearch--) | Λαμβάνει τη σημαία χρήσης διαφορετικών μορφών λέξεων στην αναζήτηση. |
|
|  | [setUseWordFormsSearch(boolean value)](#setUseWordFormsSearch-boolean-) | Ορίζει τη σημαία χρήσης διαφορετικών μορφών λέξεων στην αναζήτηση. |
|
|  | [getRetrieveAttributes()](#getRetrieveAttributes--) | Λαμβάνει τη σημαία ανάκτησης χαρακτηριστικών που σχετίζονται με τα ευρεθέντα έγγραφα. |
|
|  | [setRetrieveAttributes(boolean value)](#setRetrieveAttributes-boolean-) | Ορίζει τη σημαία για την ανάκτηση των ιδιοτήτων που σχετίζονται με τα ευρεθέντα έγγραφα. |
|
|  | [getFuzzySearch()](#getFuzzySearch--) | Λαμβάνει τις επιλογές ασαφούς αναζήτησης. |
|
|  | [getSpellingCorrector()](#getSpellingCorrector--) | Λαμβάνει τις επιλογές διορθωτή ορθογραφίας. |
|
|  | [getKeyboardLayoutCorrector()](#getKeyboardLayoutCorrector--) | Λαμβάνει τις επιλογές διορθωτή διάταξης πληκτρολογίου. |
|
|  | [getUseCaseSensitiveSearch()](#getUseCaseSensitiveSearch--) | Λαμβάνει τη σημαία της αναζήτησης με διάκριση πεζών-κεφαλαίων. |
|
|  | [setUseCaseSensitiveSearch(boolean value)](#setUseCaseSensitiveSearch-boolean-) | Ορίζει τη σημαία της αναζήτησης με διάκριση πεζών-κεφαλαίων. |
|
|  | [getMaxTotalOccurrenceCount()](#getMaxTotalOccurrenceCount--) | Λαμβάνει το μέγιστο συνολικό αριθμό εμφανίσεων όλων των όρων σε ένα ερώτημα αναζήτησης. |
|
|  | [setMaxTotalOccurrenceCount(int value)](#setMaxTotalOccurrenceCount-int-) | Ορίζει το μέγιστο συνολικό αριθμό εμφανίσεων όλων των όρων σε ένα ερώτημα αναζήτησης. |
|
|  | [getMaxOccurrenceCountPerTerm()](#getMaxOccurrenceCountPerTerm--) | Λαμβάνει το μέγιστο αριθμό εμφανίσεων κάθε όρου σε ένα ερώτημα αναζήτησης. |
|
|  | [setMaxOccurrenceCountPerTerm(int value)](#setMaxOccurrenceCountPerTerm-int-) | Ορίζει το μέγιστο αριθμό εμφανίσεων κάθε όρου σε ένα ερώτημα αναζήτησης. |
|
|  | [getDateFormats()](#getDateFormats--) | Λαμβάνει τη συλλογή των μορφών ημερομηνίας για αναζήτηση εύρους ημερομηνιών. |
|
|  | [isChunkSearch()](#isChunkSearch--) | Λαμβάνει τη σημαία της αναζήτησης ανά τμήματα. |
|
|  | [setChunkSearch(boolean value)](#setChunkSearch-boolean-) | Ορίζει τη σημαία της αναζήτησης ανά τμήματα. |
|
|  | [getSearchDocumentFilter()](#getSearchDocumentFilter--) | Λαμβάνει το φίλτρο εγγράφου αναζήτησης. |
|
|  | [setSearchDocumentFilter(ISearchDocumentFilter value)](#setSearchDocumentFilter-com.groupdocs.search.options.ISearchDocumentFilter-) | Ορίζει το φίλτρο εγγράφου αναζήτησης. |
|
|  | [getCancellation()](#getCancellation--) | Λαμβάνει το αντικείμενο ακύρωσης της λειτουργίας. |
|
|  | [setCancellation(Cancellation value)](#setCancellation-com.groupdocs.search.common.Cancellation-) | Ορίζει το αντικείμενο ακύρωσης της λειτουργίας. |
|
| [getCore()](#getCore--) |  |
### SearchOptions() {#SearchOptions--}
```
public SearchOptions()
```


Αρχικοποιεί ένα νέο αντικείμενο της κλάσης  SearchOptions .


### SearchOptions(Object data) {#SearchOptions-java.lang.Object-}
```
public SearchOptions(Object data)
```


Αρχικοποιεί ένα νέο αντικείμενο της κλάσης  SearchOptions .


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | δεδομένα | java.lang.Object | Τα σειριοποιημένα δεδομένα. |
|

### getUseSynonymSearch() {#getUseSynonymSearch--}
```
public boolean getUseSynonymSearch()
```


Λαμβάνει τη σημαία χρήσης συνωνύμων στην αναζήτηση. Η προεπιλεγμένη τιμή είναι false.


**Returns:**
boolean - Η σημαία χρήσης συνωνύμων στην αναζήτηση.

### setUseSynonymSearch(boolean value) {#setUseSynonymSearch-boolean-}
```
public void setUseSynonymSearch(boolean value)
```


Ορίζει τη σημαία χρήσης συνωνύμων στην αναζήτηση. Η προεπιλεγμένη τιμή είναι false.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | τιμή | boolean | Η σημαία χρήσης συνωνύμων στην αναζήτηση. |
|

### getUseHomophoneSearch() {#getUseHomophoneSearch--}
```
public boolean getUseHomophoneSearch()
```


Λαμβάνει τη σημαία χρήσης ομόηχων στην αναζήτηση. Η προεπιλεγμένη τιμή είναι false.


**Returns:**
boolean - Η σημαία χρήσης ομόηχων στην αναζήτηση.

### setUseHomophoneSearch(boolean value) {#setUseHomophoneSearch-boolean-}
```
public void setUseHomophoneSearch(boolean value)
```


Ορίζει τη σημαία χρήσης ομόηχων στην αναζήτηση. Η προεπιλεγμένη τιμή είναι false.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | τιμή | boolean | Η σημαία χρήσης ομόηχων στην αναζήτηση. |
|

### getUseWordFormsSearch() {#getUseWordFormsSearch--}
```
public boolean getUseWordFormsSearch()
```


Λαμβάνει τη σημαία χρήσης διαφορετικών μορφών λέξεων στην αναζήτηση. Η προεπιλεγμένη τιμή είναι false.


**Returns:**
boolean - Η σημαία χρήσης διαφορετικών μορφών λέξεων στην αναζήτηση.

### setUseWordFormsSearch(boolean value) {#setUseWordFormsSearch-boolean-}
```
public void setUseWordFormsSearch(boolean value)
```


Ορίζει τη σημαία χρήσης διαφορετικών μορφών λέξεων στην αναζήτηση. Η προεπιλεγμένη τιμή είναι false.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | τιμή | boolean | Η σημαία για χρήση διαφορετικών μορφών λέξεων στην αναζήτηση. |
|

### getRetrieveAttributes() {#getRetrieveAttributes--}
```
public boolean getRetrieveAttributes()
```


Λαμβάνει τη σημαία για ανάκτηση ιδιοτήτων που σχετίζονται με τα ευρεθέντα έγγραφα. Η προεπιλεγμένη τιμή είναι  false .


**Returns:**
boolean - Η σημαία για ανάκτηση ιδιοτήτων που σχετίζονται με τα ευρεθέντα έγγραφα.

### setRetrieveAttributes(boolean value) {#setRetrieveAttributes-boolean-}
```
public void setRetrieveAttributes(boolean value)
```


Ορίζει τη σημαία για ανάκτηση ιδιοτήτων που σχετίζονται με τα ευρεθέντα έγγραφα. Η προεπιλεγμένη τιμή είναι  false .


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | τιμή | boolean | Η σημαία για ανάκτηση ιδιοτήτων που σχετίζονται με τα ευρεθέντα έγγραφα. |
|

### getFuzzySearch() {#getFuzzySearch--}
```
public FuzzySearchOptions getFuzzySearch()
```


Λαμβάνει τις επιλογές ασαφούς αναζήτησης.


**Returns:**
[FuzzySearchOptions](../../com.groupdocs.search.options/fuzzysearchoptions) - The fuzzy search options.

### getSpellingCorrector() {#getSpellingCorrector--}
```
public SpellingCorrectorOptions getSpellingCorrector()
```


Λαμβάνει τις επιλογές διορθωτή ορθογραφίας.


**Returns:**
[SpellingCorrectorOptions](../../com.groupdocs.search.options/spellingcorrectoroptions) - The spelling corrector options.

### getKeyboardLayoutCorrector() {#getKeyboardLayoutCorrector--}
```
public KeyboardLayoutCorrectorOptions getKeyboardLayoutCorrector()
```


Λαμβάνει τις επιλογές διορθωτή διάταξης πληκτρολογίου.


**Returns:**
[KeyboardLayoutCorrectorOptions](../../com.groupdocs.search.options/keyboardlayoutcorrectoroptions) - The keyboard layout corrector options.

### getUseCaseSensitiveSearch() {#getUseCaseSensitiveSearch--}
```
public boolean getUseCaseSensitiveSearch()
```


Λαμβάνει τη σημαία για αναζήτηση με διάκριση πεζών-κεφαλαίων. Η προεπιλεγμένη τιμή είναι  false .


**Returns:**
boolean - Η σημαία για αναζήτηση με διάκριση πεζών-κεφαλαίων.

### setUseCaseSensitiveSearch(boolean value) {#setUseCaseSensitiveSearch-boolean-}
```
public void setUseCaseSensitiveSearch(boolean value)
```


Ορίζει τη σημαία για αναζήτηση με διάκριση πεζών-κεφαλαίων. Η προεπιλεγμένη τιμή είναι  false .


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | τιμή | boolean | Η σημαία για αναζήτηση με διάκριση πεζών-κεφαλαίων. |
|

### getMaxTotalOccurrenceCount() {#getMaxTotalOccurrenceCount--}
```
public int getMaxTotalOccurrenceCount()
```


Λαμβάνει τον μέγιστο συνολικό αριθμό εμφανίσεων όλων των όρων σε ένα ερώτημα αναζήτησης. Η προεπιλεγμένη τιμή είναι  500000 .


**Returns:**
int - Ο μέγιστος συνολικός αριθμός εμφανίσεων.

### setMaxTotalOccurrenceCount(int value) {#setMaxTotalOccurrenceCount-int-}
```
public void setMaxTotalOccurrenceCount(int value)
```


Ορίζει τον μέγιστο συνολικό αριθμό εμφανίσεων όλων των όρων σε ένα ερώτημα αναζήτησης. Η προεπιλεγμένη τιμή είναι  500000 .


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | τιμή | int | Ο μέγιστος συνολικός αριθμός εμφανίσεων. |
|

### getMaxOccurrenceCountPerTerm() {#getMaxOccurrenceCountPerTerm--}
```
public int getMaxOccurrenceCountPerTerm()
```


Λαμβάνει τον μέγιστο αριθμό εμφανίσεων για κάθε όρο σε ένα ερώτημα αναζήτησης. Η προεπιλεγμένη τιμή είναι  100000 .


**Returns:**
int - Ο μέγιστος αριθμός εμφανίσεων για κάθε όρο σε ένα ερώτημα αναζήτησης.

### setMaxOccurrenceCountPerTerm(int value) {#setMaxOccurrenceCountPerTerm-int-}
```
public void setMaxOccurrenceCountPerTerm(int value)
```


Ορίζει τον μέγιστο αριθμό εμφανίσεων για κάθε όρο σε ένα ερώτημα αναζήτησης. Η προεπιλεγμένη τιμή είναι  100000 .


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | τιμή | int | Ο μέγιστος αριθμός εμφανίσεων για κάθε όρο σε ένα ερώτημα αναζήτησης. |
|

### getDateFormats() {#getDateFormats--}
```
public DateFormatCollection getDateFormats()
```


Λαμβάνει τη συλλογή μορφών ημερομηνίας για αναζήτηση εύρους ημερομηνίας. Οι προεπιλεγμένες μορφές ημερομηνίας είναι 'dd.MM.yyyy', 'MM/dd/yyyy' και 'yyyy-MM-dd'.


**Returns:**
[DateFormatCollection](../../com.groupdocs.search.options/dateformatcollection) - The collection of date formats for date range search.


Το παράδειγμα δείχνει πώς να ορίσετε τις μορφές ημερομηνίας για την αναζήτηση.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // Δημιουργία ευρετηρίου στον καθορισμένο φάκελο
index.add(documentsFolder); // Καταχώρηση εγγράφων από τον καθορισμένο φάκελο
SearchOptions options = new SearchOptions();
options.getDateFormats().clear(); // Αφαίρεση προεπιλεγμένων μορφών ημερομηνίας
DateFormatElement[] elements = new DateFormatElement[] {
DateFormatElement.getMonthTwoDigits(),
DateFormatElement.getDayOfMonthTwoDigits(),
DateFormatElement.getYearFourDigits(),
};
// Δημιουργία προτύπου μορφής ημερομηνίας 'MM/dd/yyyy'
com.groupdocs.search.DateFormat dateFormat = new com.groupdocs.search.DateFormat(elements, "/");
options.getDateFormats().addItem(dateFormat);
SearchResult result = index.search(query, options); // Αναζήτηση στο ευρετήριο
 
```
 
````


### isChunkSearch() {#isChunkSearch--}
```
public boolean isChunkSearch()
```


Λαμβάνει τη σημαία για αναζήτηση κατά τμήματα. Η προεπιλεγμένη τιμή είναι  false .


**Returns:**
boolean - Η σημαία για αναζήτηση κατά τμήματα.

### setChunkSearch(boolean value) {#setChunkSearch-boolean-}
```
public void setChunkSearch(boolean value)
```


Ορίζει τη σημαία για αναζήτηση κατά τμήματα. Η προεπιλεγμένη τιμή είναι  false .


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | τιμή | boolean | Η σημαία για αναζήτηση κατά τμήματα. |
|

### getSearchDocumentFilter() {#getSearchDocumentFilter--}
```
public ISearchDocumentFilter getSearchDocumentFilter()
```


Λαμβάνει το φίλτρο εγγράφων αναζήτησης.  SearchDocumentFilter  λειτουργεί με τη λογική ένταξης. Χρησιμοποιήστε την κλάση  SearchDocumentFilter  για τη δημιουργία παραδειγμάτων φίλτρου εγγράφων αναζήτησης. Η προεπιλεγμένη τιμή είναι  null , που σημαίνει ότι θα επιστραφούν όλα τα ευρεθέντα έγγραφα.


**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - The search document filter.


Το παράδειγμα δείχνει πώς να ορίσετε το φίλτρο εγγράφου.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments1\\";
// Δημιουργία ευρετηρίου στον καθορισμένο φάκελο
Index index = new Index(indexFolder);
// Ευρετηρίαση εγγράφων
index.add(documentsFolder);
// Δημιουργία φίλτρου εγγράφων αναζήτησης που παραλείπει έγγραφα με τις επεκτάσεις '.doc', '.docx', '.rtf'
SearchOptions options = new SearchOptions();
ISearchDocumentFilter fileExtensionFilter = SearchDocumentFilter.createFileExtension(".doc", ".docx", ".rtf"); // Δημιουργία φίλτρου επέκτασης αρχείου
ISearchDocumentFilter invertedFilter = SearchDocumentFilter.createNot(fileExtensionFilter); // Αντιστροφή φίλτρου επέκτασης αρχείου
options.setSearchDocumentFilter(invertedFilter);
// Αναζήτηση στο ευρετήριο
SearchResult result = index.search("Einstein", options);
 
```
 
````


### setSearchDocumentFilter(ISearchDocumentFilter value) {#setSearchDocumentFilter-com.groupdocs.search.options.ISearchDocumentFilter-}
```
public void setSearchDocumentFilter(ISearchDocumentFilter value)
```


Ορίζει το φίλτρο εγγράφων αναζήτησης.  SearchDocumentFilter  λειτουργεί με τη λογική ένταξης. Χρησιμοποιήστε την κλάση  SearchDocumentFilter  για τη δημιουργία στιγμιοτύπων φίλτρου εγγράφων αναζήτησης. Η προεπιλεγμένη τιμή είναι  null , που σημαίνει ότι όλα τα ευρεθέντα έγγραφα θα επιστραφούν.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | value | [ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) | Το φίλτρο εγγράφου αναζήτησης. |


Το παράδειγμα δείχνει πώς να ορίσετε το φίλτρο εγγράφου.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments1\\";
// Δημιουργία ευρετηρίου στον καθορισμένο φάκελο
Index index = new Index(indexFolder);
// Ευρετηρίαση εγγράφων
index.add(documentsFolder);
// Δημιουργία φίλτρου εγγράφων αναζήτησης που παραλείπει έγγραφα με τις επεκτάσεις '.doc', '.docx', '.rtf'
SearchOptions options = new SearchOptions();
ISearchDocumentFilter fileExtensionFilter = SearchDocumentFilter.createFileExtension(".doc", ".docx", ".rtf"); // Δημιουργία φίλτρου επέκτασης αρχείου
ISearchDocumentFilter invertedFilter = SearchDocumentFilter.createNot(fileExtensionFilter); // Αντιστροφή φίλτρου επέκτασης αρχείου
options.setSearchDocumentFilter(invertedFilter);
// Αναζήτηση στο ευρετήριο
SearchResult result = index.search("Einstein", options);
 
```
 
````

|

### getCancellation() {#getCancellation--}
```
public Cancellation getCancellation()
```


Λαμβάνει το αντικείμενο ακύρωσης της λειτουργίας. Η προεπιλεγμένη τιμή είναι  null .


**Returns:**
[Cancellation](../../com.groupdocs.search.common/cancellation) - The operation cancellation object.

### setCancellation(Cancellation value) {#setCancellation-com.groupdocs.search.common.Cancellation-}
```
public void setCancellation(Cancellation value)
```


Ορίζει το αντικείμενο ακύρωσης της λειτουργίας. Η προεπιλεγμένη τιμή είναι  null .


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | value | [Cancellation](../../com.groupdocs.search.common/cancellation) | Το αντικείμενο ακύρωσης της λειτουργίας. |
|

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
