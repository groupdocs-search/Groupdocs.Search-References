---
title: "SynonymDictionary"
second_title: "GroupDocs.Search для Java API Reference"
description: "Определяет интерфейс словаря синонимов."
type: docs
weight: 23
url: /ru/java/com.groupdocs.search.dictionaries/synonymdictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface SynonymDictionary extends DictionaryBase, Iterable<String>
```

Определяет интерфейс словаря синонимов.


**Learn more**

* [Synonym search](../https://docs.groupdocs.com/display/searchjava/Synonym+search)
* [Managing synonym dictionary](../https://docs.groupdocs.com/display/searchjava/Synonym+dictionary)

## Методы

| Метод | Описание |
| --- | --- |
|  | [getCount()](#getCount--) | Возвращает количество слов, содержащихся в этом SynonymDictionary. |
|
|  | [addRange(Iterable<String[]> synonyms)](#addRange-java.lang.Iterable-java.lang.String----) | Добавляет указанную коллекцию групп синонимов к этому экземпляру SynonymDictionary. |
|
|  | [addRange(String[][] synonyms)](#addRange-java.lang.String-----) | Добавляет указанную коллекцию групп синонимов к этому экземпляру SynonymDictionary. |
|
|  | [clear()](#clear--) | Удаляет все слова из этого объекта SynonymDictionary. |
|
|  | [getSynonyms(String word)](#getSynonyms-java.lang.String-) | Получает синонимы для указанного слова. |
|
|  | [getSynonymGroups(String word)](#getSynonymGroups-java.lang.String-) | Получает все группы синонимов, к которым относится указанное слово. |
|
|  | [getAllSynonymGroups()](#getAllSynonymGroups--) | Получает все группы синонимов, содержащиеся в этом словаре. |
|
|  | [iterator()](#iterator--) | Возвращает итератор, который проходит по коллекции. |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


Возвращает количество слов, содержащихся в этом SynonymDictionary.


**Returns:**
int — количество слов, содержащихся в этом SynonymDictionary.

### addRange(Iterable<String[]> synonyms) {#addRange-java.lang.Iterable-java.lang.String----}
```
public abstract void addRange(Iterable<String[]> synonyms)
```


Добавляет указанную коллекцию групп синонимов к этому экземпляру SynonymDictionary.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | синонимы | java.lang.Iterable<java.lang.String[]> | Коллекция групп синонимов для добавления в словарь. |
|

### addRange(String[][] synonyms) {#addRange-java.lang.String-----}
```
public abstract void addRange(String[][] synonyms)
```


Добавляет указанную коллекцию групп синонимов к этому экземпляру SynonymDictionary.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | синонимы | java.lang.String[][] | Коллекция групп синонимов для добавления в словарь. |
|

### clear() {#clear--}
```
public abstract void clear()
```


Удаляет все слова из этого объекта SynonymDictionary.


### getSynonyms(String word) {#getSynonyms-java.lang.String-}
```
public abstract String[] getSynonyms(String word)
```


Получает синонимы для указанного слова. Полученный массив не содержит исходное слово.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | слово | java.lang.String | Слово, для которого предлагаются синонимы. |
|

**Returns:**
java.lang.String[] — синонимы для указанного слова или пустой массив, если объект SynonymDictionary не содержит указанное слово.

### getSynonymGroups(String word) {#getSynonymGroups-java.lang.String-}
```
public abstract String[][] getSynonymGroups(String word)
```


Получает все группы синонимов, к которым относится указанное слово.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | слово | java.lang.String | Слово для получения групп синонимов. |
|

**Returns:**
java.lang.String[][] - Все группы синонимов, к которым относится указанное слово.

### getAllSynonymGroups() {#getAllSynonymGroups--}
```
public abstract String[][] getAllSynonymGroups()
```


Получает все группы синонимов, содержащиеся в этом словаре.


**Returns:**
java.lang.String[][] - Все группы синонимов.

### iterator() {#iterator--}
```
public abstract Iterator<String> iterator()
```


Возвращает итератор, который проходит по коллекции.


**Returns:**
java.util.Iterator<java.lang.String> - Итератор, который можно использовать для перебора элементов коллекции.

