---
title: "DictionaryRepository"
second_title: "GroupDocs.Search för Java API-referens"
description: "Representerar ett arkiv för alla ordböcker i Indexet."
type: docs
weight: 12
url: /sv/java/com.groupdocs.search.dictionaries/dictionaryrepository/
---
**Inheritance:**
java.lang.Object
```
public abstract class DictionaryRepository
```

Representerar ett arkiv för alla ordböcker i indexet.

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [DictionaryRepository()](#DictionaryRepository--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getAliasDictionary()](#getAliasDictionary--) | Hämtar en ordbok med alias. |
|
|  | [getStopWordDictionary()](#getStopWordDictionary--) | Hämtar en ordbok med stoppord. |
|
|  | [getSynonymDictionary()](#getSynonymDictionary--) | Hämtar en ordbok med synonymer. |
|
|  | [getDocumentPasswords()](#getDocumentPasswords--) | Hämtar en ordbok med dokumentlösenord. |
|
|  | [getSpellingCorrector()](#getSpellingCorrector--) | Hämtar en stavningskorrigerare. |
|
|  | [getHomophoneDictionary()](#getHomophoneDictionary--) | Hämtar en ordbok med homofoner. |
|
|  | [getAlphabet()](#getAlphabet--) | Hämtar en ordbok med tecken. |
|
|  | [getCharacterReplacements()](#getCharacterReplacements--) | Hämtar en ordbok med teckenersättningar. |
|
|  | [getWordFormsProvider()](#getWordFormsProvider--) | Hämtar en leverantör av ordformer. |
|
|  | [setWordFormsProvider(IWordFormsProvider value)](#setWordFormsProvider-com.groupdocs.search.dictionaries.IWordFormsProvider-) | Ställer in en leverantör av ordformer. |
|
### DictionaryRepository() {#DictionaryRepository--}
```
public DictionaryRepository()
```


### getAliasDictionary() {#getAliasDictionary--}
```
public abstract AliasDictionary getAliasDictionary()
```


Hämtar en ordbok med alias.


**Returns:**
[AliasDictionary](../../com.groupdocs.search.dictionaries/aliasdictionary) - The dictionary of aliases.

### getStopWordDictionary() {#getStopWordDictionary--}
```
public abstract StopWordDictionary getStopWordDictionary()
```


Hämtar en ordbok med stoppord.


**Returns:**
[StopWordDictionary](../../com.groupdocs.search.dictionaries/stopworddictionary) - The dictionary of stop words.

### getSynonymDictionary() {#getSynonymDictionary--}
```
public abstract SynonymDictionary getSynonymDictionary()
```


Hämtar en ordbok med synonymer.


**Returns:**
[SynonymDictionary](../../com.groupdocs.search.dictionaries/synonymdictionary) - The dictionary of synonyms.

### getDocumentPasswords() {#getDocumentPasswords--}
```
public abstract PasswordDictionary getDocumentPasswords()
```


Hämtar en ordbok med dokumentlösenord.


**Returns:**
[PasswordDictionary](../../com.groupdocs.search.dictionaries/passworddictionary) - The dictionary of document passwords.

### getSpellingCorrector() {#getSpellingCorrector--}
```
public abstract SpellingCorrector getSpellingCorrector()
```


Hämtar en stavningskorrigerare.


**Returns:**
[SpellingCorrector](../../com.groupdocs.search.dictionaries/spellingcorrector) - The spelling corrector.

### getHomophoneDictionary() {#getHomophoneDictionary--}
```
public abstract HomophoneDictionary getHomophoneDictionary()
```


Hämtar en ordbok med homofoner.


**Returns:**
[HomophoneDictionary](../../com.groupdocs.search.dictionaries/homophonedictionary) - The dictionary of homophones.

### getAlphabet() {#getAlphabet--}
```
public abstract Alphabet getAlphabet()
```


Hämtar en ordbok med tecken.


**Returns:**
[Alphabet](../../com.groupdocs.search.dictionaries/alphabet) - The dictionary of characters.

### getCharacterReplacements() {#getCharacterReplacements--}
```
public abstract CharacterReplacementDictionary getCharacterReplacements()
```


Hämtar en ordbok med teckenersättningar.


**Returns:**
[CharacterReplacementDictionary](../../com.groupdocs.search.dictionaries/characterreplacementdictionary) - The dictionary of character replacements.

### getWordFormsProvider() {#getWordFormsProvider--}
```
public abstract IWordFormsProvider getWordFormsProvider()
```


Hämtar en leverantör av ordformer.


**Returns:**
[IWordFormsProvider](../../com.groupdocs.search.dictionaries/iwordformsprovider) - The word forms provider.

### setWordFormsProvider(IWordFormsProvider value) {#setWordFormsProvider-com.groupdocs.search.dictionaries.IWordFormsProvider-}
```
public abstract void setWordFormsProvider(IWordFormsProvider value)
```


Ställer in en leverantör av ordformer.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | value | [IWordFormsProvider](../../com.groupdocs.search.dictionaries/iwordformsprovider) | En leverantör av ordformer. |
|

