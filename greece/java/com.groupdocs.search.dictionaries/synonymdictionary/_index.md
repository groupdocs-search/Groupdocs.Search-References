---
title: "SynonymDictionary"
second_title: "GroupDocs.Search για Java API Reference"
description: "Ορίζει τη διεπαφή ενός λεξικού συνωνύμων."
type: docs
weight: 23
url: /el/java/com.groupdocs.search.dictionaries/synonymdictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface SynonymDictionary extends DictionaryBase, Iterable<String>
```

Ορίζει τη διεπαφή ενός λεξικού συνωνύμων.


**Learn more**

* [Synonym search](../https://docs.groupdocs.com/display/searchjava/Synonym+search)
* [Managing synonym dictionary](../https://docs.groupdocs.com/display/searchjava/Synonym+dictionary)

## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getCount()](#getCount--) | Λαμβάνει τον αριθμό των λέξεων που περιέχονται σε αυτό το SynonymDictionary. |
|
|  | [addRange(Iterable<String[]> synonyms)](#addRange-java.lang.Iterable-java.lang.String----) | Προσθέτει τη συγκεκριμένη συλλογή ομάδων συνωνύμων σε αυτήν την παρουσία του SynonymDictionary. |
|
|  | [addRange(String[][] synonyms)](#addRange-java.lang.String-----) | Προσθέτει τη συγκεκριμένη συλλογή ομάδων συνωνύμων σε αυτήν την παρουσία του SynonymDictionary. |
|
|  | [clear()](#clear--) | Αφαιρεί όλες τις λέξεις από αυτό το αντικείμενο SynonymDictionary. |
|
|  | [getSynonyms(String word)](#getSynonyms-java.lang.String-) | Λαμβάνει τα συνώνυμα για τη συγκεκριμένη λέξη. |
|
|  | [getSynonymGroups(String word)](#getSynonymGroups-java.lang.String-) | Λαμβάνει όλες τις ομάδες συνωνύμων στις οποίες ανήκει η συγκεκριμένη λέξη. |
|
|  | [getAllSynonymGroups()](#getAllSynonymGroups--) | Λαμβάνει όλες τις ομάδες συνωνύμων που περιέχονται σε αυτό το λεξικό. |
|
|  | [iterator()](#iterator--) | Επιστρέφει έναν επαναλήπτη που διασχίζει τη συλλογή. |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


Λαμβάνει τον αριθμό των λέξεων που περιέχονται σε αυτό το SynonymDictionary.


**Returns:**
int - Ο αριθμός των λέξεων που περιέχονται σε αυτό το SynonymDictionary.

### addRange(Iterable<String[]> synonyms) {#addRange-java.lang.Iterable-java.lang.String----}
```
public abstract void addRange(Iterable<String[]> synonyms)
```


Προσθέτει τη συγκεκριμένη συλλογή ομάδων συνωνύμων σε αυτήν την παρουσία του SynonymDictionary.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | συνώνυμα | java.lang.Iterable<java.lang.String[]> | Η συλλογή των ομάδων συνωνύμων για προσθήκη στο λεξικό. |
|

### addRange(String[][] synonyms) {#addRange-java.lang.String-----}
```
public abstract void addRange(String[][] synonyms)
```


Προσθέτει τη συγκεκριμένη συλλογή ομάδων συνωνύμων σε αυτήν την παρουσία του SynonymDictionary.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | συνώνυμα | java.lang.String[][] | Η συλλογή των ομάδων συνωνύμων για προσθήκη στο λεξικό. |
|

### clear() {#clear--}
```
public abstract void clear()
```


Αφαιρεί όλες τις λέξεις από αυτό το αντικείμενο SynonymDictionary.


### getSynonyms(String word) {#getSynonyms-java.lang.String-}
```
public abstract String[] getSynonyms(String word)
```


Λαμβάνει τα συνώνυμα για τη συγκεκριμένη λέξη. Ο τελικός πίνακας δεν περιέχει την αρχική λέξη.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | λέξη | java.lang.String | Η λέξη για την πρόταση των συνωνύμων. |
|

**Returns:**
java.lang.String[] - Τα συνώνυμα για τη συγκεκριμένη λέξη ή κενός πίνακας εάν το αντικείμενο SynonymDictionary δεν περιέχει τη συγκεκριμένη λέξη.

### getSynonymGroups(String word) {#getSynonymGroups-java.lang.String-}
```
public abstract String[][] getSynonymGroups(String word)
```


Λαμβάνει όλες τις ομάδες συνωνύμων στις οποίες ανήκει η συγκεκριμένη λέξη.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | λέξη | java.lang.String | Η λέξη για λήψη ομάδων συνωνύμων. |
|

**Returns:**
java.lang.String[][] - Όλες οι ομάδες συνωνύμων στις οποίες ανήκει η καθορισμένη λέξη.

### getAllSynonymGroups() {#getAllSynonymGroups--}
```
public abstract String[][] getAllSynonymGroups()
```


Λαμβάνει όλες τις ομάδες συνωνύμων που περιέχονται σε αυτό το λεξικό.


**Returns:**
java.lang.String[][] - Όλες οι ομάδες συνωνύμων.

### iterator() {#iterator--}
```
public abstract Iterator<String> iterator()
```


Επιστρέφει έναν επαναλήπτη που διασχίζει τη συλλογή.


**Returns:**
java.util.Iterator<java.lang.String> - Ένας επαναλήπτης που μπορεί να χρησιμοποιηθεί για επανάληψη μέσω της συλλογής.

