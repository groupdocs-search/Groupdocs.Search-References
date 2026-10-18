---
title: "FoundDocument"
second_title: "GroupDocs.Search για Java API Reference"
description: "Αντιπροσωπεύει ένα βρεθέν έγγραφο."
type: docs
weight: 14
url: /el/java/com.groupdocs.search.results/founddocument/
---
**Inheritance:**
java.lang.Object
```
public abstract class FoundDocument
```

Αντιπροσωπεύει ένα βρεθέν έγγραφο.


**Learn more**

* [Search results](../https://docs.groupdocs.com/display/searchjava/Search+results)

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [FoundDocument()](#FoundDocument--) |  |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getDocumentInfo()](#getDocumentInfo--) | Λαμβάνει τις πληροφορίες του εγγράφου. |
|
|  | [getRelevance()](#getRelevance--) | Λαμβάνει τη συνάφεια του αποτελέσματος αναζήτησης. |
|
|  | [getOccurrenceCount()](#getOccurrenceCount--) | Λαμβάνει τον αριθμό των εμφανίσεων που βρέθηκαν. |
|
|  | [getFoundFields()](#getFoundFields--) | Λαμβάνει τα πεδία του εγγράφου που βρέθηκαν. |
|
|  | [getTerms()](#getTerms--) | Λαμβάνει τους όρους που βρέθηκαν. |
|
|  | [getTermSequences()](#getTermSequences--) | Λαμβάνει τις ακολουθίες όρων που βρέθηκαν. |
|
|  | [getAttributes()](#getAttributes--) | Λαμβάνει τα χαρακτηριστικά που σχετίζονται με το ευρεθέν έγγραφο. |
|
|  | [toString()](#toString--) | Επιστρέφει την αναπαράσταση ως συμβολοσειρά του ευρεθέντος εγγράφου. |
|
|  | [serialize()](#serialize--) | Σειριοποιεί την τρέχουσα παρουσία σε έναν πίνακα byte. |
|
|  | [deserialize(byte[] array)](#deserialize-byte---) | Αποσειριοποιεί μια παρουσία από έναν πίνακα byte. |
|
### FoundDocument() {#FoundDocument--}
```
public FoundDocument()
```


### getDocumentInfo() {#getDocumentInfo--}
```
public abstract DocumentInfo getDocumentInfo()
```


Λαμβάνει τις πληροφορίες του εγγράφου.


**Returns:**
[DocumentInfo](../../com.groupdocs.search.results/documentinfo) - The document info.

### getRelevance() {#getRelevance--}
```
public abstract double getRelevance()
```


Λαμβάνει τη συνάφεια του αποτελέσματος αναζήτησης.


**Returns:**
double - Η συνάφεια του αποτελέσματος αναζήτησης.

### getOccurrenceCount() {#getOccurrenceCount--}
```
public abstract int getOccurrenceCount()
```


Λαμβάνει τον αριθμό των εμφανίσεων που βρέθηκαν.


**Returns:**
int - Ο αριθμός των εμφανίσεων που βρέθηκαν.

### getFoundFields() {#getFoundFields--}
```
public abstract FoundDocumentField[] getFoundFields()
```


Λαμβάνει τα πεδία του εγγράφου που βρέθηκαν.


**Returns:**
com.groupdocs.search.results.FoundDocumentField[] - Τα πεδία του εγγράφου που βρέθηκαν.

### getTerms() {#getTerms--}
```
public abstract String[] getTerms()
```


Λαμβάνει τους όρους που βρέθηκαν. Η τιμή αξιολογείται κάθε φορά που προσπερνάται η ιδιότητα.


**Returns:**
java.lang.String[] - Οι όροι που βρέθηκαν.

### getTermSequences() {#getTermSequences--}
```
public abstract String[][] getTermSequences()
```


Λαμβάνει τις ακολουθίες όρων που βρέθηκαν.


**Returns:**
java.lang.String[][] - Οι ακολουθίες όρων που βρέθηκαν.

### getAttributes() {#getAttributes--}
```
public abstract String[] getAttributes()
```


Λαμβάνει τα χαρακτηριστικά που σχετίζονται με το ευρεθέν έγγραφο. Η αντίστοιχη επιλογή πρέπει να ενεργοποιηθεί στις επιλογές αναζήτησης για την ανάκτηση των χαρακτηριστικών.


**Returns:**
java.lang.String[] - Τα χαρακτηριστικά που σχετίζονται με το ευρεθέν έγγραφο.

### toString() {#toString--}
```
public abstract String toString()
```


Επιστρέφει την αναπαράσταση ως συμβολοσειρά του ευρεθέντος εγγράφου.


**Returns:**
java.lang.String - Μια συμβολοσειρά που αντιπροσωπεύει το ευρεθέν έγγραφο.

### serialize() {#serialize--}
```
public abstract byte[] serialize()
```


Σειριοποιεί την τρέχουσα παρουσία σε έναν πίνακα byte.


**Returns:**
byte[] - Ένας πίνακας byte που αντιπροσωπεύει την τρέχουσα παρουσία.

### deserialize(byte[] array) {#deserialize-byte---}
```
public static FoundDocument deserialize(byte[] array)
```


Αποσειριοποιεί μια παρουσία από έναν πίνακα byte.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | πίνακας | byte[] | Ένας πίνακας byte για αποσειριοποίηση. |
|

**Returns:**
[FoundDocument](../../com.groupdocs.search.results/founddocument) - An instance deserialized from a byte array.

