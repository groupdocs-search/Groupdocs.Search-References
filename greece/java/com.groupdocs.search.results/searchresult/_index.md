---
title: "SearchResult"
second_title: "GroupDocs.Search για Java API Reference"
description: "Αντιπροσωπεύει ένα αποτέλεσμα αναζήτησης που ταιριάζει με ένα ερώτημα αναζήτησης."
type: docs
weight: 19
url: /el/java/com.groupdocs.search.results/searchresult/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public abstract class SearchResult implements Iterable<FoundDocument>
```

Αντιπροσωπεύει ένα αποτέλεσμα αναζήτησης που ταιριάζει με ένα ερώτημα αναζήτησης.


**Learn more**

* [Searching](../https://docs.groupdocs.com/display/searchjava/Searching)
* [Search results](../https://docs.groupdocs.com/display/searchjava/Search+results)


Το παράδειγμα δείχνει μια τυπική χρήση της κλάσης.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentFolder = "c:\\MyDocuments\\";
// Δημιουργία ενός δείκτη
Index index = new Index(indexFolder);
// Καταχώριση εγγράφων από τον καθορισμένο φάκελο
index.add(documentFolder);
// Ρύθμιση επιλογών αναζήτησης
SearchOptions options = new SearchOptions();
options.getFuzzySearch().setEnabled(true); // Ενεργοποίηση της ασαφούς αναζήτησης
options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(3)); // Ρύθμιση του μέγιστου αριθμού διαφορών σε 3
// Αναζήτηση εγγράφων που περιέχουν τη λέξη 'Einstein' ή τη φράση 'Theory of Relativity'
SearchResult result = index.search("Einstein OR \"Theory of Relativity\"", options);
// Εκτύπωση του αποτελέσματος
System.out.println("Έγγραφα: " + result.getDocumentCount());
System.out.println("Συνολικές εμφανίσεις: " + result.getOccurrenceCount());
for (int i = 0; i < result.getDocumentCount(); i++) {
FoundDocument document = result.getFoundDocument(i);
System.out.println("\tΈγγραφο: " + document.getDocumentInfo().getFilePath());
System.out.println("\tΕμφανίσεις: " + document.getOccurrenceCount());
for (int j = 0; j < document.getFoundFields().length; j++) {
FoundDocumentField field = document.getFoundFields()[j];
System.out.println("\t\tΠεδίο: " + field.getFieldName());
System.out.println("\t\tΕμφανίσεις: " + document.getOccurrenceCount());
// Εκτύπωση ευρεθέντων όρων
if (field.getTerms() != null) {
for (int k = 0; k < field.getTerms().length; k++) {
System.out.println("\t\t\t" + field.getTerms()[k] + " - " + field.getTermsOccurrences()[k]);
}
}
// Εκτύπωση ευρεθέντων φράσεων
if (field.getTermSequences() != null) {
for (int k = 0; k < field.getTermSequences().length; k++) {
String[] terms = field.getTermSequences()[k];
String sequence = "";
for (int m = 0; m < terms.length; m++) {
sequence += terms[m] + " ";
}
System.out.println("\t\t\t" + sequence + " - " + field.getTermSequencesOccurrences()[k]);
}
}
}
}
 
```
 
````


## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [SearchResult()](#SearchResult--) |  |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getDocumentCount()](#getDocumentCount--) | Λαμβάνει τον αριθμό των εγγράφων που βρέθηκαν. |
|
|  | [getOccurrenceCount()](#getOccurrenceCount--) | Λαμβάνει τον συνολικό αριθμό των εμφανίσεων που βρέθηκαν. |
|
|  | [getTruncated()](#getTruncated--) | Λαμβάνει μια τιμή που υποδεικνύει ότι το αποτέλεσμα είναι περικομμένο. |
|
|  | [getWarnings()](#getWarnings--) | Λαμβάνει μια προειδοποίηση που περιγράφει το αποτέλεσμα. |
|
|  | [getNextChunkSearchToken()](#getNextChunkSearchToken--) | Λαμβάνει ένα διακριτικό αναζήτησης τμήματος για την αναζήτηση του επόμενου τμήματος. |
|
|  | [getStartTime()](#getStartTime--) | Λαμβάνει την ώρα έναρξης της αναζήτησης. |
|
|  | [getEndTime()](#getEndTime--) | Λαμβάνει την ώρα λήξης της αναζήτησης. |
|
|  | [getSearchDuration()](#getSearchDuration--) | Λαμβάνει τη διάρκεια της αναζήτησης σε δευτερόλεπτα. |
|
|  | [getFoundDocument(int index)](#getFoundDocument-int-) | Λαμβάνει το έγγραφο που βρέθηκε με βάση το δείκτη. |
|
|  | [iterator()](#iterator--) | Επιστρέφει έναν επαναλήπτη που διατρέχει τη συλλογή των εγγράφων που βρέθηκαν. |
|
### SearchResult() {#SearchResult--}
```
public SearchResult()
```


### getDocumentCount() {#getDocumentCount--}
```
public abstract int getDocumentCount()
```


Λαμβάνει τον αριθμό των εγγράφων που βρέθηκαν.


**Returns:**
int - Ο αριθμός των εγγράφων που βρέθηκαν.

### getOccurrenceCount() {#getOccurrenceCount--}
```
public abstract int getOccurrenceCount()
```


Λαμβάνει τον συνολικό αριθμό των εμφανίσεων που βρέθηκαν.


**Returns:**
int - Ο συνολικός αριθμός των εμφανίσεων που βρέθηκαν.

### getTruncated() {#getTruncated--}
```
public abstract boolean getTruncated()
```


Λαμβάνει μια τιμή που υποδεικνύει ότι το αποτέλεσμα είναι περικομμένο.


**Returns:**
boolean - Μια τιμή που υποδεικνύει ότι το αποτέλεσμα είναι περικομμένο.

### getWarnings() {#getWarnings--}
```
public abstract String getWarnings()
```


Λαμβάνει μια προειδοποίηση που περιγράφει το αποτέλεσμα.


**Returns:**
java.lang.String - Μια προειδοποίηση που περιγράφει το αποτέλεσμα.

### getNextChunkSearchToken() {#getNextChunkSearchToken--}
```
public abstract ChunkSearchToken getNextChunkSearchToken()
```


Λαμβάνει ένα διακριτικό αναζήτησης τμήματος για την αναζήτηση του επόμενου τμήματος.


**Returns:**
[ChunkSearchToken](../../com.groupdocs.search.common/chunksearchtoken) - A chunk search token for searching the next chunk.

### getStartTime() {#getStartTime--}
```
public abstract Date getStartTime()
```


Λαμβάνει την ώρα έναρξης της αναζήτησης.


**Returns:**
java.util.Date - Η ώρα έναρξης της αναζήτησης.

### getEndTime() {#getEndTime--}
```
public abstract Date getEndTime()
```


Λαμβάνει την ώρα λήξης της αναζήτησης.


**Returns:**
java.util.Date - Η ώρα λήξης της αναζήτησης.

### getSearchDuration() {#getSearchDuration--}
```
public abstract double getSearchDuration()
```


Λαμβάνει τη διάρκεια της αναζήτησης σε δευτερόλεπτα.


**Returns:**
double - Η διάρκεια της αναζήτησης σε δευτερόλεπτα.

### getFoundDocument(int index) {#getFoundDocument-int-}
```
public abstract FoundDocument getFoundDocument(int index)
```


Λαμβάνει το έγγραφο που βρέθηκε με βάση το δείκτη.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | ευρετήριο | int | Ο δείκτης ενός εγγράφου που βρέθηκε. |
|

**Returns:**
[FoundDocument](../../com.groupdocs.search.results/founddocument) - The found document.

### iterator() {#iterator--}
```
public abstract Iterator<FoundDocument> iterator()
```


Επιστρέφει έναν επαναλήπτη που διατρέχει τη συλλογή των εγγράφων που βρέθηκαν.


**Returns:**
java.util.Iterator<com.groupdocs.search.results.FoundDocument> - Ένας επαναλήπτης που μπορεί να χρησιμοποιηθεί για την επανάληψη μέσω της συλλογής των ευρεθέντων εγγράφων.

