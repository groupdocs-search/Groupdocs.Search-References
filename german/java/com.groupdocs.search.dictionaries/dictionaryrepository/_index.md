---
title: "DictionaryRepository"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Stellt ein Repository aller Wörterbücher im Index dar."
type: docs
weight: 12
url: /de/java/com.groupdocs.search.dictionaries/dictionaryrepository/
---
**Inheritance:**
java.lang.Object
```
public abstract class DictionaryRepository
```

Stellt ein Repository aller Wörterbücher im Index dar.

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [DictionaryRepository()](#DictionaryRepository--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getAliasDictionary()](#getAliasDictionary--) | Gibt ein Wörterbuch der Aliase zurück. |
|
|  | [getStopWordDictionary()](#getStopWordDictionary--) | Gibt ein Wörterbuch von Stoppwörtern zurück. |
|
|  | [getSynonymDictionary()](#getSynonymDictionary--) | Gibt ein Wörterbuch von Synonymen zurück. |
|
|  | [getDocumentPasswords()](#getDocumentPasswords--) | Gibt ein Wörterbuch von Dokumentenpasswörtern zurück. |
|
|  | [getSpellingCorrector()](#getSpellingCorrector--) | Gibt einen Rechtschreibkorrektor zurück. |
|
|  | [getHomophoneDictionary()](#getHomophoneDictionary--) | Gibt ein Wörterbuch von Homophonen zurück. |
|
|  | [getAlphabet()](#getAlphabet--) | Gibt ein Wörterbuch von Zeichen zurück. |
|
|  | [getCharacterReplacements()](#getCharacterReplacements--) | Gibt ein Wörterbuch von Zeichenersetzungen zurück. |
|
|  | [getWordFormsProvider()](#getWordFormsProvider--) | Gibt einen Wortformen‑Provider zurück. |
|
|  | [setWordFormsProvider(IWordFormsProvider value)](#setWordFormsProvider-com.groupdocs.search.dictionaries.IWordFormsProvider-) | Setzt einen Wortformen‑Provider. |
|
### DictionaryRepository() {#DictionaryRepository--}
```
public DictionaryRepository()
```


### getAliasDictionary() {#getAliasDictionary--}
```
public abstract AliasDictionary getAliasDictionary()
```


Gibt ein Wörterbuch der Aliase zurück.


**Returns:**
[AliasDictionary](../../com.groupdocs.search.dictionaries/aliasdictionary) - The dictionary of aliases.

### getStopWordDictionary() {#getStopWordDictionary--}
```
public abstract StopWordDictionary getStopWordDictionary()
```


Gibt ein Wörterbuch von Stoppwörtern zurück.


**Returns:**
[StopWordDictionary](../../com.groupdocs.search.dictionaries/stopworddictionary) - The dictionary of stop words.

### getSynonymDictionary() {#getSynonymDictionary--}
```
public abstract SynonymDictionary getSynonymDictionary()
```


Gibt ein Wörterbuch von Synonymen zurück.


**Returns:**
[SynonymDictionary](../../com.groupdocs.search.dictionaries/synonymdictionary) - The dictionary of synonyms.

### getDocumentPasswords() {#getDocumentPasswords--}
```
public abstract PasswordDictionary getDocumentPasswords()
```


Gibt ein Wörterbuch von Dokumentenpasswörtern zurück.


**Returns:**
[PasswordDictionary](../../com.groupdocs.search.dictionaries/passworddictionary) - The dictionary of document passwords.

### getSpellingCorrector() {#getSpellingCorrector--}
```
public abstract SpellingCorrector getSpellingCorrector()
```


Gibt einen Rechtschreibkorrektor zurück.


**Returns:**
[SpellingCorrector](../../com.groupdocs.search.dictionaries/spellingcorrector) - The spelling corrector.

### getHomophoneDictionary() {#getHomophoneDictionary--}
```
public abstract HomophoneDictionary getHomophoneDictionary()
```


Gibt ein Wörterbuch von Homophonen zurück.


**Returns:**
[HomophoneDictionary](../../com.groupdocs.search.dictionaries/homophonedictionary) - The dictionary of homophones.

### getAlphabet() {#getAlphabet--}
```
public abstract Alphabet getAlphabet()
```


Gibt ein Wörterbuch von Zeichen zurück.


**Returns:**
[Alphabet](../../com.groupdocs.search.dictionaries/alphabet) - The dictionary of characters.

### getCharacterReplacements() {#getCharacterReplacements--}
```
public abstract CharacterReplacementDictionary getCharacterReplacements()
```


Gibt ein Wörterbuch von Zeichenersetzungen zurück.


**Returns:**
[CharacterReplacementDictionary](../../com.groupdocs.search.dictionaries/characterreplacementdictionary) - The dictionary of character replacements.

### getWordFormsProvider() {#getWordFormsProvider--}
```
public abstract IWordFormsProvider getWordFormsProvider()
```


Gibt einen Wortformen‑Provider zurück.


**Returns:**
[IWordFormsProvider](../../com.groupdocs.search.dictionaries/iwordformsprovider) - The word forms provider.

### setWordFormsProvider(IWordFormsProvider value) {#setWordFormsProvider-com.groupdocs.search.dictionaries.IWordFormsProvider-}
```
public abstract void setWordFormsProvider(IWordFormsProvider value)
```


Setzt einen Wortformen‑Provider.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | value | [IWordFormsProvider](../../com.groupdocs.search.dictionaries/iwordformsprovider) | Ein Wortformen‑Provider. |
|

