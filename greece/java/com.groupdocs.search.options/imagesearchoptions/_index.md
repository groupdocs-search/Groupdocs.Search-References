---
title: "ImageSearchOptions"
second_title: "GroupDocs.Search για Java API Reference"
description: "Παρέχει επιλογές για τη λειτουργία αντίστροφης αναζήτησης εικόνας."
type: docs
weight: 24
url: /el/java/com.groupdocs.search.options/imagesearchoptions/
---
**Inheritance:**
java.lang.Object
```
public class ImageSearchOptions
```

Παρέχει επιλογές για τη λειτουργία αντίστροφης αναζήτησης εικόνας.

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [ImageSearchOptions()](#ImageSearchOptions--) | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης  ImageSearchOptions . |
|
|  | [ImageSearchOptions(Object data)](#ImageSearchOptions-java.lang.Object-) | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης  ImageSearchOptions . |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getHashDifferences()](#getHashDifferences--) | Λαμβάνει τον μέγιστο αριθμό μη αντιστοιχισμένων bits στο hash της εικόνας. |
|
|  | [setHashDifferences(int value)](#setHashDifferences-int-) | Ορίζει τον μέγιστο αριθμό μη αντιστοιχισμένων bits στο hash της εικόνας. |
|
|  | [getMaxResultCount()](#getMaxResultCount--) | Λαμβάνει τον μέγιστο αριθμό εικόνων που βρέθηκαν για ένα αίτημα αντίστροφης αναζήτησης εικόνας. |
|
|  | [setMaxResultCount(int value)](#setMaxResultCount-int-) | Ορίζει τον μέγιστο αριθμό εικόνων που βρέθηκαν για ένα αίτημα αντίστροφης αναζήτησης εικόνας. |
|
|  | [getSearchDocumentFilter()](#getSearchDocumentFilter--) | Λαμβάνει το φίλτρο εγγράφου αναζήτησης. |
|
|  | [setSearchDocumentFilter(ISearchDocumentFilter value)](#setSearchDocumentFilter-com.groupdocs.search.options.ISearchDocumentFilter-) | Λαμβάνει ή ορίζει το φίλτρο εγγράφου αναζήτησης. |
|
| [getCore()](#getCore--) |  |
### ImageSearchOptions() {#ImageSearchOptions--}
```
public ImageSearchOptions()
```


Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης  ImageSearchOptions .


### ImageSearchOptions(Object data) {#ImageSearchOptions-java.lang.Object-}
```
public ImageSearchOptions(Object data)
```


Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης  ImageSearchOptions .


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | δεδομένα | java.lang.Object | Τα σειριοποιημένα δεδομένα. |
|

### getHashDifferences() {#getHashDifferences--}
```
public int getHashDifferences()
```


Λαμβάνει τον μέγιστο αριθμό μη αντιστοιχισμένων bits στο hash της εικόνας. Η προεπιλεγμένη τιμή είναι  5 .


**Returns:**
int - Μέγιστος αριθμός μη αντιστοιχισμένων bits στο hash της εικόνας.

### setHashDifferences(int value) {#setHashDifferences-int-}
```
public void setHashDifferences(int value)
```


Ορίζει τον μέγιστο αριθμό μη αντιστοιχισμένων bits στο hash της εικόνας. Η προεπιλεγμένη τιμή είναι 5.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | τιμή | int | Ο μέγιστος αριθμός μη αντιστοιχισμένων bits στο hash της εικόνας. |
|

### getMaxResultCount() {#getMaxResultCount--}
```
public int getMaxResultCount()
```


Λαμβάνει τον μέγιστο αριθμό εικόνων που βρέθηκαν για αίτημα αντίστροφης αναζήτησης εικόνας. Η προεπιλεγμένη τιμή είναι 1000.


**Returns:**
int - Ο μέγιστος αριθμός εικόνων που βρέθηκαν για αίτημα αντίστροφης αναζήτησης εικόνας.

### setMaxResultCount(int value) {#setMaxResultCount-int-}
```
public void setMaxResultCount(int value)
```


Ορίζει τον μέγιστο αριθμό εικόνων που βρέθηκαν για αίτημα αντίστροφης αναζήτησης εικόνας. Η προεπιλεγμένη τιμή είναι 1000.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | τιμή | int | Ο μέγιστος αριθμός εικόνων που βρέθηκαν για αίτημα αντίστροφης αναζήτησης εικόνας. |
|

### getSearchDocumentFilter() {#getSearchDocumentFilter--}
```
public ISearchDocumentFilter getSearchDocumentFilter()
```


Λαμβάνει το φίλτρο εγγράφου αναζήτησης.  SearchDocumentFilter  λειτουργεί με λογική ένταξης. Χρησιμοποιήστε την κλάση  GroupDocs.Search.Options.SearchDocumentFilter  για δημιουργία παραδειγμάτων φίλτρου εγγράφου αναζήτησης. Η προεπιλεγμένη τιμή είναι  null , που σημαίνει ότι όλα τα ευρεθέντα έγγραφα θα επιστραφούν.


**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - The search document filter.

### setSearchDocumentFilter(ISearchDocumentFilter value) {#setSearchDocumentFilter-com.groupdocs.search.options.ISearchDocumentFilter-}
```
public void setSearchDocumentFilter(ISearchDocumentFilter value)
```


Λαμβάνει ή ορίζει το φίλτρο εγγράφου αναζήτησης.  SearchDocumentFilter  λειτουργεί με λογική ένταξης. Χρησιμοποιήστε την κλάση  GroupDocs.Search.Options.SearchDocumentFilter  για δημιουργία παραδειγμάτων φίλτρου εγγράφου αναζήτησης. Η προεπιλεγμένη τιμή είναι  null , που σημαίνει ότι όλα τα ευρεθέντα έγγραφα θα επιστραφούν.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | value | [ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) | Το φίλτρο εγγράφου αναζήτησης. |
|

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
