---
title: "Indexer"
second_title: "GroupDocs.Search для Java API Reference"
description: "Представляет сервис, управляющий распределением проиндексированных документов по шардам поисковой сети."
type: docs
weight: 10
url: /ru/java/com.groupdocs.search.scaling/indexer/
---
**Inheritance:**
java.lang.Object
```
public abstract class Indexer
```

Представляет сервис, управляющий распределением проиндексированных документов по шардам поисковой сети.

## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [Indexer()](#Indexer--) |  |
## Методы

| Метод | Описание |
| --- | --- |
|  | [add(Document[] documents, String[] passwords, IndexingOptions options)](#add-com.groupdocs.search.Document---java.lang.String---com.groupdocs.search.options.IndexingOptions-) | Выполняет операцию индексации. |
|
|  | [add(ExtractedData[] data, IndexingOptions options)](#add-com.groupdocs.search.ExtractedData---com.groupdocs.search.options.IndexingOptions-) | Выполняет операцию индексации. |
|
|  | [delete(String[] documentKeys, DeleteOptions options)](#delete-java.lang.String---com.groupdocs.search.options.DeleteOptions-) | Удаляет проиндексированные документы. |
|
|  | [optimize(OptimizeOptions options)](#optimize-com.groupdocs.search.options.OptimizeOptions-) | Минимизирует количество сегментов индекса, объединяя их друг с другом. |
|
|  | [synchronize(SynchronizeOptions options)](#synchronize-com.groupdocs.search.options.SynchronizeOptions-) | Синхронизирует список проиндексированных документов с документами на шардах. |
|
|  | [changeAttributes(AttributeChangeBatch batch, ChangeAttributesOptions options)](#changeAttributes-com.groupdocs.search.common.AttributeChangeBatch-com.groupdocs.search.options.ChangeAttributesOptions-) | Применяет указанную партию изменений атрибутов к проиндексированным документам без переиндексации. |
|
|  | [getAttributes(String documentKey)](#getAttributes-java.lang.String-) | Получает все атрибуты, связанные с указанным проиндексированным документом. |
|
|  | [getDictionary(DictionaryType dictionaryType, int shardIndex)](#getDictionary-com.groupdocs.search.dictionaries.DictionaryType-int-) | Получает словарь из указанного шарда. |
|
|  | [getAlphabet(int shardIndex)](#getAlphabet-int-) | Получает алфавитный словарь. |
|
|  | [getAliasDictionary(int shardIndex)](#getAliasDictionary-int-) | Получает словарь псевдонимов. |
|
|  | [getCharacterReplacementDictionary(int shardIndex)](#getCharacterReplacementDictionary-int-) | Получает словарь замены символов. |
|
|  | [getSynonymDictionary(int shardIndex)](#getSynonymDictionary-int-) | Получает словарь синонимов. |
|
|  | [getHomophoneDictionary(int shardIndex)](#getHomophoneDictionary-int-) | Получает словарь омонимов. |
|
|  | [getSpellingCorrector(int shardIndex)](#getSpellingCorrector-int-) | Получает словарь корректора орфографии. |
|
|  | [getStopWordDictionary(int shardIndex)](#getStopWordDictionary-int-) | Получает словарь стоп-слов. |
|
|  | [getPasswordDictionary(int shardIndex)](#getPasswordDictionary-int-) | Получает словарь паролей. |
|
|  | [setDictionary(DictionaryBase dictionary, int shardIndex)](#setDictionary-com.groupdocs.search.dictionaries.DictionaryBase-int-) | Устанавливает словарь в указанном шарде. |
|
|  | [setDictionary(DictionaryBase dictionary)](#setDictionary-com.groupdocs.search.dictionaries.DictionaryBase-) | Устанавливает словарь во всех шардах. |
|
|  | [deleteAllData()](#deleteAllData--) | Удаляет все проиндексированные данные со всех шардов поисковой сети. |
|
### Indexer() {#Indexer--}
```
public Indexer()
```


### add(Document[] documents, String[] passwords, IndexingOptions options) {#add-com.groupdocs.search.Document---java.lang.String---com.groupdocs.search.options.IndexingOptions-}
```
public abstract void add(Document[] documents, String[] passwords, IndexingOptions options)
```


Выполняет операцию индексирования. Поддерживается только индексирование из потока и структуры.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | documents | [Document\[\]](../../com.groupdocs.search/document) | Документы из файловой системы, потока или структуры. |
|
|  | пароли | java.lang.String[] | Пароли документа. |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | Параметры добавления. |
|

### add(ExtractedData[] data, IndexingOptions options) {#add-com.groupdocs.search.ExtractedData---com.groupdocs.search.options.IndexingOptions-}
```
public abstract void add(ExtractedData[] data, IndexingOptions options)
```


Выполняет операцию индексирования. Добавляет извлечённые данные в поисковую сеть.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | data | [ExtractedData\[\]](../../com.groupdocs.search/extracteddata) | Извлечённые данные. |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | Параметры индексации. |
|

### delete(String[] documentKeys, DeleteOptions options) {#delete-java.lang.String---com.groupdocs.search.options.DeleteOptions-}
```
public abstract void delete(String[] documentKeys, DeleteOptions options)
```


Удаляет проиндексированные документы.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | documentKeys | java.lang.String[] | Ключи документов, добавленных из потоков или структур. |
|
|  | options | [DeleteOptions](../../com.groupdocs.search.options/deleteoptions) | Параметры удаления. |
|

### optimize(OptimizeOptions options) {#optimize-com.groupdocs.search.options.OptimizeOptions-}
```
public abstract void optimize(OptimizeOptions options)
```


Уменьшает количество сегментов индекса, объединяя их друг с другом. Эта операция улучшает производительность поиска.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | options | [OptimizeOptions](../../com.groupdocs.search.options/optimizeoptions) | Параметры оптимизации. |
|

### synchronize(SynchronizeOptions options) {#synchronize-com.groupdocs.search.options.SynchronizeOptions-}
```
public abstract void synchronize(SynchronizeOptions options)
```


Синхронизирует список проиндексированных документов с документами на шардах. Эта операция исправляет проблемы с индексированием и удалением документов, возникшие из‑за проблем связи с узлами поисковой сети.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | options | [SynchronizeOptions](../../com.groupdocs.search.options/synchronizeoptions) | Параметры синхронизации. |
|

### changeAttributes(AttributeChangeBatch batch, ChangeAttributesOptions options) {#changeAttributes-com.groupdocs.search.common.AttributeChangeBatch-com.groupdocs.search.options.ChangeAttributesOptions-}
```
public abstract void changeAttributes(AttributeChangeBatch batch, ChangeAttributesOptions options)
```


Применяет указанную партию изменений атрибутов к проиндексированным документам без переиндексации.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | batch | [AttributeChangeBatch](../../com.groupdocs.search.common/attributechangebatch) | Пакет изменений атрибутов. |
|
|  | options | [ChangeAttributesOptions](../../com.groupdocs.search.options/changeattributesoptions) | Параметры изменения атрибутов. |
|

### getAttributes(String documentKey) {#getAttributes-java.lang.String-}
```
public abstract String[] getAttributes(String documentKey)
```


Получает все атрибуты, связанные с указанным проиндексированным документом.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | documentKey | java.lang.String | Ключ документа. |
|

**Returns:**
java.lang.String[] — Атрибуты, связанные с указанным проиндексированным документом.

### getDictionary(DictionaryType dictionaryType, int shardIndex) {#getDictionary-com.groupdocs.search.dictionaries.DictionaryType-int-}
```
public abstract DictionaryBase getDictionary(DictionaryType dictionaryType, int shardIndex)
```


Получает словарь из указанного шарда.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | dictionaryType | [DictionaryType](../../com.groupdocs.search.dictionaries/dictionarytype) | Тип словаря. |
|
|  | shardIndex | int | Индекс шарда. |
|

**Returns:**
[DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase) - The dictionary.

### getAlphabet(int shardIndex) {#getAlphabet-int-}
```
public abstract Alphabet getAlphabet(int shardIndex)
```


Получает алфавитный словарь.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | shardIndex | int | Индекс шарда. |
|

**Returns:**
[Alphabet](../../com.groupdocs.search.dictionaries/alphabet) - The dictionary.

### getAliasDictionary(int shardIndex) {#getAliasDictionary-int-}
```
public abstract AliasDictionary getAliasDictionary(int shardIndex)
```


Получает словарь псевдонимов.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | shardIndex | int | Индекс шарда. |
|

**Returns:**
[AliasDictionary](../../com.groupdocs.search.dictionaries/aliasdictionary) - The dictionary.

### getCharacterReplacementDictionary(int shardIndex) {#getCharacterReplacementDictionary-int-}
```
public abstract CharacterReplacementDictionary getCharacterReplacementDictionary(int shardIndex)
```


Получает словарь замены символов.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | shardIndex | int | Индекс шарда. |
|

**Returns:**
[CharacterReplacementDictionary](../../com.groupdocs.search.dictionaries/characterreplacementdictionary) - The dictionary.

### getSynonymDictionary(int shardIndex) {#getSynonymDictionary-int-}
```
public abstract SynonymDictionary getSynonymDictionary(int shardIndex)
```


Получает словарь синонимов.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | shardIndex | int | Индекс шарда. |
|

**Returns:**
[SynonymDictionary](../../com.groupdocs.search.dictionaries/synonymdictionary) - The dictionary.

### getHomophoneDictionary(int shardIndex) {#getHomophoneDictionary-int-}
```
public abstract HomophoneDictionary getHomophoneDictionary(int shardIndex)
```


Получает словарь омонимов.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | shardIndex | int | Индекс шарда. |
|

**Returns:**
[HomophoneDictionary](../../com.groupdocs.search.dictionaries/homophonedictionary) - The dictionary.

### getSpellingCorrector(int shardIndex) {#getSpellingCorrector-int-}
```
public abstract SpellingCorrector getSpellingCorrector(int shardIndex)
```


Получает словарь корректора орфографии.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | shardIndex | int | Индекс шарда. |
|

**Returns:**
[SpellingCorrector](../../com.groupdocs.search.dictionaries/spellingcorrector) - The dictionary.

### getStopWordDictionary(int shardIndex) {#getStopWordDictionary-int-}
```
public abstract StopWordDictionary getStopWordDictionary(int shardIndex)
```


Получает словарь стоп-слов.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | shardIndex | int | Индекс шарда. |
|

**Returns:**
[StopWordDictionary](../../com.groupdocs.search.dictionaries/stopworddictionary) - The dictionary.

### getPasswordDictionary(int shardIndex) {#getPasswordDictionary-int-}
```
public abstract PasswordDictionary getPasswordDictionary(int shardIndex)
```


Получает словарь паролей.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | shardIndex | int | Индекс шарда. |
|

**Returns:**
[PasswordDictionary](../../com.groupdocs.search.dictionaries/passworddictionary) - The dictionary.

### setDictionary(DictionaryBase dictionary, int shardIndex) {#setDictionary-com.groupdocs.search.dictionaries.DictionaryBase-int-}
```
public abstract void setDictionary(DictionaryBase dictionary, int shardIndex)
```


Устанавливает словарь в указанном шарде.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | dictionary | [DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase) | Словарь. |
|
|  | shardIndex | int | Индекс шарда. |
|

### setDictionary(DictionaryBase dictionary) {#setDictionary-com.groupdocs.search.dictionaries.DictionaryBase-}
```
public abstract void setDictionary(DictionaryBase dictionary)
```


Устанавливает словарь во всех шардах.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | dictionary | [DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase) | Словарь. |
|

### deleteAllData() {#deleteAllData--}
```
public abstract void deleteAllData()
```


Удаляет все проиндексированные данные со всех шардов поисковой сети.


