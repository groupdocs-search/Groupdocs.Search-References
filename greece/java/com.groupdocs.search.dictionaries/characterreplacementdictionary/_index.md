---
title: "CharacterReplacementDictionary"
second_title: "GroupDocs.Search για Java API Reference"
description: "Ορίζει τη διεπαφή ενός λεξικού αντικατάστασης χαρακτήρων που χρησιμοποιείται κατά τη διαδικασία ευρετηρίασης."
type: docs
weight: 16
url: /el/java/com.groupdocs.search.dictionaries/characterreplacementdictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface CharacterReplacementDictionary extends DictionaryBase, Iterable<Character>
```

Ορίζει τη διεπαφή ενός λεξικού αντικατάστασης χαρακτήρων που χρησιμοποιείται κατά τη διαδικασία ευρετηρίασης. Η αντικατάσταση χαρακτήρων μπορεί, για παράδειγμα, να χρησιμοποιηθεί για την αφαίρεση τόνων από τονισμένους χαρακτήρες ή για τη δημιουργία ευρετηρίου χωρίς διάκριση πεζών-κεφαλαίων.


**Learn more**

* [Character replacement during Indexing](../https://docs.groupdocs.com/display/searchjava/Character+replacement+during+Indexing)
* [Managing character replacements](../https://docs.groupdocs.com/display/searchjava/Character+replacements)

## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getCount()](#getCount--) | Λαμβάνει τον αριθμό των χαρακτήρων που περιέχονται σε αυτό το CharacterReplacementDictionary. |
|
|  | [addRange(Iterable<CharacterReplacementPair> characterReplacements)](#addRange-java.lang.Iterable-com.groupdocs.search.dictionaries.CharacterReplacementPair--) | Προσθέτει τη συγκεκριμένη συλλογή αντικαταστάσεων χαρακτήρων σε αυτήν την παρουσία του CharacterReplacementDictionary. |
|
|  | [addRange(CharacterReplacementPair[] characterReplacements)](#addRange-com.groupdocs.search.dictionaries.CharacterReplacementPair---) | Προσθέτει τη συγκεκριμένη συλλογή αντικαταστάσεων χαρακτήρων σε αυτήν την παρουσία του CharacterReplacementDictionary. |
|
|  | [removeRange(char[] characters)](#removeRange-char---) | Αφαιρεί τη συγκεκριμένη συλλογή αντικαταστάσεων χαρακτήρων από αυτήν την παρουσία του CharacterReplacementDictionary. |
|
|  | [contains(char character)](#contains-char-) | Καθορίζει εάν ένα αντικείμενο CharacterReplacementDictionary περιέχει αντικατάσταση για τον καθορισμένο χαρακτήρα. |
|
|  | [getReplacement(char character)](#getReplacement-char-) | Λαμβάνει μια αντικατάσταση για τον καθορισμένο χαρακτήρα. |
|
|  | [clear()](#clear--) | Αφαιρεί όλες τις αντικαταστάσεις χαρακτήρων από ένα αντικείμενο CharacterReplacementDictionary. |
|
|  | [iterator()](#iterator--) | Επιστρέφει έναν επαναλήπτη που διασχίζει τη συλλογή. |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


Λαμβάνει τον αριθμό των χαρακτήρων που περιέχονται σε αυτό το CharacterReplacementDictionary.


**Returns:**
int - Ο αριθμός των χαρακτήρων στο λεξικό.

### addRange(Iterable<CharacterReplacementPair> characterReplacements) {#addRange-java.lang.Iterable-com.groupdocs.search.dictionaries.CharacterReplacementPair--}
```
public abstract void addRange(Iterable<CharacterReplacementPair> characterReplacements)
```


Προσθέτει τη συγκεκριμένη συλλογή αντικαταστάσεων χαρακτήρων σε αυτήν την παρουσία του CharacterReplacementDictionary.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | characterReplacements | java.lang.Iterable<com.groupdocs.search.dictionaries.CharacterReplacementPair> | Η συλλογή των αντικαταστάσεων χαρακτήρων που θα προστεθούν στο λεξικό. |
|

### addRange(CharacterReplacementPair[] characterReplacements) {#addRange-com.groupdocs.search.dictionaries.CharacterReplacementPair---}
```
public abstract void addRange(CharacterReplacementPair[] characterReplacements)
```


Προσθέτει τη συγκεκριμένη συλλογή αντικαταστάσεων χαρακτήρων σε αυτήν την παρουσία του CharacterReplacementDictionary.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | characterReplacements | [CharacterReplacementPair\[\]](../../com.groupdocs.search.dictionaries/characterreplacementpair) | Η συλλογή των αντικαταστάσεων χαρακτήρων που θα προστεθούν στο λεξικό. |
|

### removeRange(char[] characters) {#removeRange-char---}
```
public abstract void removeRange(char[] characters)
```


Αφαιρεί τη συγκεκριμένη συλλογή αντικαταστάσεων χαρακτήρων από αυτήν την παρουσία του CharacterReplacementDictionary.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | χαρακτήρες | char[] | Η συλλογή των χαρακτήρων που θα αφαιρεθούν. |
|

### contains(char character) {#contains-char-}
```
public abstract boolean contains(char character)
```


Καθορίζει εάν ένα αντικείμενο CharacterReplacementDictionary περιέχει αντικατάσταση για τον καθορισμένο χαρακτήρα.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | χαρακτήρας | char | Ο χαρακτήρας που θα εντοπιστεί στο αντικείμενο CharacterReplacementDictionary. |
|

**Returns:**
boolean - true εάν το αντικείμενο CharacterReplacementDictionary περιέχει τον καθορισμένο χαρακτήρα· διαφορετικά, false.

### getReplacement(char character) {#getReplacement-char-}
```
public abstract char getReplacement(char character)
```


Λαμβάνει μια αντικατάσταση για τον καθορισμένο χαρακτήρα.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | χαρακτήρας | char | Ο χαρακτήρας για τον οποίο θα ληφθεί μια αντικατάσταση. |
|

**Returns:**
char - Η αντικατάσταση για τον καθορισμένο χαρακτήρα.

### clear() {#clear--}
```
public abstract void clear()
```


Αφαιρεί όλες τις αντικαταστάσεις χαρακτήρων από ένα αντικείμενο CharacterReplacementDictionary.


### iterator() {#iterator--}
```
public abstract Iterator<Character> iterator()
```


Επιστρέφει έναν επαναλήπτη που διασχίζει τη συλλογή.


**Returns:**
java.util.Iterator<java.lang.Character> - Ένας επαναλήπτης που μπορεί να χρησιμοποιηθεί για επανάληψη μέσω της συλλογής.

