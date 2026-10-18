---
title: "SimilarityLevel"
second_title: "GroupDocs.Search για Java API Reference"
description: "Αναπαριστά έναν αλγόριθμο ασαφούς αναζήτησης που καθορίζει το επίπεδο ομοιότητας."
type: docs
weight: 35
url: /el/java/com.groupdocs.search.options/similaritylevel/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.options.FuzzyAlgorithm](../../com.groupdocs.search.options/fuzzyalgorithm)
```
public class SimilarityLevel extends FuzzyAlgorithm
```

Αντιπροσωπεύει έναν αλγόριθμο της ασαφούς αναζήτησης που καθορίζει το επίπεδο ομοιότητας. Ο αλγόριθμος επιπέδου ομοιότητας υπολογίζει τον μέγιστο αριθμό λαθών για μια λέξη ως αντίστροφα ανάλογο του μήκους της λέξης.


**Learn more**

* [Fuzzy search](../https://docs.groupdocs.com/display/searchjava/Fuzzy+search)


Το παράδειγμα δείχνει μια τυπική χρήση της κλάσης.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // Δημιουργία ευρετηρίου στον καθορισμένο φάκελο
index.add(documentsFolder); // Καταχώρηση εγγράφων από τον καθορισμένο φάκελο
SearchOptions options = new SearchOptions();
options.getFuzzySearch().setEnabled(true); // Ενεργοποίηση της ασαφούς αναζήτησης
options.getFuzzySearch().setFuzzyAlgorithm(new SimilarityLevel(0.8)); // Δημιουργία του αλγορίθμου ασαφούς αναζήτησης
// Αυτή η συνάρτηση ορίζει το 0 ως μέγιστο αριθμό λαθών για λέξεις από 1 έως 4 χαρακτήρες.
// Ορίζει το 1 ως μέγιστο αριθμό λαθών για λέξεις από 5 έως 9 χαρακτήρες.
// Ορίζει το 2 ως μέγιστο αριθμό λαθών για λέξεις από 10 έως 14 χαρακτήρες. Και ούτω καθεξής.
SearchResult result = index.search(query, options); // Αναζήτηση στο ευρετήριο
 
```
 
````


## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [SimilarityLevel(double value)](#SimilarityLevel-double-) | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης  SimilarityLevel . |
|
|  | [SimilarityLevel(Object data)](#SimilarityLevel-java.lang.Object-) | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης  SimilarityLevel . |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getSimilarityLevel(int termLength)](#getSimilarityLevel-int-) | Λαμβάνει την τιμή του επιπέδου ομοιότητας για το καθορισμένο μήκος όρου. |
|
|  | [getMaxMistakeCount(int termLength)](#getMaxMistakeCount-int-) | Λαμβάνει τον μέγιστο επιτρεπόμενο αριθμό λαθών για το καθορισμένο μήκος όρου. |
|
### SimilarityLevel(double value) {#SimilarityLevel-double-}
```
public SimilarityLevel(double value)
```


Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης  SimilarityLevel .


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | τιμή | double | Η τιμή του επιπέδου ομοιότητας. |
|

### SimilarityLevel(Object data) {#SimilarityLevel-java.lang.Object-}
```
public SimilarityLevel(Object data)
```


Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης  SimilarityLevel .


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | δεδομένα | java.lang.Object | Τα σειριοποιημένα δεδομένα. |
|

### getSimilarityLevel(int termLength) {#getSimilarityLevel-int-}
```
public double getSimilarityLevel(int termLength)
```


Λαμβάνει την τιμή του επιπέδου ομοιότητας για το καθορισμένο μήκος όρου.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | termLength | int | Το μήκος του όρου. |
|

**Returns:**
double - Η τιμή του επιπέδου ομοιότητας.

### getMaxMistakeCount(int termLength) {#getMaxMistakeCount-int-}
```
public int getMaxMistakeCount(int termLength)
```


Λαμβάνει τον μέγιστο επιτρεπόμενο αριθμό λαθών για το καθορισμένο μήκος όρου.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | termLength | int | Το μήκος του όρου. |
|

**Returns:**
int - Μέγιστος επιτρεπτός αριθμός λαθών.

