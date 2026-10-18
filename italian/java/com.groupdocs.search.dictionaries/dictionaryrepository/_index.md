---
title: "DictionaryRepository"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Rappresenta un repository di tutti i dizionari nell'Index."
type: docs
weight: 12
url: /it/java/com.groupdocs.search.dictionaries/dictionaryrepository/
---
**Inheritance:**
java.lang.Object
```
public abstract class DictionaryRepository
```

Rappresenta un repository di tutti i dizionari nell'Indice.

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [DictionaryRepository()](#DictionaryRepository--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getAliasDictionary()](#getAliasDictionary--) | Restituisce un dizionario di alias. |
|
|  | [getStopWordDictionary()](#getStopWordDictionary--) | Restituisce un dizionario di parole di stop. |
|
|  | [getSynonymDictionary()](#getSynonymDictionary--) | Restituisce un dizionario di sinonimi. |
|
|  | [getDocumentPasswords()](#getDocumentPasswords--) | Restituisce un dizionario di password dei documenti. |
|
|  | [getSpellingCorrector()](#getSpellingCorrector--) | Restituisce un correttore ortografico. |
|
|  | [getHomophoneDictionary()](#getHomophoneDictionary--) | Restituisce un dizionario di omofoni. |
|
|  | [getAlphabet()](#getAlphabet--) | Restituisce un dizionario di caratteri. |
|
|  | [getCharacterReplacements()](#getCharacterReplacements--) | Restituisce un dizionario di sostituzioni di caratteri. |
|
|  | [getWordFormsProvider()](#getWordFormsProvider--) | Restituisce un provider di forme di parole. |
|
|  | [setWordFormsProvider(IWordFormsProvider value)](#setWordFormsProvider-com.groupdocs.search.dictionaries.IWordFormsProvider-) | Imposta un provider di forme di parole. |
|
### DictionaryRepository() {#DictionaryRepository--}
```
public DictionaryRepository()
```


### getAliasDictionary() {#getAliasDictionary--}
```
public abstract AliasDictionary getAliasDictionary()
```


Restituisce un dizionario di alias.


**Returns:**
[AliasDictionary](../../com.groupdocs.search.dictionaries/aliasdictionary) - The dictionary of aliases.

### getStopWordDictionary() {#getStopWordDictionary--}
```
public abstract StopWordDictionary getStopWordDictionary()
```


Restituisce un dizionario di parole di stop.


**Returns:**
[StopWordDictionary](../../com.groupdocs.search.dictionaries/stopworddictionary) - The dictionary of stop words.

### getSynonymDictionary() {#getSynonymDictionary--}
```
public abstract SynonymDictionary getSynonymDictionary()
```


Restituisce un dizionario di sinonimi.


**Returns:**
[SynonymDictionary](../../com.groupdocs.search.dictionaries/synonymdictionary) - The dictionary of synonyms.

### getDocumentPasswords() {#getDocumentPasswords--}
```
public abstract PasswordDictionary getDocumentPasswords()
```


Restituisce un dizionario di password dei documenti.


**Returns:**
[PasswordDictionary](../../com.groupdocs.search.dictionaries/passworddictionary) - The dictionary of document passwords.

### getSpellingCorrector() {#getSpellingCorrector--}
```
public abstract SpellingCorrector getSpellingCorrector()
```


Restituisce un correttore ortografico.


**Returns:**
[SpellingCorrector](../../com.groupdocs.search.dictionaries/spellingcorrector) - The spelling corrector.

### getHomophoneDictionary() {#getHomophoneDictionary--}
```
public abstract HomophoneDictionary getHomophoneDictionary()
```


Restituisce un dizionario di omofoni.


**Returns:**
[HomophoneDictionary](../../com.groupdocs.search.dictionaries/homophonedictionary) - The dictionary of homophones.

### getAlphabet() {#getAlphabet--}
```
public abstract Alphabet getAlphabet()
```


Restituisce un dizionario di caratteri.


**Returns:**
[Alphabet](../../com.groupdocs.search.dictionaries/alphabet) - The dictionary of characters.

### getCharacterReplacements() {#getCharacterReplacements--}
```
public abstract CharacterReplacementDictionary getCharacterReplacements()
```


Restituisce un dizionario di sostituzioni di caratteri.


**Returns:**
[CharacterReplacementDictionary](../../com.groupdocs.search.dictionaries/characterreplacementdictionary) - The dictionary of character replacements.

### getWordFormsProvider() {#getWordFormsProvider--}
```
public abstract IWordFormsProvider getWordFormsProvider()
```


Restituisce un provider di forme di parole.


**Returns:**
[IWordFormsProvider](../../com.groupdocs.search.dictionaries/iwordformsprovider) - The word forms provider.

### setWordFormsProvider(IWordFormsProvider value) {#setWordFormsProvider-com.groupdocs.search.dictionaries.IWordFormsProvider-}
```
public abstract void setWordFormsProvider(IWordFormsProvider value)
```


Imposta un provider di forme di parole.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | value | [IWordFormsProvider](../../com.groupdocs.search.dictionaries/iwordformsprovider) | Un provider di forme di parole. |
|

