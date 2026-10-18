---
title: "DictionaryRepository"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Stelt een repository voor van alle woordenboeken in de Index."
type: docs
weight: 12
url: /nl/java/com.groupdocs.search.dictionaries/dictionaryrepository/
---
**Inheritance:**
java.lang.Object
```
public abstract class DictionaryRepository
```

Stelt een opslagplaats van alle woordenboeken in de Index voor.

## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [DictionaryRepository()](#DictionaryRepository--) |  |
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getAliasDictionary()](#getAliasDictionary--) | Haalt een woordenboek met aliassen op. |
|
|  | [getStopWordDictionary()](#getStopWordDictionary--) | Haalt een woordenboek met stopwoorden op. |
|
|  | [getSynonymDictionary()](#getSynonymDictionary--) | Haalt een woordenboek met synoniemen op. |
|
|  | [getDocumentPasswords()](#getDocumentPasswords--) | Haalt een woordenboek met documentwachtwoorden op. |
|
|  | [getSpellingCorrector()](#getSpellingCorrector--) | Haalt een spellingcorrector op. |
|
|  | [getHomophoneDictionary()](#getHomophoneDictionary--) | Haalt een woordenboek met homofonen op. |
|
|  | [getAlphabet()](#getAlphabet--) | Haalt een woordenboek met tekens op. |
|
|  | [getCharacterReplacements()](#getCharacterReplacements--) | Haalt een woordenboek met tekenvervangingen op. |
|
|  | [getWordFormsProvider()](#getWordFormsProvider--) | Haalt een provider voor woordvormen op. |
|
|  | [setWordFormsProvider(IWordFormsProvider value)](#setWordFormsProvider-com.groupdocs.search.dictionaries.IWordFormsProvider-) | Stelt een provider voor woordvormen in. |
|
### DictionaryRepository() {#DictionaryRepository--}
```
public DictionaryRepository()
```


### getAliasDictionary() {#getAliasDictionary--}
```
public abstract AliasDictionary getAliasDictionary()
```


Haalt een woordenboek met aliassen op.


**Returns:**
[AliasDictionary](../../com.groupdocs.search.dictionaries/aliasdictionary) - The dictionary of aliases.

### getStopWordDictionary() {#getStopWordDictionary--}
```
public abstract StopWordDictionary getStopWordDictionary()
```


Haalt een woordenboek met stopwoorden op.


**Returns:**
[StopWordDictionary](../../com.groupdocs.search.dictionaries/stopworddictionary) - The dictionary of stop words.

### getSynonymDictionary() {#getSynonymDictionary--}
```
public abstract SynonymDictionary getSynonymDictionary()
```


Haalt een woordenboek met synoniemen op.


**Returns:**
[SynonymDictionary](../../com.groupdocs.search.dictionaries/synonymdictionary) - The dictionary of synonyms.

### getDocumentPasswords() {#getDocumentPasswords--}
```
public abstract PasswordDictionary getDocumentPasswords()
```


Haalt een woordenboek met documentwachtwoorden op.


**Returns:**
[PasswordDictionary](../../com.groupdocs.search.dictionaries/passworddictionary) - The dictionary of document passwords.

### getSpellingCorrector() {#getSpellingCorrector--}
```
public abstract SpellingCorrector getSpellingCorrector()
```


Haalt een spellingcorrector op.


**Returns:**
[SpellingCorrector](../../com.groupdocs.search.dictionaries/spellingcorrector) - The spelling corrector.

### getHomophoneDictionary() {#getHomophoneDictionary--}
```
public abstract HomophoneDictionary getHomophoneDictionary()
```


Haalt een woordenboek met homofonen op.


**Returns:**
[HomophoneDictionary](../../com.groupdocs.search.dictionaries/homophonedictionary) - The dictionary of homophones.

### getAlphabet() {#getAlphabet--}
```
public abstract Alphabet getAlphabet()
```


Haalt een woordenboek met tekens op.


**Returns:**
[Alphabet](../../com.groupdocs.search.dictionaries/alphabet) - The dictionary of characters.

### getCharacterReplacements() {#getCharacterReplacements--}
```
public abstract CharacterReplacementDictionary getCharacterReplacements()
```


Haalt een woordenboek met tekenvervangingen op.


**Returns:**
[CharacterReplacementDictionary](../../com.groupdocs.search.dictionaries/characterreplacementdictionary) - The dictionary of character replacements.

### getWordFormsProvider() {#getWordFormsProvider--}
```
public abstract IWordFormsProvider getWordFormsProvider()
```


Haalt een provider voor woordvormen op.


**Returns:**
[IWordFormsProvider](../../com.groupdocs.search.dictionaries/iwordformsprovider) - The word forms provider.

### setWordFormsProvider(IWordFormsProvider value) {#setWordFormsProvider-com.groupdocs.search.dictionaries.IWordFormsProvider-}
```
public abstract void setWordFormsProvider(IWordFormsProvider value)
```


Stelt een provider voor woordvormen in.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | value | [IWordFormsProvider](../../com.groupdocs.search.dictionaries/iwordformsprovider) | Een provider voor woordvormen. |
|

