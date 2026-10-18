---
title: "DictionaryRepository"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Mewakili repositori semua kamus dalam Indeks."
type: docs
weight: 12
url: /id/java/com.groupdocs.search.dictionaries/dictionaryrepository/
---
**Inheritance:**
java.lang.Object
```
public abstract class DictionaryRepository
```

Mewakili repositori semua kamus dalam Indeks.

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [DictionaryRepository()](#DictionaryRepository--) |  |
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getAliasDictionary()](#getAliasDictionary--) | Mendapatkan kamus alias. |
|
|  | [getStopWordDictionary()](#getStopWordDictionary--) | Mendapatkan kamus kata henti. |
|
|  | [getSynonymDictionary()](#getSynonymDictionary--) | Mendapatkan kamus sinonim. |
|
|  | [getDocumentPasswords()](#getDocumentPasswords--) | Mendapatkan kamus kata sandi dokumen. |
|
|  | [getSpellingCorrector()](#getSpellingCorrector--) | Mendapatkan korektor ejaan. |
|
|  | [getHomophoneDictionary()](#getHomophoneDictionary--) | Mendapatkan kamus homofon. |
|
|  | [getAlphabet()](#getAlphabet--) | Mendapatkan kamus karakter. |
|
|  | [getCharacterReplacements()](#getCharacterReplacements--) | Mendapatkan kamus penggantian karakter. |
|
|  | [getWordFormsProvider()](#getWordFormsProvider--) | Mendapatkan penyedia bentuk kata. |
|
|  | [setWordFormsProvider(IWordFormsProvider value)](#setWordFormsProvider-com.groupdocs.search.dictionaries.IWordFormsProvider-) | Mengatur penyedia bentuk kata. |
|
### DictionaryRepository() {#DictionaryRepository--}
```
public DictionaryRepository()
```


### getAliasDictionary() {#getAliasDictionary--}
```
public abstract AliasDictionary getAliasDictionary()
```


Mendapatkan kamus alias.


**Returns:**
[AliasDictionary](../../com.groupdocs.search.dictionaries/aliasdictionary) - The dictionary of aliases.

### getStopWordDictionary() {#getStopWordDictionary--}
```
public abstract StopWordDictionary getStopWordDictionary()
```


Mendapatkan kamus kata henti.


**Returns:**
[StopWordDictionary](../../com.groupdocs.search.dictionaries/stopworddictionary) - The dictionary of stop words.

### getSynonymDictionary() {#getSynonymDictionary--}
```
public abstract SynonymDictionary getSynonymDictionary()
```


Mendapatkan kamus sinonim.


**Returns:**
[SynonymDictionary](../../com.groupdocs.search.dictionaries/synonymdictionary) - The dictionary of synonyms.

### getDocumentPasswords() {#getDocumentPasswords--}
```
public abstract PasswordDictionary getDocumentPasswords()
```


Mendapatkan kamus kata sandi dokumen.


**Returns:**
[PasswordDictionary](../../com.groupdocs.search.dictionaries/passworddictionary) - The dictionary of document passwords.

### getSpellingCorrector() {#getSpellingCorrector--}
```
public abstract SpellingCorrector getSpellingCorrector()
```


Mendapatkan korektor ejaan.


**Returns:**
[SpellingCorrector](../../com.groupdocs.search.dictionaries/spellingcorrector) - The spelling corrector.

### getHomophoneDictionary() {#getHomophoneDictionary--}
```
public abstract HomophoneDictionary getHomophoneDictionary()
```


Mendapatkan kamus homofon.


**Returns:**
[HomophoneDictionary](../../com.groupdocs.search.dictionaries/homophonedictionary) - The dictionary of homophones.

### getAlphabet() {#getAlphabet--}
```
public abstract Alphabet getAlphabet()
```


Mendapatkan kamus karakter.


**Returns:**
[Alphabet](../../com.groupdocs.search.dictionaries/alphabet) - The dictionary of characters.

### getCharacterReplacements() {#getCharacterReplacements--}
```
public abstract CharacterReplacementDictionary getCharacterReplacements()
```


Mendapatkan kamus penggantian karakter.


**Returns:**
[CharacterReplacementDictionary](../../com.groupdocs.search.dictionaries/characterreplacementdictionary) - The dictionary of character replacements.

### getWordFormsProvider() {#getWordFormsProvider--}
```
public abstract IWordFormsProvider getWordFormsProvider()
```


Mendapatkan penyedia bentuk kata.


**Returns:**
[IWordFormsProvider](../../com.groupdocs.search.dictionaries/iwordformsprovider) - The word forms provider.

### setWordFormsProvider(IWordFormsProvider value) {#setWordFormsProvider-com.groupdocs.search.dictionaries.IWordFormsProvider-}
```
public abstract void setWordFormsProvider(IWordFormsProvider value)
```


Mengatur penyedia bentuk kata.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | value | [IWordFormsProvider](../../com.groupdocs.search.dictionaries/iwordformsprovider) | Penyedia bentuk kata. |
|

