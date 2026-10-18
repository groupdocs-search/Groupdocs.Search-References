---
title: "MetadataIndexingOptions"
second_title: "GroupDocs.Search για Java API Reference"
description: "Παρέχει επιλογές για την ευρετηρίαση πεδίων μεταδεδομένων."
type: docs
weight: 29
url: /el/java/com.groupdocs.search.options/metadataindexingoptions/
---
**Inheritance:**
java.lang.Object
```
public abstract class MetadataIndexingOptions
```

Παρέχει επιλογές για την ευρετηρίαση πεδίων μεταδεδομένων.


**Learn more**

* [Indexing options](../https://docs.groupdocs.com/display/searchjava/Indexing+options)
* MetadataIndexingOptions are used when retrieving document text from an index: [Getting indexed documents](../https://docs.groupdocs.com/display/searchjava/Getting+indexed+documents)
* MetadataIndexingOptions are used when highlighting search results: [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [MetadataIndexingOptions()](#MetadataIndexingOptions--) |  |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getIndexingEmptyValues()](#getIndexingEmptyValues--) | Λαμβάνει μια τιμή που υποδεικνύει εάν θα ευρετηριαστούν κενές τιμές πεδίου ή όχι. |
|
|  | [setIndexingEmptyValues(boolean value)](#setIndexingEmptyValues-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν θα ευρετηριαστούν κενές τιμές πεδίου ή όχι. |
|
|  | [getIndexingEmptyNames()](#getIndexingEmptyNames--) | Λαμβάνει μια τιμή που υποδεικνύει εάν θα ευρετηριαστούν κενά ονόματα πεδίου ή όχι. |
|
|  | [setIndexingEmptyNames(boolean value)](#setIndexingEmptyNames-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν θα ευρετηριαστούν κενά ονόματα πεδίου ή όχι. |
|
|  | [getDefaultFieldName()](#getDefaultFieldName--) | Λαμβάνει το προεπιλεγμένο όνομα πεδίου που χρησιμοποιείται για την ευρετηρίαση κενών ονομάτων πεδίου. |
|
|  | [setDefaultFieldName(String value)](#setDefaultFieldName-java.lang.String-) | Ορίζει το προεπιλεγμένο όνομα πεδίου που χρησιμοποιείται για την ευρετηρίαση κενών ονομάτων πεδίου. |
|
|  | [getSeparatorInCompoundName()](#getSeparatorInCompoundName--) | Λαμβάνει το διαχωριστικό στο σύνθετο όνομα ενός πεδίου. |
|
|  | [setSeparatorInCompoundName(String value)](#setSeparatorInCompoundName-java.lang.String-) | Ορίζει το διαχωριστικό στο σύνθετο όνομα ενός πεδίου. |
|
|  | [getMaxBytesToIndexField()](#getMaxBytesToIndexField--) | Λαμβάνει το μέγιστο αριθμό τιμών σε έναν πίνακα τύπου byte για την ευρετηρίαση του πεδίου. |
|
|  | [setMaxBytesToIndexField(int value)](#setMaxBytesToIndexField-int-) | Ορίζει το μέγιστο αριθμό τιμών σε έναν πίνακα τύπου byte για την ευρετηρίαση του πεδίου. |
|
|  | [getMaxIntsToIndexField()](#getMaxIntsToIndexField--) | Λαμβάνει το μέγιστο αριθμό τιμών σε έναν πίνακα τύπου int για την ευρετηρίαση του πεδίου. |
|
|  | [setMaxIntsToIndexField(int value)](#setMaxIntsToIndexField-int-) | Ορίζει το μέγιστο αριθμό τιμών σε έναν πίνακα τύπου int για την ευρετηρίαση του πεδίου. |
|
|  | [getMaxLongsToIndexField()](#getMaxLongsToIndexField--) | Λαμβάνει το μέγιστο αριθμό τιμών σε έναν πίνακα τύπου long για την ευρετηρίαση του πεδίου. |
|
|  | [setMaxLongsToIndexField(int value)](#setMaxLongsToIndexField-int-) | Ορίζει το μέγιστο αριθμό τιμών σε έναν πίνακα τύπου long για την ευρετηρίαση του πεδίου. |
|
|  | [getMaxDoublesToIndexField()](#getMaxDoublesToIndexField--) | Λαμβάνει το μέγιστο αριθμό τιμών σε έναν πίνακα τύπου double για την ευρετηρίαση του πεδίου. |
|
|  | [setMaxDoublesToIndexField(int value)](#setMaxDoublesToIndexField-int-) | Ορίζει το μέγιστο αριθμό τιμών σε έναν πίνακα τύπου double για την ευρετηρίαση του πεδίου. |
|
|  | [getSeparatorBetweenValues()](#getSeparatorBetweenValues--) | Λαμβάνει το διαχωριστικό μεταξύ τιμών σε ένα πεδίο τύπου array. |
|
|  | [setSeparatorBetweenValues(String value)](#setSeparatorBetweenValues-java.lang.String-) | Ορίζει το διαχωριστικό μεταξύ τιμών σε ένα πεδίο τύπου array. |
|
### MetadataIndexingOptions() {#MetadataIndexingOptions--}
```
public MetadataIndexingOptions()
```


### getIndexingEmptyValues() {#getIndexingEmptyValues--}
```
public abstract boolean getIndexingEmptyValues()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν θα ευρετηριαστούν κενές τιμές πεδίου ή όχι. Η προεπιλεγμένη τιμή είναι  true .


**Returns:**
boolean - Μια τιμή που υποδεικνύει εάν θα ευρετηριαστούν κενές τιμές πεδίου ή όχι.

### setIndexingEmptyValues(boolean value) {#setIndexingEmptyValues-boolean-}
```
public abstract void setIndexingEmptyValues(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει εάν θα γίνει ευρετηρίαση κενών τιμών πεδίου ή όχι. Η προεπιλεγμένη τιμή είναι  true .


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | τιμή | boolean | Μια τιμή που υποδεικνύει εάν θα γίνει ευρετηρίαση κενών τιμών πεδίου ή όχι. |
|

### getIndexingEmptyNames() {#getIndexingEmptyNames--}
```
public abstract boolean getIndexingEmptyNames()
```


Αποκτά μια τιμή που υποδεικνύει εάν θα γίνει ευρετηρίαση κενών ονομάτων πεδίου ή όχι. Η προεπιλεγμένη τιμή είναι  true .


**Returns:**
boolean - Μια τιμή που υποδεικνύει εάν θα γίνει ευρετηρίαση κενών ονομάτων πεδίου ή όχι.

### setIndexingEmptyNames(boolean value) {#setIndexingEmptyNames-boolean-}
```
public abstract void setIndexingEmptyNames(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει εάν θα γίνει ευρετηρίαση κενών ονομάτων πεδίου ή όχι. Η προεπιλεγμένη τιμή είναι  true .


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | τιμή | boolean | Μια τιμή που υποδεικνύει εάν θα γίνει ευρετηρίαση κενών ονομάτων πεδίου ή όχι. |
|

### getDefaultFieldName() {#getDefaultFieldName--}
```
public abstract String getDefaultFieldName()
```


Αποκτά το προεπιλεγμένο όνομα πεδίου που χρησιμοποιείται για την ευρετηρίαση κενών ονομάτων πεδίου. Η προεπιλεγμένη τιμή είναι  "unknown" .


**Returns:**
java.lang.String - Το προεπιλεγμένο όνομα πεδίου που χρησιμοποιείται για την ευρετηρίαση κενών ονομάτων πεδίου.

### setDefaultFieldName(String value) {#setDefaultFieldName-java.lang.String-}
```
public abstract void setDefaultFieldName(String value)
```


Ορίζει το προεπιλεγμένο όνομα πεδίου που χρησιμοποιείται για την ευρετηρίαση κενών ονομάτων πεδίου. Η προεπιλεγμένη τιμή είναι  "unknown" .


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | τιμή | java.lang.String | Το προεπιλεγμένο όνομα πεδίου που χρησιμοποιείται για την ευρετηρίαση κενών ονομάτων πεδίου. |
|

### getSeparatorInCompoundName() {#getSeparatorInCompoundName--}
```
public abstract String getSeparatorInCompoundName()
```


Αποκτά το διαχωριστικό στο σύνθετο όνομα ενός πεδίου. Η προεπιλεγμένη τιμή είναι  "." .


**Returns:**
java.lang.String - Το διαχωριστικό στο σύνθετο όνομα ενός πεδίου.

### setSeparatorInCompoundName(String value) {#setSeparatorInCompoundName-java.lang.String-}
```
public abstract void setSeparatorInCompoundName(String value)
```


Ορίζει το διαχωριστικό στο σύνθετο όνομα ενός πεδίου. Η προεπιλεγμένη τιμή είναι  "." .


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | τιμή | java.lang.String | Το διαχωριστικό στο σύνθετο όνομα ενός πεδίου. |
|

### getMaxBytesToIndexField() {#getMaxBytesToIndexField--}
```
public abstract int getMaxBytesToIndexField()
```


Αποκτά τον μέγιστο αριθμό τιμών σε έναν πίνακα τύπου byte για την ευρετηρίαση του πεδίου. Η προεπιλεγμένη τιμή είναι  Integer.MAX_VALUE .


**Returns:**
int - Ο μέγιστος αριθμός τιμών σε έναν πίνακα τύπου byte για την ευρετηρίαση του πεδίου.

### setMaxBytesToIndexField(int value) {#setMaxBytesToIndexField-int-}
```
public abstract void setMaxBytesToIndexField(int value)
```


Ορίζει τον μέγιστο αριθμό τιμών σε έναν πίνακα τύπου byte για την ευρετηρίαση του πεδίου. Η προεπιλεγμένη τιμή είναι  Integer.MAX_VALUE .


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | τιμή | int | Ο μέγιστος αριθμός τιμών σε έναν πίνακα τύπου byte για την ευρετηρίαση του πεδίου. |
|

### getMaxIntsToIndexField() {#getMaxIntsToIndexField--}
```
public abstract int getMaxIntsToIndexField()
```


Αποκτά τον μέγιστο αριθμό τιμών σε έναν πίνακα τύπου int για την ευρετηρίαση του πεδίου. Η προεπιλεγμένη τιμή είναι  Integer.MAX_VALUE .


**Returns:**
int - Ο μέγιστος αριθμός τιμών σε έναν πίνακα τύπου int για την ευρετηρίαση του πεδίου.

### setMaxIntsToIndexField(int value) {#setMaxIntsToIndexField-int-}
```
public abstract void setMaxIntsToIndexField(int value)
```


Ορίζει τον μέγιστο αριθμό τιμών σε έναν πίνακα τύπου int για την ευρετηρίαση του πεδίου. Η προεπιλεγμένη τιμή είναι  Integer.MAX_VALUE .


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | τιμή | int | Ο μέγιστος αριθμός τιμών σε έναν πίνακα τύπου int για την ευρετηρίαση του πεδίου. |
|

### getMaxLongsToIndexField() {#getMaxLongsToIndexField--}
```
public abstract int getMaxLongsToIndexField()
```


Αποκτά τον μέγιστο αριθμό τιμών σε έναν πίνακα τύπου long για την ευρετηρίαση του πεδίου. Η προεπιλεγμένη τιμή είναι  Integer.MAX_VALUE .


**Returns:**
int - Ο μέγιστος αριθμός τιμών σε έναν πίνακα τύπου long για την ευρετηρίαση του πεδίου.

### setMaxLongsToIndexField(int value) {#setMaxLongsToIndexField-int-}
```
public abstract void setMaxLongsToIndexField(int value)
```


Ορίζει τον μέγιστο αριθμό τιμών σε έναν πίνακα τύπου long για την ευρετηρίαση του πεδίου. Η προεπιλεγμένη τιμή είναι  Integer.MAX_VALUE .


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | τιμή | int | Ο μέγιστος αριθμός τιμών σε έναν πίνακα τύπου long για την ευρετηρίαση του πεδίου. |
|

### getMaxDoublesToIndexField() {#getMaxDoublesToIndexField--}
```
public abstract int getMaxDoublesToIndexField()
```


Λαμβάνει τον μέγιστο αριθμό τιμών σε έναν πίνακα τύπου double για την ευρετηρίαση του πεδίου. Η προεπιλεγμένη τιμή είναι  Integer.MAX_VALUE .


**Returns:**
int - Ο μέγιστος αριθμός τιμών σε έναν πίνακα τύπου double για την ευρετηρίαση του πεδίου.

### setMaxDoublesToIndexField(int value) {#setMaxDoublesToIndexField-int-}
```
public abstract void setMaxDoublesToIndexField(int value)
```


Ορίζει τον μέγιστο αριθμό τιμών σε έναν πίνακα τύπου double για την ευρετηρίαση του πεδίου. Η προεπιλεγμένη τιμή είναι  Integer.MAX_VALUE .


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | τιμή | int | Ο μέγιστος αριθμός τιμών σε έναν πίνακα τύπου double για την ευρετηρίαση του πεδίου. |
|

### getSeparatorBetweenValues() {#getSeparatorBetweenValues--}
```
public abstract String getSeparatorBetweenValues()
```


Λαμβάνει το διαχωριστικό μεταξύ τιμών σε ένα πεδίο τύπου πίνακα. Η προεπιλεγμένη τιμή είναι το σύμβολο διαστήματος.


**Returns:**
java.lang.String - Το διαχωριστικό μεταξύ τιμών σε ένα πεδίο τύπου πίνακα.

### setSeparatorBetweenValues(String value) {#setSeparatorBetweenValues-java.lang.String-}
```
public abstract void setSeparatorBetweenValues(String value)
```


Ορίζει το διαχωριστικό μεταξύ τιμών σε ένα πεδίο τύπου πίνακα. Η προεπιλεγμένη τιμή είναι το σύμβολο διαστήματος.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | τιμή | java.lang.String | Το διαχωριστικό μεταξύ τιμών σε ένα πεδίο τύπου πίνακα. |
|

