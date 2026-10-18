---
title: "DictionaryRepository"
second_title: "GroupDocs.Search για Java API Reference"
description: "Αντιπροσωπεύει μια αποθήκη όλων των λεξικών στο Ευρετήριο."
type: docs
weight: 12
url: /el/java/com.groupdocs.search.dictionaries/dictionaryrepository/
---
**Inheritance:**
java.lang.Object
```
public abstract class DictionaryRepository
```

Αντιπροσωπεύει μια αποθήκη όλων των λεξικών στο Ευρετήριο.

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [DictionaryRepository()](#DictionaryRepository--) |  |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getAliasDictionary()](#getAliasDictionary--) | Λαμβάνει ένα λεξικό ψευδωνύμων. |
|
|  | [getStopWordDictionary()](#getStopWordDictionary--) | Λαμβάνει ένα λεξικό λέξεων-σταματημάτων. |
|
|  | [getSynonymDictionary()](#getSynonymDictionary--) | Λαμβάνει ένα λεξικό συνωνύμων. |
|
|  | [getDocumentPasswords()](#getDocumentPasswords--) | Λαμβάνει ένα λεξικό κωδικών εγγράφων. |
|
|  | [getSpellingCorrector()](#getSpellingCorrector--) | Λαμβάνει έναν διορθωτή ορθογραφίας. |
|
|  | [getHomophoneDictionary()](#getHomophoneDictionary--) | Λαμβάνει ένα λεξικό ομοηχείων. |
|
|  | [getAlphabet()](#getAlphabet--) | Λαμβάνει ένα λεξικό χαρακτήρων. |
|
|  | [getCharacterReplacements()](#getCharacterReplacements--) | Λαμβάνει ένα λεξικό αντικαταστάσεων χαρακτήρων. |
|
|  | [getWordFormsProvider()](#getWordFormsProvider--) | Λαμβάνει έναν πάροχο μορφών λέξεων. |
|
|  | [setWordFormsProvider(IWordFormsProvider value)](#setWordFormsProvider-com.groupdocs.search.dictionaries.IWordFormsProvider-) | Ορίζει έναν πάροχο μορφών λέξεων. |
|
### DictionaryRepository() {#DictionaryRepository--}
```
public DictionaryRepository()
```


### getAliasDictionary() {#getAliasDictionary--}
```
public abstract AliasDictionary getAliasDictionary()
```


Λαμβάνει ένα λεξικό ψευδωνύμων.


**Returns:**
[AliasDictionary](../../com.groupdocs.search.dictionaries/aliasdictionary) - The dictionary of aliases.

### getStopWordDictionary() {#getStopWordDictionary--}
```
public abstract StopWordDictionary getStopWordDictionary()
```


Λαμβάνει ένα λεξικό λέξεων-σταματημάτων.


**Returns:**
[StopWordDictionary](../../com.groupdocs.search.dictionaries/stopworddictionary) - The dictionary of stop words.

### getSynonymDictionary() {#getSynonymDictionary--}
```
public abstract SynonymDictionary getSynonymDictionary()
```


Λαμβάνει ένα λεξικό συνωνύμων.


**Returns:**
[SynonymDictionary](../../com.groupdocs.search.dictionaries/synonymdictionary) - The dictionary of synonyms.

### getDocumentPasswords() {#getDocumentPasswords--}
```
public abstract PasswordDictionary getDocumentPasswords()
```


Λαμβάνει ένα λεξικό κωδικών εγγράφων.


**Returns:**
[PasswordDictionary](../../com.groupdocs.search.dictionaries/passworddictionary) - The dictionary of document passwords.

### getSpellingCorrector() {#getSpellingCorrector--}
```
public abstract SpellingCorrector getSpellingCorrector()
```


Λαμβάνει έναν διορθωτή ορθογραφίας.


**Returns:**
[SpellingCorrector](../../com.groupdocs.search.dictionaries/spellingcorrector) - The spelling corrector.

### getHomophoneDictionary() {#getHomophoneDictionary--}
```
public abstract HomophoneDictionary getHomophoneDictionary()
```


Λαμβάνει ένα λεξικό ομοηχείων.


**Returns:**
[HomophoneDictionary](../../com.groupdocs.search.dictionaries/homophonedictionary) - The dictionary of homophones.

### getAlphabet() {#getAlphabet--}
```
public abstract Alphabet getAlphabet()
```


Λαμβάνει ένα λεξικό χαρακτήρων.


**Returns:**
[Alphabet](../../com.groupdocs.search.dictionaries/alphabet) - The dictionary of characters.

### getCharacterReplacements() {#getCharacterReplacements--}
```
public abstract CharacterReplacementDictionary getCharacterReplacements()
```


Λαμβάνει ένα λεξικό αντικαταστάσεων χαρακτήρων.


**Returns:**
[CharacterReplacementDictionary](../../com.groupdocs.search.dictionaries/characterreplacementdictionary) - The dictionary of character replacements.

### getWordFormsProvider() {#getWordFormsProvider--}
```
public abstract IWordFormsProvider getWordFormsProvider()
```


Λαμβάνει έναν πάροχο μορφών λέξεων.


**Returns:**
[IWordFormsProvider](../../com.groupdocs.search.dictionaries/iwordformsprovider) - The word forms provider.

### setWordFormsProvider(IWordFormsProvider value) {#setWordFormsProvider-com.groupdocs.search.dictionaries.IWordFormsProvider-}
```
public abstract void setWordFormsProvider(IWordFormsProvider value)
```


Ορίζει έναν πάροχο μορφών λέξεων.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | value | [IWordFormsProvider](../../com.groupdocs.search.dictionaries/iwordformsprovider) | Ένας πάροχος μορφών λέξεων. |
|

