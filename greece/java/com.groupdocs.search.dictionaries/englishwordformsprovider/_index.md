---
title: "EnglishWordFormsProvider"
second_title: "GroupDocs.Search για Java API Reference"
description: "Αντιπροσωπεύει έναν πάροχο αγγλικών μορφών λέξεων."
type: docs
weight: 13
url: /el/java/com.groupdocs.search.dictionaries/englishwordformsprovider/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.IWordFormsProvider](../../com.groupdocs.search.dictionaries/iwordformsprovider)
```
public class EnglishWordFormsProvider implements IWordFormsProvider
```

Αντιπροσωπεύει έναν πάροχο αγγλικών μορφών λέξεων.


**Learn more**

* [Search for different word forms](../https://docs.groupdocs.com/display/searchjava/Search+for+different+word+forms)
* [Word forms provider](../https://docs.groupdocs.com/display/searchjava/Word+forms+provider)

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [EnglishWordFormsProvider()](#EnglishWordFormsProvider--) | Αρχικοποιεί μια νέα παρουσία της |
EnglishWordFormsProvider
κλάσης.
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getWordForms(String word)](#getWordForms-java.lang.String-) | Λαμβάνει τις μορφές λέξης για τη συγκεκριμένη λέξη. |
|
### EnglishWordFormsProvider() {#EnglishWordFormsProvider--}
```
public EnglishWordFormsProvider()
```


Αρχικοποιεί μια νέα παρουσία της
EnglishWordFormsProvider
κλάσης.


### getWordForms(String word) {#getWordForms-java.lang.String-}
```
public final String[] getWordForms(String word)
```


Λαμβάνει τις μορφές λέξης για τη συγκεκριμένη λέξη.
Ο τελικός πίνακας δεν περιέχει την αρχική λέξη.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | λέξη | java.lang.String | Η λέξη για πρόταση των μορφών λέξης. |
|

**Returns:**
java.lang.String[] - Οι μορφές λέξης για τη συγκεκριμένη λέξη ή κενός πίνακας εάν ο IWordFormsProvider δεν παρέχει μορφές λέξης για τη συγκεκριμένη λέξη.

