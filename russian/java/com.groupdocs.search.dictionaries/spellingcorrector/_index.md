---
title: "SpellingCorrector"
second_title: "GroupDocs.Search для Java API Reference"
description: "Определяет интерфейс корректора орфографии для терминов в запросе."
type: docs
weight: 21
url: /ru/java/com.groupdocs.search.dictionaries/spellingcorrector/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase)
```
public interface SpellingCorrector extends DictionaryBase
```

Определяет интерфейс корректора орфографии для терминов в запросе.


**Learn more**

* [Spell checking](../https://docs.groupdocs.com/display/searchjava/Spell+checking)
* [Managing spelling corrector](../https://docs.groupdocs.com/display/searchjava/Spelling+corrector)

## Методы

| Метод | Описание |
| --- | --- |
|  | [getCount()](#getCount--) | Получает количество слов, содержащихся в этом  SpellingCorrector . |
|
|  | [getWords()](#getWords--) | Получает коллекцию слов, которая в данный момент содержится в этом  SpellingCorrector . |
|
|  | [addRange(Iterable<String> words)](#addRange-java.lang.Iterable-java.lang.String--) | Добавляет указанную коллекцию слов в этот экземпляр  SpellingCorrector . |
|
|  | [addRange(String[] words)](#addRange-java.lang.String---) | Добавляет указанную коллекцию слов в этот экземпляр  SpellingCorrector . |
|
|  | [clear()](#clear--) | Удаляет все слова из объекта  SpellingCorrector . |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


Получает количество слов, содержащихся в этом  SpellingCorrector .


**Returns:**
int - Количество слов, содержащихся в этом  SpellingCorrector .

### getWords() {#getWords--}
```
public abstract String[] getWords()
```


Получает коллекцию слов, которая в данный момент содержится в этом  SpellingCorrector .


**Returns:**
java.lang.String[] - Коллекция слов.

### addRange(Iterable<String> words) {#addRange-java.lang.Iterable-java.lang.String--}
```
public abstract void addRange(Iterable<String> words)
```


Добавляет указанную коллекцию слов в этот экземпляр  SpellingCorrector .


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | слова | java.lang.Iterable<java.lang.String> | Коллекция слов для добавления в словарь. |
|

### addRange(String[] words) {#addRange-java.lang.String---}
```
public abstract void addRange(String[] words)
```


Добавляет указанную коллекцию слов в этот экземпляр  SpellingCorrector .


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | слова | java.lang.String[] | Коллекция слов для добавления в словарь. |
|

### clear() {#clear--}
```
public abstract void clear()
```


Удаляет все слова из объекта  SpellingCorrector .


