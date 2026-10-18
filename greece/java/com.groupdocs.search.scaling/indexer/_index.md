---
title: "Indexer"
second_title: "GroupDocs.Search για Java API Reference"
description: "Αντιπροσωπεύει μια υπηρεσία που διαχειρίζεται τη διανομή των ευρετηριασμένων εγγράφων σε τμήματα του δικτύου αναζήτησης."
type: docs
weight: 10
url: /el/java/com.groupdocs.search.scaling/indexer/
---
**Inheritance:**
java.lang.Object
```
public abstract class Indexer
```

Αντιπροσωπεύει μια υπηρεσία που διαχειρίζεται τη διανομή των ευρετηριασμένων εγγράφων σε τμήματα του δικτύου αναζήτησης.

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [Indexer()](#Indexer--) |  |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [add(Document[] documents, String[] passwords, IndexingOptions options)](#add-com.groupdocs.search.Document---java.lang.String---com.groupdocs.search.options.IndexingOptions-) | Εκτελεί λειτουργία ευρετηρίου. |
|
|  | [add(ExtractedData[] data, IndexingOptions options)](#add-com.groupdocs.search.ExtractedData---com.groupdocs.search.options.IndexingOptions-) | Εκτελεί λειτουργία ευρετηρίου. |
|
|  | [delete(String[] documentKeys, DeleteOptions options)](#delete-java.lang.String---com.groupdocs.search.options.DeleteOptions-) | Διαγράφει τα ευρετηριασμένα έγγραφα. |
|
|  | [optimize(OptimizeOptions options)](#optimize-com.groupdocs.search.options.OptimizeOptions-) | Μειώνει τον αριθμό των τμημάτων του ευρετηρίου συγχωνεύοντάς τα μεταξύ τους. |
|
|  | [synchronize(SynchronizeOptions options)](#synchronize-com.groupdocs.search.options.SynchronizeOptions-) | Συγχρονίζει τη λίστα των ευρετηριασμένων εγγράφων με αυτά στα shards. |
|
|  | [changeAttributes(AttributeChangeBatch batch, ChangeAttributesOptions options)](#changeAttributes-com.groupdocs.search.common.AttributeChangeBatch-com.groupdocs.search.options.ChangeAttributesOptions-) | Εφαρμόζει το καθορισμένο πακέτο αλλαγών χαρακτηριστικών στα ευρετηριασμένα έγγραφα χωρίς επανευρετηρίαση. |
|
|  | [getAttributes(String documentKey)](#getAttributes-java.lang.String-) | Λαμβάνει όλες τις ιδιότητες που σχετίζονται με το καθορισμένο ευρετηριασμένο έγγραφο. |
|
|  | [getDictionary(DictionaryType dictionaryType, int shardIndex)](#getDictionary-com.groupdocs.search.dictionaries.DictionaryType-int-) | Λαμβάνει ένα λεξικό από το καθορισμένο shard. |
|
|  | [getAlphabet(int shardIndex)](#getAlphabet-int-) | Λαμβάνει το αλφαβητικό λεξικό. |
|
|  | [getAliasDictionary(int shardIndex)](#getAliasDictionary-int-) | Λαμβάνει το λεξικό ψευδωνύμων. |
|
|  | [getCharacterReplacementDictionary(int shardIndex)](#getCharacterReplacementDictionary-int-) | Λαμβάνει το λεξικό αντικατάστασης χαρακτήρων. |
|
|  | [getSynonymDictionary(int shardIndex)](#getSynonymDictionary-int-) | Λαμβάνει το λεξικό συνωνύμων. |
|
|  | [getHomophoneDictionary(int shardIndex)](#getHomophoneDictionary-int-) | Λαμβάνει το λεξικό ομόηχων. |
|
|  | [getSpellingCorrector(int shardIndex)](#getSpellingCorrector-int-) | Λαμβάνει το λεξικό διορθωτή ορθογραφίας. |
|
|  | [getStopWordDictionary(int shardIndex)](#getStopWordDictionary-int-) | Λαμβάνει το λεξικό λέξεων-διακοπής. |
|
|  | [getPasswordDictionary(int shardIndex)](#getPasswordDictionary-int-) | Λαμβάνει το λεξικό κωδικών. |
|
|  | [setDictionary(DictionaryBase dictionary, int shardIndex)](#setDictionary-com.groupdocs.search.dictionaries.DictionaryBase-int-) | Ορίζει ένα λεξικό στο καθορισμένο τμήμα. |
|
|  | [setDictionary(DictionaryBase dictionary)](#setDictionary-com.groupdocs.search.dictionaries.DictionaryBase-) | Ορίζει ένα λεξικό σε όλα τα τμήματα. |
|
|  | [deleteAllData()](#deleteAllData--) | Διαγράφει όλα τα ευρετηριασμένα δεδομένα από όλα τα τμήματα του δικτύου αναζήτησης. |
|
### Indexer() {#Indexer--}
```
public Indexer()
```


### add(Document[] documents, String[] passwords, IndexingOptions options) {#add-com.groupdocs.search.Document---java.lang.String---com.groupdocs.search.options.IndexingOptions-}
```
public abstract void add(Document[] documents, String[] passwords, IndexingOptions options)
```


Εκτελεί λειτουργία ευρετηρίασης. Υποστηρίζεται ευρετηρίαση μόνο από ροή και δομή.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | documents | [Document\[\]](../../com.groupdocs.search/document) | Τα έγγραφα από το σύστημα αρχείων, τη ροή ή τη δομή. |
|
|  | κωδικοί πρόσβασης | java.lang.String[] | Οι κωδικοί πρόσβασης του εγγράφου. |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | Οι επιλογές προσθήκης. |
|

### add(ExtractedData[] data, IndexingOptions options) {#add-com.groupdocs.search.ExtractedData---com.groupdocs.search.options.IndexingOptions-}
```
public abstract void add(ExtractedData[] data, IndexingOptions options)
```


Εκτελεί λειτουργία ευρετηρίασης. Προσθέτει τα εξαγόμενα δεδομένα στο δίκτυο αναζήτησης.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | data | [ExtractedData\[\]](../../com.groupdocs.search/extracteddata) | Τα εξαγόμενα δεδομένα. |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | Οι επιλογές δεικτοδότησης. |
|

### delete(String[] documentKeys, DeleteOptions options) {#delete-java.lang.String---com.groupdocs.search.options.DeleteOptions-}
```
public abstract void delete(String[] documentKeys, DeleteOptions options)
```


Διαγράφει τα ευρετηριασμένα έγγραφα.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | documentKeys | java.lang.String[] | Τα κλειδιά των εγγράφων που προστέθηκαν από ροές ή δομές. |
|
|  | options | [DeleteOptions](../../com.groupdocs.search.options/deleteoptions) | Οι επιλογές διαγραφής. |
|

### optimize(OptimizeOptions options) {#optimize-com.groupdocs.search.options.OptimizeOptions-}
```
public abstract void optimize(OptimizeOptions options)
```


Μειώνει τον αριθμό των τμημάτων του ευρετηρίου συγχωνεύοντάς τα μεταξύ τους. Αυτή η λειτουργία βελτιώνει την απόδοση της αναζήτησης.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | options | [OptimizeOptions](../../com.groupdocs.search.options/optimizeoptions) | Οι επιλογές βελτιστοποίησης. |
|

### synchronize(SynchronizeOptions options) {#synchronize-com.groupdocs.search.options.SynchronizeOptions-}
```
public abstract void synchronize(SynchronizeOptions options)
```


Συγχρονίζει τη λίστα των ευρετηριασμένων εγγράφων με αυτά στα τμήματα. Αυτή η λειτουργία διορθώνει προβλήματα με την ευρετηρίαση και τη διαγραφή εγγράφων που προκλήθηκαν από προβλήματα επικοινωνίας με τους κόμβους του δικτύου αναζήτησης.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | options | [SynchronizeOptions](../../com.groupdocs.search.options/synchronizeoptions) | Οι επιλογές συγχρονισμού. |
|

### changeAttributes(AttributeChangeBatch batch, ChangeAttributesOptions options) {#changeAttributes-com.groupdocs.search.common.AttributeChangeBatch-com.groupdocs.search.options.ChangeAttributesOptions-}
```
public abstract void changeAttributes(AttributeChangeBatch batch, ChangeAttributesOptions options)
```


Εφαρμόζει το καθορισμένο πακέτο αλλαγών χαρακτηριστικών στα ευρετηριασμένα έγγραφα χωρίς επανευρετηρίαση.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | batch | [AttributeChangeBatch](../../com.groupdocs.search.common/attributechangebatch) | Η παρτίδα αλλαγής ιδιότητας. |
|
|  | options | [ChangeAttributesOptions](../../com.groupdocs.search.options/changeattributesoptions) | Οι επιλογές αλλαγής ιδιοτήτων. |
|

### getAttributes(String documentKey) {#getAttributes-java.lang.String-}
```
public abstract String[] getAttributes(String documentKey)
```


Λαμβάνει όλες τις ιδιότητες που σχετίζονται με το καθορισμένο ευρετηριασμένο έγγραφο.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | documentKey | java.lang.String | Το κλειδί του εγγράφου. |
|

**Returns:**
java.lang.String[] - Τα χαρακτηριστικά που σχετίζονται με το καθορισμένο ευρετηριασμένο έγγραφο.

### getDictionary(DictionaryType dictionaryType, int shardIndex) {#getDictionary-com.groupdocs.search.dictionaries.DictionaryType-int-}
```
public abstract DictionaryBase getDictionary(DictionaryType dictionaryType, int shardIndex)
```


Λαμβάνει ένα λεξικό από το καθορισμένο shard.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | dictionaryType | [DictionaryType](../../com.groupdocs.search.dictionaries/dictionarytype) | Ο τύπος λεξικού. |
|
|  | shardIndex | int | Ο δείκτης τμήματος. |
|

**Returns:**
[DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase) - The dictionary.

### getAlphabet(int shardIndex) {#getAlphabet-int-}
```
public abstract Alphabet getAlphabet(int shardIndex)
```


Λαμβάνει το αλφαβητικό λεξικό.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | shardIndex | int | Ο δείκτης τμήματος. |
|

**Returns:**
[Alphabet](../../com.groupdocs.search.dictionaries/alphabet) - The dictionary.

### getAliasDictionary(int shardIndex) {#getAliasDictionary-int-}
```
public abstract AliasDictionary getAliasDictionary(int shardIndex)
```


Λαμβάνει το λεξικό ψευδωνύμων.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | shardIndex | int | Ο δείκτης τμήματος. |
|

**Returns:**
[AliasDictionary](../../com.groupdocs.search.dictionaries/aliasdictionary) - The dictionary.

### getCharacterReplacementDictionary(int shardIndex) {#getCharacterReplacementDictionary-int-}
```
public abstract CharacterReplacementDictionary getCharacterReplacementDictionary(int shardIndex)
```


Λαμβάνει το λεξικό αντικατάστασης χαρακτήρων.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | shardIndex | int | Ο δείκτης τμήματος. |
|

**Returns:**
[CharacterReplacementDictionary](../../com.groupdocs.search.dictionaries/characterreplacementdictionary) - The dictionary.

### getSynonymDictionary(int shardIndex) {#getSynonymDictionary-int-}
```
public abstract SynonymDictionary getSynonymDictionary(int shardIndex)
```


Λαμβάνει το λεξικό συνωνύμων.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | shardIndex | int | Ο δείκτης τμήματος. |
|

**Returns:**
[SynonymDictionary](../../com.groupdocs.search.dictionaries/synonymdictionary) - The dictionary.

### getHomophoneDictionary(int shardIndex) {#getHomophoneDictionary-int-}
```
public abstract HomophoneDictionary getHomophoneDictionary(int shardIndex)
```


Λαμβάνει το λεξικό ομόηχων.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | shardIndex | int | Ο δείκτης τμήματος. |
|

**Returns:**
[HomophoneDictionary](../../com.groupdocs.search.dictionaries/homophonedictionary) - The dictionary.

### getSpellingCorrector(int shardIndex) {#getSpellingCorrector-int-}
```
public abstract SpellingCorrector getSpellingCorrector(int shardIndex)
```


Λαμβάνει το λεξικό διορθωτή ορθογραφίας.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | shardIndex | int | Ο δείκτης τμήματος. |
|

**Returns:**
[SpellingCorrector](../../com.groupdocs.search.dictionaries/spellingcorrector) - The dictionary.

### getStopWordDictionary(int shardIndex) {#getStopWordDictionary-int-}
```
public abstract StopWordDictionary getStopWordDictionary(int shardIndex)
```


Λαμβάνει το λεξικό λέξεων-διακοπής.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | shardIndex | int | Ο δείκτης τμήματος. |
|

**Returns:**
[StopWordDictionary](../../com.groupdocs.search.dictionaries/stopworddictionary) - The dictionary.

### getPasswordDictionary(int shardIndex) {#getPasswordDictionary-int-}
```
public abstract PasswordDictionary getPasswordDictionary(int shardIndex)
```


Λαμβάνει το λεξικό κωδικών.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | shardIndex | int | Ο δείκτης τμήματος. |
|

**Returns:**
[PasswordDictionary](../../com.groupdocs.search.dictionaries/passworddictionary) - The dictionary.

### setDictionary(DictionaryBase dictionary, int shardIndex) {#setDictionary-com.groupdocs.search.dictionaries.DictionaryBase-int-}
```
public abstract void setDictionary(DictionaryBase dictionary, int shardIndex)
```


Ορίζει ένα λεξικό στο καθορισμένο τμήμα.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | dictionary | [DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase) | Το λεξικό. |
|
|  | shardIndex | int | Ο δείκτης τμήματος. |
|

### setDictionary(DictionaryBase dictionary) {#setDictionary-com.groupdocs.search.dictionaries.DictionaryBase-}
```
public abstract void setDictionary(DictionaryBase dictionary)
```


Ορίζει ένα λεξικό σε όλα τα τμήματα.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | dictionary | [DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase) | Το λεξικό. |
|

### deleteAllData() {#deleteAllData--}
```
public abstract void deleteAllData()
```


Διαγράφει όλα τα ευρετηριασμένα δεδομένα από όλα τα τμήματα του δικτύου αναζήτησης.


