---
title: "TableDiscreteFunction"
second_title: "GroupDocs.Search για Java API Reference"
description: "Αναπαριστά τον αλγόριθμο ασαφούς αναζήτησης που περιέχει αντιστοιχίες μεταξύ των μηκών λέξεων και του αριθμού των επιτρεπόμενων λαθών."
type: docs
weight: 40
url: /el/java/com.groupdocs.search.options/tablediscretefunction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.options.FuzzyAlgorithm](../../com.groupdocs.search.options/fuzzyalgorithm)
```
public class TableDiscreteFunction extends FuzzyAlgorithm
```

Αντιπροσωπεύει τον ασαφή αλγόριθμο αναζήτησης που περιέχει αντιστοιχίες μεταξύ του μήκους των λέξεων και του αριθμού των επιτρεπόμενων σφαλμάτων. Αυτός ο αλγόριθμος μπορεί να καθοριστεί με έναν πίνακα τιμών εξόδου ή με μια λειτουργία βήματος.


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
options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(1, new Step(5, 2), new Step(8, 3))); // Δημιουργία του ασαφούς αλγορίθμου αναζήτησης
// Αυτή η λειτουργία καθορίζει το 1 ως μέγιστο αριθμό σφαλμάτων για λέξεις από 1 έως 4 χαρακτήρες.
// Καθορίζει το 2 ως μέγιστο αριθμό σφαλμάτων για λέξεις από 5 έως 7 χαρακτήρες.
// Καθορίζει το 3 ως μέγιστο αριθμό σφαλμάτων για λέξεις από 8 και περισσότερους χαρακτήρες.
SearchResult result = index.search(query, options); // Αναζήτηση στο ευρετήριο
 
```
 
````


## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [TableDiscreteFunction(int offsetOfInputs, int[] tableOfOutputs)](#TableDiscreteFunction-int-int---) | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης  TableDiscreteFunction . |
|
|  | [TableDiscreteFunction(int firstStepLevel, Step[] steps)](#TableDiscreteFunction-int-com.groupdocs.search.options.Step...-) | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης  TableDiscreteFunction . |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getSimilarityLevel(int termLength)](#getSimilarityLevel-int-) | Λαμβάνει ένα επίπεδο ομοιότητας για το καθορισμένο μήκος όρου. |
|
|  | [getMaxMistakeCount(int termLength)](#getMaxMistakeCount-int-) | Λαμβάνει τον μέγιστο επιτρεπόμενο αριθμό λαθών για το καθορισμένο μήκος όρου. |
|
### TableDiscreteFunction(int offsetOfInputs, int[] tableOfOutputs) {#TableDiscreteFunction-int-int---}
```
public TableDiscreteFunction(int offsetOfInputs, int[] tableOfOutputs)
```


Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης  TableDiscreteFunction .


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | offsetOfInputs | int | Η μετατόπιση των δεικτών του πίνακα σε σχέση με τις τιμές εισόδου. |
|
|  | tableOfOutputs | int[] | Ο πίνακας των τιμών εξόδου. |
|

### TableDiscreteFunction(int firstStepLevel, Step[] steps) {#TableDiscreteFunction-int-com.groupdocs.search.options.Step...-}
```
public TableDiscreteFunction(int firstStepLevel, Step[] steps)
```


Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης  TableDiscreteFunction .


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | firstStepLevel | int | Το επίπεδο του πρώτου βήματος της συνάρτησης βήματος. |
|
|  | steps | [Step\[\]](../../com.groupdocs.search.options/step) | Τα επόμενα βήματα της συνάρτησης βήματος. |
|

### getSimilarityLevel(int termLength) {#getSimilarityLevel-int-}
```
public double getSimilarityLevel(int termLength)
```


Λαμβάνει ένα επίπεδο ομοιότητας για το καθορισμένο μήκος όρου.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | termLength | int | Το μήκος του όρου. |
|

**Returns:**
double - Ένα επίπεδο ομοιότητας.

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
int - Ένας μέγιστος επιτρεπόμενος αριθμός λαθών.

