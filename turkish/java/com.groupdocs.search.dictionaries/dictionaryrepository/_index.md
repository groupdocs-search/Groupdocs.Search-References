---
title: "DictionaryRepository"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Dizin'deki tüm sözlüklerin bir deposunu temsil eder."
type: docs
weight: 12
url: /tr/java/com.groupdocs.search.dictionaries/dictionaryrepository/
---
**Inheritance:**
java.lang.Object
```
public abstract class DictionaryRepository
```

İndeksteki tüm sözlüklerin deposunu temsil eder.

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [DictionaryRepository()](#DictionaryRepository--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getAliasDictionary()](#getAliasDictionary--) | Takma adların bir sözlüğünü alır. |
|
|  | [getStopWordDictionary()](#getStopWordDictionary--) | Durma kelimelerinin bir sözlüğünü alır. |
|
|  | [getSynonymDictionary()](#getSynonymDictionary--) | Eşanlamlıların bir sözlüğünü alır. |
|
|  | [getDocumentPasswords()](#getDocumentPasswords--) | Belge şifrelerinin bir sözlüğünü alır. |
|
|  | [getSpellingCorrector()](#getSpellingCorrector--) | Yazım düzelticiyi alır. |
|
|  | [getHomophoneDictionary()](#getHomophoneDictionary--) | Eşsesli kelimelerin bir sözlüğünü alır. |
|
|  | [getAlphabet()](#getAlphabet--) | Karakterlerin bir sözlüğünü alır. |
|
|  | [getCharacterReplacements()](#getCharacterReplacements--) | Karakter değişimlerinin bir sözlüğünü alır. |
|
|  | [getWordFormsProvider()](#getWordFormsProvider--) | Kelime biçimleri sağlayıcısını alır. |
|
|  | [setWordFormsProvider(IWordFormsProvider value)](#setWordFormsProvider-com.groupdocs.search.dictionaries.IWordFormsProvider-) | Kelime biçimleri sağlayıcısını ayarlar. |
|
### DictionaryRepository() {#DictionaryRepository--}
```
public DictionaryRepository()
```


### getAliasDictionary() {#getAliasDictionary--}
```
public abstract AliasDictionary getAliasDictionary()
```


Takma adların bir sözlüğünü alır.


**Returns:**
[AliasDictionary](../../com.groupdocs.search.dictionaries/aliasdictionary) - The dictionary of aliases.

### getStopWordDictionary() {#getStopWordDictionary--}
```
public abstract StopWordDictionary getStopWordDictionary()
```


Durma kelimelerinin bir sözlüğünü alır.


**Returns:**
[StopWordDictionary](../../com.groupdocs.search.dictionaries/stopworddictionary) - The dictionary of stop words.

### getSynonymDictionary() {#getSynonymDictionary--}
```
public abstract SynonymDictionary getSynonymDictionary()
```


Eşanlamlıların bir sözlüğünü alır.


**Returns:**
[SynonymDictionary](../../com.groupdocs.search.dictionaries/synonymdictionary) - The dictionary of synonyms.

### getDocumentPasswords() {#getDocumentPasswords--}
```
public abstract PasswordDictionary getDocumentPasswords()
```


Belge şifrelerinin bir sözlüğünü alır.


**Returns:**
[PasswordDictionary](../../com.groupdocs.search.dictionaries/passworddictionary) - The dictionary of document passwords.

### getSpellingCorrector() {#getSpellingCorrector--}
```
public abstract SpellingCorrector getSpellingCorrector()
```


Yazım düzelticiyi alır.


**Returns:**
[SpellingCorrector](../../com.groupdocs.search.dictionaries/spellingcorrector) - The spelling corrector.

### getHomophoneDictionary() {#getHomophoneDictionary--}
```
public abstract HomophoneDictionary getHomophoneDictionary()
```


Eşsesli kelimelerin bir sözlüğünü alır.


**Returns:**
[HomophoneDictionary](../../com.groupdocs.search.dictionaries/homophonedictionary) - The dictionary of homophones.

### getAlphabet() {#getAlphabet--}
```
public abstract Alphabet getAlphabet()
```


Karakterlerin bir sözlüğünü alır.


**Returns:**
[Alphabet](../../com.groupdocs.search.dictionaries/alphabet) - The dictionary of characters.

### getCharacterReplacements() {#getCharacterReplacements--}
```
public abstract CharacterReplacementDictionary getCharacterReplacements()
```


Karakter değişimlerinin bir sözlüğünü alır.


**Returns:**
[CharacterReplacementDictionary](../../com.groupdocs.search.dictionaries/characterreplacementdictionary) - The dictionary of character replacements.

### getWordFormsProvider() {#getWordFormsProvider--}
```
public abstract IWordFormsProvider getWordFormsProvider()
```


Kelime biçimleri sağlayıcısını alır.


**Returns:**
[IWordFormsProvider](../../com.groupdocs.search.dictionaries/iwordformsprovider) - The word forms provider.

### setWordFormsProvider(IWordFormsProvider value) {#setWordFormsProvider-com.groupdocs.search.dictionaries.IWordFormsProvider-}
```
public abstract void setWordFormsProvider(IWordFormsProvider value)
```


Kelime biçimleri sağlayıcısını ayarlar.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | value | [IWordFormsProvider](../../com.groupdocs.search.dictionaries/iwordformsprovider) | Bir kelime biçimleri sağlayıcısı. |
|

