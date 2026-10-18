---
title: "HomophoneDictionary"
second_title: "GroupDocs.Search για Java API Reference"
description: "Ορίζει τη διεπαφή ενός λεξικού ομοηχείων με διαφορετική ορθογραφία."
type: docs
weight: 18
url: /el/java/com.groupdocs.search.dictionaries/homophonedictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface HomophoneDictionary extends DictionaryBase, Iterable<String>
```

Ορίζει τη διεπαφή ενός λεξικού ομοηχείων με διαφορετική ορθογραφία.


**Learn more**

* [Homophone search](../https://docs.groupdocs.com/display/searchjava/Homophone+search)
* [Managing homophone dictionary](../https://docs.groupdocs.com/display/searchjava/Homophone+dictionary)

## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getCount()](#getCount--) | Αποκτά τον αριθμό των λέξεων που περιέχονται σε αυτό το  HomophoneDictionary . |
|
|  | [addRange(Iterable<String[]> homophones)](#addRange-java.lang.Iterable-java.lang.String----) | Προσθέτει τη συγκεκριμένη συλλογή ομάδων ομόφωνων σε αυτήν την παρουσία του  HomophoneDictionary . |
|
|  | [addRange(String[][] homophones)](#addRange-java.lang.String-----) | Προσθέτει τη συγκεκριμένη συλλογή ομάδων ομόφωνων σε αυτήν την παρουσία του  HomophoneDictionary . |
|
|  | [clear()](#clear--) | Αφαιρεί όλες τις λέξεις από ένα αντικείμενο  HomophoneDictionary . |
|
|  | [getHomophones(String word)](#getHomophones-java.lang.String-) | Αποκτά τα ομόφωνα για τη συγκεκριμένη λέξη. |
|
|  | [getHomophoneGroups(String word)](#getHomophoneGroups-java.lang.String-) | Αποκτά όλες τις ομάδες ομόφωνων στις οποίες ανήκει η συγκεκριμένη λέξη. |
|
|  | [getAllHomophoneGroups()](#getAllHomophoneGroups--) | Αποκτά όλες τις ομάδες ομόφωνων που περιέχονται σε αυτό το λεξικό. |
|
|  | [iterator()](#iterator--) | Επιστρέφει έναν επαναλήπτη που διασχίζει τη συλλογή. |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


Αποκτά τον αριθμό των λέξεων που περιέχονται σε αυτό το  HomophoneDictionary .


**Returns:**
int - Ο αριθμός των λέξεων.

### addRange(Iterable<String[]> homophones) {#addRange-java.lang.Iterable-java.lang.String----}
```
public abstract void addRange(Iterable<String[]> homophones)
```


Προσθέτει τη συγκεκριμένη συλλογή ομάδων ομόφωνων σε αυτήν την παρουσία του  HomophoneDictionary .


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | homophones | java.lang.Iterable<java.lang.String[]> | Η συλλογή των ομάδων ομόφωνων για προσθήκη στο λεξικό. |
|

### addRange(String[][] homophones) {#addRange-java.lang.String-----}
```
public abstract void addRange(String[][] homophones)
```


Προσθέτει τη συγκεκριμένη συλλογή ομάδων ομόφωνων σε αυτήν την παρουσία του  HomophoneDictionary .


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | homophones | java.lang.String[][] | Η συλλογή των ομάδων ομόφωνων για προσθήκη στο λεξικό. |
|

### clear() {#clear--}
```
public abstract void clear()
```


Αφαιρεί όλες τις λέξεις από ένα αντικείμενο  HomophoneDictionary .


### getHomophones(String word) {#getHomophones-java.lang.String-}
```
public abstract String[] getHomophones(String word)
```


Αποκτά τα ομόφωνα για τη συγκεκριμένη λέξη. Ο τελικός πίνακας δεν περιέχει τη αρχική λέξη.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | λέξη | java.lang.String | Η λέξη για πρόταση των ομοηχείων. |
|

**Returns:**
java.lang.String[] - Τα ομοηχεία για τη συγκεκριμένη λέξη ή κενός πίνακας εάν το αντικείμενο HomophoneDictionary δεν περιέχει τη συγκεκριμένη λέξη.

### getHomophoneGroups(String word) {#getHomophoneGroups-java.lang.String-}
```
public abstract String[][] getHomophoneGroups(String word)
```


Αποκτά όλες τις ομάδες ομόφωνων στις οποίες ανήκει η συγκεκριμένη λέξη.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | λέξη | java.lang.String | Η λέξη για λήψη ομάδων ομοηχείων. |
|

**Returns:**
java.lang.String[][] - Όλες οι ομάδες ομοηχείων στις οποίες ανήκει η συγκεκριμένη λέξη.

### getAllHomophoneGroups() {#getAllHomophoneGroups--}
```
public abstract String[][] getAllHomophoneGroups()
```


Αποκτά όλες τις ομάδες ομόφωνων που περιέχονται σε αυτό το λεξικό.


**Returns:**
java.lang.String[][] - Όλες οι ομάδες ομοηχείων.

### iterator() {#iterator--}
```
public abstract Iterator<String> iterator()
```


Επιστρέφει έναν επαναλήπτη που διασχίζει τη συλλογή.


**Returns:**
java.util.Iterator<java.lang.String> - Ένας επαναλήπτης που μπορεί να χρησιμοποιηθεί για επανάληψη μέσω της συλλογής.

