---
title: "FoundDocumentField"
second_title: "GroupDocs.Search για Java API Reference"
description: "Αντιπροσωπεύει ένα πεδίο βρεθέντος εγγράφου."
type: docs
weight: 15
url: /el/java/com.groupdocs.search.results/founddocumentfield/
---
**Inheritance:**
java.lang.Object
```
public abstract class FoundDocumentField
```

Αντιπροσωπεύει ένα πεδίο βρεθέντος εγγράφου.


**Learn more**

* [Search results](../https://docs.groupdocs.com/display/searchjava/Search+results)

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [FoundDocumentField()](#FoundDocumentField--) |  |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getFieldName()](#getFieldName--) | Λαμβάνει το όνομα του πεδίου. |
|
|  | [getOccurrenceCount()](#getOccurrenceCount--) | Λαμβάνει τον αριθμό των εμφανίσεων που βρέθηκαν. |
|
|  | [getTerms()](#getTerms--) | Λαμβάνει τους όρους που βρέθηκαν. |
|
|  | [getTermsOccurrences()](#getTermsOccurrences--) | Λαμβάνει τις εμφανίσεις των ευρεθέντων όρων. |
|
|  | [getTermSequences()](#getTermSequences--) | Λαμβάνει τις ακολουθίες όρων που βρέθηκαν. |
|
|  | [getTermSequencesOccurrences()](#getTermSequencesOccurrences--) | Λαμβάνει τις εμφανίσεις των ευρεθέντων ακολουθιών όρων. |
|
|  | [toString()](#toString--) | Επιστρέφει την αναπαράσταση ως συμβολοσειρά του ευρεθέντος πεδίου εγγράφου. |
|
|  | [serialize()](#serialize--) | Σειριοποιεί την τρέχουσα παρουσία σε έναν πίνακα byte. |
|
|  | [deserialize(byte[] array)](#deserialize-byte---) | Αποσειριοποιεί μια παρουσία από έναν πίνακα byte. |
|
### FoundDocumentField() {#FoundDocumentField--}
```
public FoundDocumentField()
```


### getFieldName() {#getFieldName--}
```
public abstract String getFieldName()
```


Λαμβάνει το όνομα του πεδίου.


**Returns:**
java.lang.String - Το όνομα του πεδίου.

### getOccurrenceCount() {#getOccurrenceCount--}
```
public abstract int getOccurrenceCount()
```


Λαμβάνει τον αριθμό των εμφανίσεων που βρέθηκαν.


**Returns:**
int - Ο αριθμός των εμφανίσεων που βρέθηκαν.

### getTerms() {#getTerms--}
```
public abstract String[] getTerms()
```


Λαμβάνει τους όρους που βρέθηκαν.


**Returns:**
java.lang.String[] - Οι όροι που βρέθηκαν.

### getTermsOccurrences() {#getTermsOccurrences--}
```
public abstract int[] getTermsOccurrences()
```


Λαμβάνει τις εμφανίσεις των ευρεθέντων όρων.


**Returns:**
int[] - Οι εμφανίσεις των ευρεθέντων όρων.

### getTermSequences() {#getTermSequences--}
```
public abstract String[][] getTermSequences()
```


Λαμβάνει τις ακολουθίες όρων που βρέθηκαν.


**Returns:**
java.lang.String[][] - Οι ακολουθίες όρων που βρέθηκαν.

### getTermSequencesOccurrences() {#getTermSequencesOccurrences--}
```
public abstract int[] getTermSequencesOccurrences()
```


Λαμβάνει τις εμφανίσεις των ευρεθέντων ακολουθιών όρων.


**Returns:**
int[] - Οι εμφανίσεις των ευρεθέντων ακολουθιών όρων.

### toString() {#toString--}
```
public abstract String toString()
```


Επιστρέφει την αναπαράσταση ως συμβολοσειρά του ευρεθέντος πεδίου εγγράφου.


**Returns:**
java.lang.String - Μια συμβολοσειρά που αντιπροσωπεύει το ευρεθέν πεδίο εγγράφου.

### serialize() {#serialize--}
```
public abstract byte[] serialize()
```


Σειριοποιεί την τρέχουσα παρουσία σε έναν πίνακα byte.


**Returns:**
byte[] - Ένας πίνακας byte που αντιπροσωπεύει την τρέχουσα παρουσία.

### deserialize(byte[] array) {#deserialize-byte---}
```
public static FoundDocumentField deserialize(byte[] array)
```


Αποσειριοποιεί μια παρουσία από έναν πίνακα byte.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | πίνακας | byte[] | Ένας πίνακας byte για αποσειριοποίηση. |
|

**Returns:**
[FoundDocumentField](../../com.groupdocs.search.results/founddocumentfield) - An instance deserialized from a byte array.

