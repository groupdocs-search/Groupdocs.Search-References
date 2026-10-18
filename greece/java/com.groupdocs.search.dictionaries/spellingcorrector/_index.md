---
title: "SpellingCorrector"
second_title: "GroupDocs.Search για Java API Reference"
description: "Ορίζει τη διεπαφή ενός διορθωτή ορθογραφίας για όρους σε ένα ερώτημα."
type: docs
weight: 21
url: /el/java/com.groupdocs.search.dictionaries/spellingcorrector/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase)
```
public interface SpellingCorrector extends DictionaryBase
```

Ορίζει τη διεπαφή ενός διορθωτή ορθογραφίας για όρους σε ένα ερώτημα.


**Learn more**

* [Spell checking](../https://docs.groupdocs.com/display/searchjava/Spell+checking)
* [Managing spelling corrector](../https://docs.groupdocs.com/display/searchjava/Spelling+corrector)

## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getCount()](#getCount--) | Λαμβάνει τον αριθμό των λέξεων που περιέχονται σε αυτό το SpellingCorrector. |
|
|  | [getWords()](#getWords--) | Λαμβάνει τη συλλογή των λέξεων που περιέχονται αυτήν τη στιγμή σε αυτό το SpellingCorrector. |
|
|  | [addRange(Iterable<String> words)](#addRange-java.lang.Iterable-java.lang.String--) | Προσθέτει τη συγκεκριμένη συλλογή λέξεων σε αυτήν την παρουσία του SpellingCorrector. |
|
|  | [addRange(String[] words)](#addRange-java.lang.String---) | Προσθέτει τη συγκεκριμένη συλλογή λέξεων σε αυτήν την παρουσία του SpellingCorrector. |
|
|  | [clear()](#clear--) | Αφαιρεί όλες τις λέξεις από ένα αντικείμενο SpellingCorrector. |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


Λαμβάνει τον αριθμό των λέξεων που περιέχονται σε αυτό το SpellingCorrector.


**Returns:**
int - Ο αριθμός των λέξεων που περιέχονται σε αυτό το SpellingCorrector.

### getWords() {#getWords--}
```
public abstract String[] getWords()
```


Λαμβάνει τη συλλογή των λέξεων που περιέχονται αυτήν τη στιγμή σε αυτό το SpellingCorrector.


**Returns:**
java.lang.String[] - Η συλλογή των λέξεων.

### addRange(Iterable<String> words) {#addRange-java.lang.Iterable-java.lang.String--}
```
public abstract void addRange(Iterable<String> words)
```


Προσθέτει τη συγκεκριμένη συλλογή λέξεων σε αυτήν την παρουσία του SpellingCorrector.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | λέξεις | java.lang.Iterable<java.lang.String> | Η συλλογή των λέξεων για προσθήκη στο λεξικό. |
|

### addRange(String[] words) {#addRange-java.lang.String---}
```
public abstract void addRange(String[] words)
```


Προσθέτει τη συγκεκριμένη συλλογή λέξεων σε αυτήν την παρουσία του SpellingCorrector.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | λέξεις | java.lang.String[] | Η συλλογή των λέξεων για προσθήκη στο λεξικό. |
|

### clear() {#clear--}
```
public abstract void clear()
```


Αφαιρεί όλες τις λέξεις από ένα αντικείμενο SpellingCorrector.


