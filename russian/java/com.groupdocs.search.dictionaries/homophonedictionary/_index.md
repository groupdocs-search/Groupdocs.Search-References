---
title: "HomophoneDictionary"
second_title: "GroupDocs.Search для Java API Reference"
description: "Определяет интерфейс словаря гетерографических омонимов."
type: docs
weight: 18
url: /ru/java/com.groupdocs.search.dictionaries/homophonedictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface HomophoneDictionary extends DictionaryBase, Iterable<String>
```

Определяет интерфейс словаря гетерографических омонимов.


**Learn more**

* [Homophone search](../https://docs.groupdocs.com/display/searchjava/Homophone+search)
* [Managing homophone dictionary](../https://docs.groupdocs.com/display/searchjava/Homophone+dictionary)

## Методы

| Метод | Описание |
| --- | --- |
|  | [getCount()](#getCount--) | Получает количество слов, содержащихся в этом  HomophoneDictionary . |
|
|  | [addRange(Iterable<String[]> homophones)](#addRange-java.lang.Iterable-java.lang.String----) | Добавляет указанную коллекцию групп омонимов в этот экземпляр  HomophoneDictionary . |
|
|  | [addRange(String[][] homophones)](#addRange-java.lang.String-----) | Добавляет указанную коллекцию групп омонимов в этот экземпляр  HomophoneDictionary . |
|
|  | [clear()](#clear--) | Удаляет все слова из объекта  HomophoneDictionary . |
|
|  | [getHomophones(String word)](#getHomophones-java.lang.String-) | Получает омонимы для указанного слова. |
|
|  | [getHomophoneGroups(String word)](#getHomophoneGroups-java.lang.String-) | Получает все группы омонимов, к которым относится указанное слово. |
|
|  | [getAllHomophoneGroups()](#getAllHomophoneGroups--) | Получает все группы омонимов, содержащиеся в этом словаре. |
|
|  | [iterator()](#iterator--) | Возвращает итератор, который проходит по коллекции. |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


Получает количество слов, содержащихся в этом  HomophoneDictionary .


**Returns:**
int - Количество слов.

### addRange(Iterable<String[]> homophones) {#addRange-java.lang.Iterable-java.lang.String----}
```
public abstract void addRange(Iterable<String[]> homophones)
```


Добавляет указанную коллекцию групп омонимов в этот экземпляр  HomophoneDictionary .


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | homophones | java.lang.Iterable<java.lang.String[]> | Коллекция групп омонимов для добавления в словарь. |
|

### addRange(String[][] homophones) {#addRange-java.lang.String-----}
```
public abstract void addRange(String[][] homophones)
```


Добавляет указанную коллекцию групп омонимов в этот экземпляр  HomophoneDictionary .


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | homophones | java.lang.String[][] | Коллекция групп омонимов для добавления в словарь. |
|

### clear() {#clear--}
```
public abstract void clear()
```


Удаляет все слова из объекта  HomophoneDictionary .


### getHomophones(String word) {#getHomophones-java.lang.String-}
```
public abstract String[] getHomophones(String word)
```


Получает омонимы для указанного слова. Полученный массив не содержит исходное слово.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | слово | java.lang.String | Слово для предложения омофонов. |
|

**Returns:**
java.lang.String[] - Омофоны для указанного слова или пустой массив, если объект  HomophoneDictionary  не содержит указанного слова.

### getHomophoneGroups(String word) {#getHomophoneGroups-java.lang.String-}
```
public abstract String[][] getHomophoneGroups(String word)
```


Получает все группы омонимов, к которым относится указанное слово.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | слово | java.lang.String | Слово для получения групп омофонов. |
|

**Returns:**
java.lang.String[][] - Все группы омофонов, к которым относится указанное слово.

### getAllHomophoneGroups() {#getAllHomophoneGroups--}
```
public abstract String[][] getAllHomophoneGroups()
```


Получает все группы омонимов, содержащиеся в этом словаре.


**Returns:**
java.lang.String[][] - Все группы омофонов.

### iterator() {#iterator--}
```
public abstract Iterator<String> iterator()
```


Возвращает итератор, который проходит по коллекции.


**Returns:**
java.util.Iterator<java.lang.String> - Итератор, который можно использовать для перебора элементов коллекции.

