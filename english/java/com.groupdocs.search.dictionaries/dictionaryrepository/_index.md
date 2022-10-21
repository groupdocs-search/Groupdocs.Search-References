---
title: DictionaryRepository
second_title: GroupDocs.Search for Java API Reference
description: Represents a repository of all dictionaries in an Index.
type: docs
weight: 16
url: /java/com.groupdocs.search.dictionaries/dictionaryrepository/
---
**Inheritance:**
java.lang.Object
```
public abstract class DictionaryRepository
```

Represents a repository of all dictionaries in an  Index .
## Constructors

| Constructor | Description |
| --- | --- |
| [DictionaryRepository()](#DictionaryRepository--) |  |
## Methods

| Method | Description |
| --- | --- |
| [getAliasDictionary()](#getAliasDictionary--) | Gets a dictionary of aliases. |
| [getStopWordDictionary()](#getStopWordDictionary--) | Gets a dictionary of stop words. |
| [getSynonymDictionary()](#getSynonymDictionary--) | Gets a dictionary of synonyms. |
| [getDocumentPasswords()](#getDocumentPasswords--) | Gets a dictionary of document passwords. |
| [getSpellingCorrector()](#getSpellingCorrector--) | Gets a spelling corrector. |
| [getHomophoneDictionary()](#getHomophoneDictionary--) | Gets a dictionary of homophones. |
| [getAlphabet()](#getAlphabet--) | Gets a dictionary of characters. |
| [getCharacterReplacements()](#getCharacterReplacements--) | Gets a dictionary of character replacements. |
| [getWordFormsProvider()](#getWordFormsProvider--) | Gets a word forms provider. |
| [setWordFormsProvider(IWordFormsProvider value)](#setWordFormsProvider-com.groupdocs.search.dictionaries.IWordFormsProvider-) | Sets a word forms provider. |
### DictionaryRepository() {#DictionaryRepository--}
```
public DictionaryRepository()
```


### getAliasDictionary() {#getAliasDictionary--}
```
public abstract AliasDictionary getAliasDictionary()
```


Gets a dictionary of aliases.

**Returns:**
[AliasDictionary](../../com.groupdocs.search.dictionaries/aliasdictionary) - The dictionary of aliases.
### getStopWordDictionary() {#getStopWordDictionary--}
```
public abstract StopWordDictionary getStopWordDictionary()
```


Gets a dictionary of stop words.

**Returns:**
[StopWordDictionary](../../com.groupdocs.search.dictionaries/stopworddictionary) - The dictionary of stop words.
### getSynonymDictionary() {#getSynonymDictionary--}
```
public abstract SynonymDictionary getSynonymDictionary()
```


Gets a dictionary of synonyms.

**Returns:**
[SynonymDictionary](../../com.groupdocs.search.dictionaries/synonymdictionary) - The dictionary of synonyms.
### getDocumentPasswords() {#getDocumentPasswords--}
```
public abstract PasswordDictionary getDocumentPasswords()
```


Gets a dictionary of document passwords.

**Returns:**
[PasswordDictionary](../../com.groupdocs.search.dictionaries/passworddictionary) - The dictionary of document passwords.
### getSpellingCorrector() {#getSpellingCorrector--}
```
public abstract SpellingCorrector getSpellingCorrector()
```


Gets a spelling corrector.

**Returns:**
[SpellingCorrector](../../com.groupdocs.search.dictionaries/spellingcorrector) - The spelling corrector.
### getHomophoneDictionary() {#getHomophoneDictionary--}
```
public abstract HomophoneDictionary getHomophoneDictionary()
```


Gets a dictionary of homophones.

**Returns:**
[HomophoneDictionary](../../com.groupdocs.search.dictionaries/homophonedictionary) - The dictionary of homophones.
### getAlphabet() {#getAlphabet--}
```
public abstract Alphabet getAlphabet()
```


Gets a dictionary of characters.

**Returns:**
[Alphabet](../../com.groupdocs.search.dictionaries/alphabet) - The dictionary of characters.
### getCharacterReplacements() {#getCharacterReplacements--}
```
public abstract CharacterReplacementDictionary getCharacterReplacements()
```


Gets a dictionary of character replacements.

**Returns:**
[CharacterReplacementDictionary](../../com.groupdocs.search.dictionaries/characterreplacementdictionary) - The dictionary of character replacements.
### getWordFormsProvider() {#getWordFormsProvider--}
```
public abstract IWordFormsProvider getWordFormsProvider()
```


Gets a word forms provider.

**Returns:**
[IWordFormsProvider](../../com.groupdocs.search.dictionaries/iwordformsprovider) - The word forms provider.
### setWordFormsProvider(IWordFormsProvider value) {#setWordFormsProvider-com.groupdocs.search.dictionaries.IWordFormsProvider-}
```
public abstract void setWordFormsProvider(IWordFormsProvider value)
```


Sets a word forms provider.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [IWordFormsProvider](../../com.groupdocs.search.dictionaries/iwordformsprovider) | A word forms provider. |

