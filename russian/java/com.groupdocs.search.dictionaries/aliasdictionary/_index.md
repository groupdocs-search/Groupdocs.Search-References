---
title: "AliasDictionary"
second_title: "GroupDocs.Search для Java API Reference"
description: "Определяет интерфейс словаря псевдонимов."
type: docs
weight: 14
url: /ru/java/com.groupdocs.search.dictionaries/aliasdictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface AliasDictionary extends DictionaryBase, Iterable<String>
```

Определяет интерфейс словаря псевдонимов.


**Learn more**

* [Using aliases](../https://docs.groupdocs.com/display/searchjava/Using+aliases)
* [Managing alias dictionary](../https://docs.groupdocs.com/display/searchjava/Alias+dictionary)

## Методы

| Метод | Описание |
| --- | --- |
|  | [getCount()](#getCount--) | Получает количество псевдонимов, содержащихся в  AliasDictionary . |
|
|  | [addRange(Iterable<AliasReplacementPair> pairs)](#addRange-java.lang.Iterable-com.groupdocs.search.dictionaries.AliasReplacementPair--) | Добавляет указанную коллекцию пар псевдоним/замена к этому экземпляру  AliasDictionary . |
|
|  | [addRange(AliasReplacementPair[] pairs)](#addRange-com.groupdocs.search.dictionaries.AliasReplacementPair---) | Добавляет указанную коллекцию пар псевдоним/замена к этому экземпляру  AliasDictionary . |
|
|  | [add(String alias, String text)](#add-java.lang.String-java.lang.String-) | Добавляет указанную пару псевдонима и связанного текста к этому экземпляру  AliasDictionary . |
|
|  | [remove(String alias)](#remove-java.lang.String-) | Удаляет указанный псевдоним из объекта  AliasDictionary . |
|
|  | [contains(String alias)](#contains-java.lang.String-) | Определяет, содержит ли объект  AliasDictionary  указанный псевдоним. |
|
|  | [getText(String alias)](#getText-java.lang.String-) | Получает текст, связанный с указанным псевдонимом. |
|
|  | [clear()](#clear--) | Удаляет все псевдонимы из объекта  AliasDictionary . |
|
|  | [iterator()](#iterator--) | Возвращает итератор, который проходит по коллекции. |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


Получает количество псевдонимов, содержащихся в  AliasDictionary .


**Returns:**
int - Количество псевдонимов, содержащихся в  AliasDictionary .

### addRange(Iterable<AliasReplacementPair> pairs) {#addRange-java.lang.Iterable-com.groupdocs.search.dictionaries.AliasReplacementPair--}
```
public abstract void addRange(Iterable<AliasReplacementPair> pairs)
```


Добавляет указанную коллекцию пар псевдоним/замена к этому экземпляру  AliasDictionary .


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | пары | java.lang.Iterable<com.groupdocs.search.dictionaries.AliasReplacementPair> | Коллекция пар псевдоним/замена для добавления в словарь. |
|

### addRange(AliasReplacementPair[] pairs) {#addRange-com.groupdocs.search.dictionaries.AliasReplacementPair---}
```
public abstract void addRange(AliasReplacementPair[] pairs)
```


Добавляет указанную коллекцию пар псевдоним/замена к этому экземпляру  AliasDictionary .


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | pairs | [AliasReplacementPair\[\]](../../com.groupdocs.search.dictionaries/aliasreplacementpair) | Коллекция пар псевдоним/замена для добавления в словарь. |
|

### add(String alias, String text) {#add-java.lang.String-java.lang.String-}
```
public abstract void add(String alias, String text)
```


Добавляет указанную пару псевдонима и связанного текста к этому экземпляру  AliasDictionary .


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | псевдоним | java.lang.String | Псевдоним для добавления в словарь. |
|
|  | текст | java.lang.String | Текст, который будет связан с псевдонимом. |
|

### remove(String alias) {#remove-java.lang.String-}
```
public abstract boolean remove(String alias)
```


Удаляет указанный псевдоним из объекта  AliasDictionary .


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | псевдоним | java.lang.String | Псевдоним для удаления. |
|

**Returns:**
boolean - Этот метод возвращает  true  если псевдоним успешно найден и удалён. Этот метод возвращает  false  если псевдоним не найден в объекте  AliasDictionary .

### contains(String alias) {#contains-java.lang.String-}
```
public abstract boolean contains(String alias)
```


Определяет, содержит ли объект  AliasDictionary  указанный псевдоним.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | псевдоним | java.lang.String | Псевдоним для поиска в объекте  AliasDictionary . |
|

**Returns:**
boolean -  true  если объект  AliasDictionary  содержит указанный псевдоним; в противном случае,  false .

### getText(String alias) {#getText-java.lang.String-}
```
public abstract String getText(String alias)
```


Получает текст, связанный с указанным псевдонимом.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | псевдоним | java.lang.String | Псевдоним для поиска в объекте  AliasDictionary . |
|

**Returns:**
java.lang.String - Текст, связанный с указанным псевдонимом, или  null .

### clear() {#clear--}
```
public abstract void clear()
```


Удаляет все псевдонимы из объекта  AliasDictionary .


### iterator() {#iterator--}
```
public abstract Iterator<String> iterator()
```


Возвращает итератор, который проходит по коллекции.


**Returns:**
java.util.Iterator<java.lang.String> - Итератор, который можно использовать для перебора элементов коллекции.

