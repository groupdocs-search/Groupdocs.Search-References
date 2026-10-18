---
title: "StopWordDictionary"
second_title: "GroupDocs.Search для Java API Reference"
description: "Определяет интерфейс словаря стоп-слов."
type: docs
weight: 22
url: /ru/java/com.groupdocs.search.dictionaries/stopworddictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface StopWordDictionary extends DictionaryBase, Iterable<String>
```

Определяет интерфейс словаря стоп-слов.


**Learn more**

* [Indexing with stop words](../https://docs.groupdocs.com/display/searchjava/Indexing+with+stop+words)
* [Managing stop word dictionary](../https://docs.groupdocs.com/display/searchjava/Stop+word+dictionary)

## Методы

| Метод | Описание |
| --- | --- |
|  | [getCount()](#getCount--) | Получает количество стоп-слов, содержащихся в  StopWordDictionary . |
|
|  | [addRange(Iterable<String> words)](#addRange-java.lang.Iterable-java.lang.String--) | Добавляет указанную коллекцию слов в этот экземпляр  StopWordDictionary . |
|
|  | [addRange(String[] words)](#addRange-java.lang.String---) | Добавляет указанную коллекцию слов в этот экземпляр  StopWordDictionary . |
|
|  | [removeRange(Iterable<String> words)](#removeRange-java.lang.Iterable-java.lang.String--) | Удаляет указанную коллекцию слов из этого экземпляра  StopWordDictionary . |
|
|  | [removeRange(String[] words)](#removeRange-java.lang.String---) | Удаляет указанную коллекцию слов из этого экземпляра  StopWordDictionary . |
|
|  | [contains(String word)](#contains-java.lang.String-) | Определяет, содержит ли объект  StopWordDictionary  указанное слово. |
|
|  | [clear()](#clear--) | Удаляет все слова из объекта  StopWordDictionary . |
|
|  | [iterator()](#iterator--) | Возвращает итератор, который проходит по коллекции. |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


Получает количество стоп-слов, содержащихся в  StopWordDictionary .


**Returns:**
int - Количество стоп-слов в словаре.

### addRange(Iterable<String> words) {#addRange-java.lang.Iterable-java.lang.String--}
```
public abstract void addRange(Iterable<String> words)
```


Добавляет указанную коллекцию слов в этот экземпляр  StopWordDictionary .


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | слова | java.lang.Iterable<java.lang.String> | Коллекция слов для добавления в словарь. |
|

### addRange(String[] words) {#addRange-java.lang.String---}
```
public abstract void addRange(String[] words)
```


Добавляет указанную коллекцию слов в этот экземпляр  StopWordDictionary .


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | слова | java.lang.String[] | Коллекция слов для добавления в словарь. |
|

### removeRange(Iterable<String> words) {#removeRange-java.lang.Iterable-java.lang.String--}
```
public abstract void removeRange(Iterable<String> words)
```


Удаляет указанную коллекцию слов из этого экземпляра  StopWordDictionary .


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | слова | java.lang.Iterable<java.lang.String> | Коллекция слов для удаления. |
|

### removeRange(String[] words) {#removeRange-java.lang.String---}
```
public abstract void removeRange(String[] words)
```


Удаляет указанную коллекцию слов из этого экземпляра  StopWordDictionary .


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | слова | java.lang.String[] | Коллекция слов для удаления. |
|

### contains(String word) {#contains-java.lang.String-}
```
public abstract boolean contains(String word)
```


Определяет, содержит ли объект  StopWordDictionary  указанное слово.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | слово | java.lang.String | Слово для поиска в объекте  StopWordDictionary . |
|

**Returns:**
boolean -  true  если объект  StopWordDictionary  содержит указанное слово; иначе,  false .

### clear() {#clear--}
```
public abstract void clear()
```


Удаляет все слова из объекта  StopWordDictionary .


### iterator() {#iterator--}
```
public abstract Iterator<String> iterator()
```


Возвращает итератор, который проходит по коллекции.


**Returns:**
java.util.Iterator<java.lang.String> - Итератор, который можно использовать для перебора элементов коллекции.

