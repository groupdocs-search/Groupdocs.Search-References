---
title: "StopWordDictionary"
second_title: "GroupDocs.Search για Java API Reference"
description: "Ορίζει τη διεπαφή ενός λεξικού λέξεων-αποκλεισμού."
type: docs
weight: 22
url: /el/java/com.groupdocs.search.dictionaries/stopworddictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface StopWordDictionary extends DictionaryBase, Iterable<String>
```

Ορίζει τη διεπαφή ενός λεξικού λέξεων-αποκλεισμού.


**Learn more**

* [Indexing with stop words](../https://docs.groupdocs.com/display/searchjava/Indexing+with+stop+words)
* [Managing stop word dictionary](../https://docs.groupdocs.com/display/searchjava/Stop+word+dictionary)

## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getCount()](#getCount--) | Αποκτά τον αριθμό των λέξεων-σταματημάτων που περιέχονται στο StopWordDictionary. |
|
|  | [addRange(Iterable<String> words)](#addRange-java.lang.Iterable-java.lang.String--) | Προσθέτει τη συγκεκριμένη συλλογή λέξεων σε αυτήν την παρουσία του StopWordDictionary. |
|
|  | [addRange(String[] words)](#addRange-java.lang.String---) | Προσθέτει τη συγκεκριμένη συλλογή λέξεων σε αυτήν την παρουσία του StopWordDictionary. |
|
|  | [removeRange(Iterable<String> words)](#removeRange-java.lang.Iterable-java.lang.String--) | Αφαιρεί τη συγκεκριμένη συλλογή λέξεων από αυτήν την παρουσία του StopWordDictionary. |
|
|  | [removeRange(String[] words)](#removeRange-java.lang.String---) | Αφαιρεί τη συγκεκριμένη συλλογή λέξεων από αυτήν την παρουσία του StopWordDictionary. |
|
|  | [contains(String word)](#contains-java.lang.String-) | Καθορίζει εάν ένα αντικείμενο StopWordDictionary περιέχει τη συγκεκριμένη λέξη. |
|
|  | [clear()](#clear--) | Αφαιρεί όλες τις λέξεις από ένα αντικείμενο StopWordDictionary. |
|
|  | [iterator()](#iterator--) | Επιστρέφει έναν επαναλήπτη που διασχίζει τη συλλογή. |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


Αποκτά τον αριθμό των λέξεων-σταματημάτων που περιέχονται στο StopWordDictionary.


**Returns:**
int - Ο αριθμός των λέξεων-σταματημάτων στο λεξικό.

### addRange(Iterable<String> words) {#addRange-java.lang.Iterable-java.lang.String--}
```
public abstract void addRange(Iterable<String> words)
```


Προσθέτει τη συγκεκριμένη συλλογή λέξεων σε αυτήν την παρουσία του StopWordDictionary.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | λέξεις | java.lang.Iterable<java.lang.String> | Η συλλογή των λέξεων για προσθήκη στο λεξικό. |
|

### addRange(String[] words) {#addRange-java.lang.String---}
```
public abstract void addRange(String[] words)
```


Προσθέτει τη συγκεκριμένη συλλογή λέξεων σε αυτήν την παρουσία του StopWordDictionary.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | λέξεις | java.lang.String[] | Η συλλογή των λέξεων για προσθήκη στο λεξικό. |
|

### removeRange(Iterable<String> words) {#removeRange-java.lang.Iterable-java.lang.String--}
```
public abstract void removeRange(Iterable<String> words)
```


Αφαιρεί τη συγκεκριμένη συλλογή λέξεων από αυτήν την παρουσία του StopWordDictionary.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | λέξεις | java.lang.Iterable<java.lang.String> | Η συλλογή των λέξεων για αφαίρεση. |
|

### removeRange(String[] words) {#removeRange-java.lang.String---}
```
public abstract void removeRange(String[] words)
```


Αφαιρεί τη συγκεκριμένη συλλογή λέξεων από αυτήν την παρουσία του StopWordDictionary.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | λέξεις | java.lang.String[] | Η συλλογή των λέξεων για αφαίρεση. |
|

### contains(String word) {#contains-java.lang.String-}
```
public abstract boolean contains(String word)
```


Καθορίζει εάν ένα αντικείμενο StopWordDictionary περιέχει τη συγκεκριμένη λέξη.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | λέξη | java.lang.String | Η λέξη για εντοπισμό στο αντικείμενο StopWordDictionary. |
|

**Returns:**
boolean - true εάν το αντικείμενο StopWordDictionary περιέχει τη συγκεκριμένη λέξη· διαφορετικά, false.

### clear() {#clear--}
```
public abstract void clear()
```


Αφαιρεί όλες τις λέξεις από ένα αντικείμενο StopWordDictionary.


### iterator() {#iterator--}
```
public abstract Iterator<String> iterator()
```


Επιστρέφει έναν επαναλήπτη που διασχίζει τη συλλογή.


**Returns:**
java.util.Iterator<java.lang.String> - Ένας επαναλήπτης που μπορεί να χρησιμοποιηθεί για επανάληψη μέσω της συλλογής.

