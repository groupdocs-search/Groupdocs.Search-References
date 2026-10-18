---
title: "FuzzySearchOptions"
second_title: "GroupDocs.Search για Java API Reference"
description: "Παρέχει επιλογές για την ασαφή αναζήτηση."
type: docs
weight: 21
url: /el/java/com.groupdocs.search.options/fuzzysearchoptions/
---
**Inheritance:**
java.lang.Object
```
public abstract class FuzzySearchOptions
```

Παρέχει επιλογές για την ασαφή αναζήτηση.


**Learn more**

* [Fuzzy search](../https://docs.groupdocs.com/display/searchjava/Fuzzy+search)
* [Search options](../https://docs.groupdocs.com/display/searchjava/Search+options)

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [FuzzySearchOptions()](#FuzzySearchOptions--) |  |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getEnabled()](#getEnabled--) | Λαμβάνει μια τιμή που υποδεικνύει αν η λειτουργία fuzzy search είναι ενεργοποιημένη. |
|
|  | [setEnabled(boolean value)](#setEnabled-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν η λειτουργία fuzzy search είναι ενεργοποιημένη. |
|
|  | [getFuzzyAlgorithm()](#getFuzzyAlgorithm--) | Ανακτά τον αλγόριθμο fuzzy search. |
|
|  | [setFuzzyAlgorithm(FuzzyAlgorithm value)](#setFuzzyAlgorithm-com.groupdocs.search.options.FuzzyAlgorithm-) | Ορίζει τον αλγόριθμο fuzzy search. |
|
|  | [getOnlyBestResults()](#getOnlyBestResults--) | Λαμβάνει μια τιμή που υποδεικνύει εάν θα επιστραφούν μόνο τα καλύτερα αποτελέσματα. |
|
|  | [setOnlyBestResults(boolean value)](#setOnlyBestResults-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν θα επιστραφούν μόνο τα καλύτερα αποτελέσματα. |
|
|  | [getOnlyBestResultsRange()](#getOnlyBestResultsRange--) | Λαμβάνει τη μέγιστη υπέρβαση του ελάχιστου αριθμού λαθών που εντοπίζονται. |
|
|  | [setOnlyBestResultsRange(byte value)](#setOnlyBestResultsRange-byte-) | Ορίζει τη μέγιστη υπέρβαση του ελάχιστου αριθμού λαθών που εντοπίζονται. |
|
|  | [getConsiderTranspositions()](#getConsiderTranspositions--) | Ανακτά μια τιμή που υποδεικνύει εάν ο αλγόριθμος fuzzy search πρέπει να θεωρεί τη μετατόπιση δύο διαδοχικών χαρακτήρων ως ένα σφάλμα. |
|
|  | [setConsiderTranspositions(boolean value)](#setConsiderTranspositions-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν ο αλγόριθμος fuzzy search πρέπει να θεωρεί τη μετατόπιση δύο διαδοχικών χαρακτήρων ως ένα σφάλμα. |
|
### FuzzySearchOptions() {#FuzzySearchOptions--}
```
public FuzzySearchOptions()
```


### getEnabled() {#getEnabled--}
```
public abstract boolean getEnabled()
```


Ανακτά μια τιμή που υποδεικνύει εάν η λειτουργία fuzzy search είναι ενεργοποιημένη. Η προεπιλεγμένη τιμή είναι  false .


**Returns:**
boolean - Μια τιμή που υποδεικνύει εάν η λειτουργία fuzzy search είναι ενεργοποιημένη.

### setEnabled(boolean value) {#setEnabled-boolean-}
```
public abstract void setEnabled(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει εάν η λειτουργία fuzzy search είναι ενεργοποιημένη. Η προεπιλεγμένη τιμή είναι  false .


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | τιμή | boolean | Μια τιμή που υποδεικνύει εάν η λειτουργία fuzzy search είναι ενεργοποιημένη. |
|

### getFuzzyAlgorithm() {#getFuzzyAlgorithm--}
```
public abstract FuzzyAlgorithm getFuzzyAlgorithm()
```


Ανακτά τον αλγόριθμο fuzzy search. Οι τρέχουσες διαθέσιμες αλγόριθμοι fuzzy search είναι  SimilarityLevel  και  TableDiscreteFunction . Η προεπιλεγμένη τιμή είναι ένα στιγμιότυπο του  SimilarityLevel  με τιμή επιπέδου ομοιότητας  0.5 .


**Returns:**
[FuzzyAlgorithm](../../com.groupdocs.search.options/fuzzyalgorithm) - The fuzzy search algorithm.


Το παράδειγμα δείχνει πώς να ορίσετε τον αλγόριθμο fuzzy search.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // Δημιουργία ευρετηρίου στον καθορισμένο φάκελο
index.add(documentsFolder); // Καταχώρηση εγγράφων από τον καθορισμένο φάκελο
SearchOptions options = new SearchOptions();
options.getFuzzySearch().setEnabled(true); // Ενεργοποίηση της ασαφούς αναζήτησης
options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(1, new Step(5, 2), new Step(8, 3))); // Δημιουργία του ασαφούς αλγορίθμου αναζήτησης
// Αυτή η λειτουργία καθορίζει το 1 ως μέγιστο αριθμό σφαλμάτων για λέξεις από 1 έως 4 χαρακτήρες.
// Καθορίζει το 2 ως μέγιστο αριθμό σφαλμάτων για λέξεις από 5 έως 7 χαρακτήρες.
// Καθορίζει το 3 ως μέγιστο αριθμό σφαλμάτων για λέξεις από 8 και περισσότερους χαρακτήρες.
SearchResult result = index.search(query, options); // Αναζήτηση στο ευρετήριο
 
```
 
````


### setFuzzyAlgorithm(FuzzyAlgorithm value) {#setFuzzyAlgorithm-com.groupdocs.search.options.FuzzyAlgorithm-}
```
public abstract void setFuzzyAlgorithm(FuzzyAlgorithm value)
```


Ορίζει τον αλγόριθμο fuzzy search. Οι τρέχουσες διαθέσιμες αλγόριθμοι fuzzy search είναι  SimilarityLevel  και  TableDiscreteFunction . Η προεπιλεγμένη τιμή είναι ένα στιγμιότυπο του  SimilarityLevel  με τιμή επιπέδου ομοιότητας  0.5 .


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | value | [FuzzyAlgorithm](../../com.groupdocs.search.options/fuzzyalgorithm) | Ο αλγόριθμος fuzzy search. |


Το παράδειγμα δείχνει πώς να ορίσετε τον αλγόριθμο fuzzy search.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // Δημιουργία ευρετηρίου στον καθορισμένο φάκελο
index.add(documentsFolder); // Καταχώρηση εγγράφων από τον καθορισμένο φάκελο
SearchOptions options = new SearchOptions();
options.getFuzzySearch().setEnabled(true); // Ενεργοποίηση της ασαφούς αναζήτησης
options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(1, new Step(5, 2), new Step(8, 3))); // Δημιουργία του ασαφούς αλγορίθμου αναζήτησης
// Αυτή η λειτουργία καθορίζει το 1 ως μέγιστο αριθμό σφαλμάτων για λέξεις από 1 έως 4 χαρακτήρες.
// Καθορίζει το 2 ως μέγιστο αριθμό σφαλμάτων για λέξεις από 5 έως 7 χαρακτήρες.
// Καθορίζει το 3 ως μέγιστο αριθμό σφαλμάτων για λέξεις από 8 και περισσότερους χαρακτήρες.
SearchResult result = index.search(query, options); // Αναζήτηση στο ευρετήριο
 
```
 
````

|

### getOnlyBestResults() {#getOnlyBestResults--}
```
public abstract boolean getOnlyBestResults()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν θα επιστραφούν μόνο τα καλύτερα αποτελέσματα. Η προεπιλεγμένη τιμή είναι  false .


**Returns:**
boolean -  true  εάν θα επιστραφούν μόνο τα καλύτερα αποτελέσματα· διαφορετικά  false .

### setOnlyBestResults(boolean value) {#setOnlyBestResults-boolean-}
```
public abstract void setOnlyBestResults(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει εάν θα επιστραφούν μόνο τα καλύτερα αποτελέσματα. Η προεπιλεγμένη τιμή είναι  false .


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | τιμή | boolean | true  εάν θα επιστραφούν μόνο τα καλύτερα αποτελέσματα· διαφορετικά  false . |
|

### getOnlyBestResultsRange() {#getOnlyBestResultsRange--}
```
public abstract byte getOnlyBestResultsRange()
```


Λαμβάνει τη μέγιστη υπέρβαση του ελάχιστου αριθμού λαθών που βρέθηκαν. Η προεπιλεγμένη τιμή είναι  0 .


**Returns:**
byte - Η μέγιστη υπέρβαση του ελάχιστου αριθμού λαθών που βρέθηκαν.

### setOnlyBestResultsRange(byte value) {#setOnlyBestResultsRange-byte-}
```
public abstract void setOnlyBestResultsRange(byte value)
```


Ορίζει τη μέγιστη υπέρβαση του ελάχιστου αριθμού λαθών που βρέθηκαν. Η προεπιλεγμένη τιμή είναι  0 .


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | τιμή | byte | Η μέγιστη υπέρβαση του ελάχιστου αριθμού λαθών που βρέθηκαν. |
|

### getConsiderTranspositions() {#getConsiderTranspositions--}
```
public abstract boolean getConsiderTranspositions()
```


Ανακτά μια τιμή που υποδεικνύει εάν ο αλγόριθμος fuzzy search πρέπει να θεωρεί τη μετατόπιση δύο διαδοχικών χαρακτήρων ως ένα σφάλμα. Η προεπιλεγμένη τιμή είναι  true .


**Returns:**
boolean -  true  εάν ο αλγόριθμος fuzzy search θεωρεί τις μετατοπίσεις· διαφορετικά  false .

### setConsiderTranspositions(boolean value) {#setConsiderTranspositions-boolean-}
```
public abstract void setConsiderTranspositions(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει εάν ο αλγόριθμος fuzzy search πρέπει να θεωρεί τη μετατόπιση δύο διαδοχικών χαρακτήρων ως ένα σφάλμα. Η προεπιλεγμένη τιμή είναι  true .


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | τιμή | boolean | :  true  εάν ο αλγόριθμος fuzzy search θεωρεί τις μετατοπίσεις· διαφορετικά  false . |
|

