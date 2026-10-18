---
title: "DictionaryRepository"
second_title: "GroupDocs.Search для Java API Reference"
description: "Представляет репозиторий всех словарей в индексе."
type: docs
weight: 12
url: /ru/java/com.groupdocs.search.dictionaries/dictionaryrepository/
---
**Inheritance:**
java.lang.Object
```
public abstract class DictionaryRepository
```

Представляет репозиторий всех словарей в индексе.

## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [DictionaryRepository()](#DictionaryRepository--) |  |
## Методы

| Метод | Описание |
| --- | --- |
|  | [getAliasDictionary()](#getAliasDictionary--) | Получает словарь псевдонимов. |
|
|  | [getStopWordDictionary()](#getStopWordDictionary--) | Получает словарь стоп-слов. |
|
|  | [getSynonymDictionary()](#getSynonymDictionary--) | Получает словарь синонимов. |
|
|  | [getDocumentPasswords()](#getDocumentPasswords--) | Получает словарь паролей документов. |
|
|  | [getSpellingCorrector()](#getSpellingCorrector--) | Получает корректор орфографии. |
|
|  | [getHomophoneDictionary()](#getHomophoneDictionary--) | Получает словарь омонимов. |
|
|  | [getAlphabet()](#getAlphabet--) | Получает словарь символов. |
|
|  | [getCharacterReplacements()](#getCharacterReplacements--) | Получает словарь замен символов. |
|
|  | [getWordFormsProvider()](#getWordFormsProvider--) | Получает поставщик форм слов. |
|
|  | [setWordFormsProvider(IWordFormsProvider value)](#setWordFormsProvider-com.groupdocs.search.dictionaries.IWordFormsProvider-) | Устанавливает поставщик форм слов. |
|
### DictionaryRepository() {#DictionaryRepository--}
```
public DictionaryRepository()
```


### getAliasDictionary() {#getAliasDictionary--}
```
public abstract AliasDictionary getAliasDictionary()
```


Получает словарь псевдонимов.


**Returns:**
[AliasDictionary](../../com.groupdocs.search.dictionaries/aliasdictionary) - The dictionary of aliases.

### getStopWordDictionary() {#getStopWordDictionary--}
```
public abstract StopWordDictionary getStopWordDictionary()
```


Получает словарь стоп-слов.


**Returns:**
[StopWordDictionary](../../com.groupdocs.search.dictionaries/stopworddictionary) - The dictionary of stop words.

### getSynonymDictionary() {#getSynonymDictionary--}
```
public abstract SynonymDictionary getSynonymDictionary()
```


Получает словарь синонимов.


**Returns:**
[SynonymDictionary](../../com.groupdocs.search.dictionaries/synonymdictionary) - The dictionary of synonyms.

### getDocumentPasswords() {#getDocumentPasswords--}
```
public abstract PasswordDictionary getDocumentPasswords()
```


Получает словарь паролей документов.


**Returns:**
[PasswordDictionary](../../com.groupdocs.search.dictionaries/passworddictionary) - The dictionary of document passwords.

### getSpellingCorrector() {#getSpellingCorrector--}
```
public abstract SpellingCorrector getSpellingCorrector()
```


Получает корректор орфографии.


**Returns:**
[SpellingCorrector](../../com.groupdocs.search.dictionaries/spellingcorrector) - The spelling corrector.

### getHomophoneDictionary() {#getHomophoneDictionary--}
```
public abstract HomophoneDictionary getHomophoneDictionary()
```


Получает словарь омонимов.


**Returns:**
[HomophoneDictionary](../../com.groupdocs.search.dictionaries/homophonedictionary) - The dictionary of homophones.

### getAlphabet() {#getAlphabet--}
```
public abstract Alphabet getAlphabet()
```


Получает словарь символов.


**Returns:**
[Alphabet](../../com.groupdocs.search.dictionaries/alphabet) - The dictionary of characters.

### getCharacterReplacements() {#getCharacterReplacements--}
```
public abstract CharacterReplacementDictionary getCharacterReplacements()
```


Получает словарь замен символов.


**Returns:**
[CharacterReplacementDictionary](../../com.groupdocs.search.dictionaries/characterreplacementdictionary) - The dictionary of character replacements.

### getWordFormsProvider() {#getWordFormsProvider--}
```
public abstract IWordFormsProvider getWordFormsProvider()
```


Получает поставщик форм слов.


**Returns:**
[IWordFormsProvider](../../com.groupdocs.search.dictionaries/iwordformsprovider) - The word forms provider.

### setWordFormsProvider(IWordFormsProvider value) {#setWordFormsProvider-com.groupdocs.search.dictionaries.IWordFormsProvider-}
```
public abstract void setWordFormsProvider(IWordFormsProvider value)
```


Устанавливает поставщик форм слов.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | value | [IWordFormsProvider](../../com.groupdocs.search.dictionaries/iwordformsprovider) | Поставщик форм слов. |
|

