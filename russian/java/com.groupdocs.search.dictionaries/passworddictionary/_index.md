---
title: "PasswordDictionary"
second_title: "GroupDocs.Search для Java API Reference"
description: "Определяет интерфейс словаря паролей документов."
type: docs
weight: 20
url: /ru/java/com.groupdocs.search.dictionaries/passworddictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface PasswordDictionary extends DictionaryBase, Iterable<String>
```

Определяет интерфейс словаря паролей документов.


**Learn more**

* [Indexing password protected documents](../https://docs.groupdocs.com/display/searchjava/Indexing+password+protected+documents)
* [Managing document passwords](../https://docs.groupdocs.com/display/searchjava/Document+passwords)

## Методы

| Метод | Описание |
| --- | --- |
|  | [getCount()](#getCount--) | Возвращает количество элементов, содержащихся в словаре. |
|
|  | [getPassword(String filePath)](#getPassword-java.lang.String-) | Возвращает пароль для файла. |
|
|  | [clear()](#clear--) | Удаляет все пароли из этого объекта  PasswordDictionary . |
|
|  | [contains(String filePath)](#contains-java.lang.String-) | Определяет, содержит ли словарь пароль для указанного документа. |
|
|  | [add(String filePath, String password)](#add-java.lang.String-java.lang.String-) | Добавляет пароль для документа в словарь. |
|
|  | [remove(String filePath)](#remove-java.lang.String-) | Удаляет пароль указанного документа из словаря. |
|
|  | [iterator()](#iterator--) | Возвращает итератор, который проходит по коллекции. |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


Возвращает количество элементов, содержащихся в словаре.


**Returns:**
int - Количество элементов, содержащихся в словаре.

### getPassword(String filePath) {#getPassword-java.lang.String-}
```
public abstract String getPassword(String filePath)
```


Возвращает пароль для файла.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | filePath | java.lang.String | Путь к файлу. |
|

**Returns:**
java.lang.String - Пароль для файла.

### clear() {#clear--}
```
public abstract void clear()
```


Удаляет все пароли из этого объекта  PasswordDictionary .


### contains(String filePath) {#contains-java.lang.String-}
```
public abstract boolean contains(String filePath)
```


Определяет, содержит ли словарь пароль для указанного документа.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | filePath | java.lang.String | Путь к файлу документа. |
|

**Returns:**
boolean -  true  если словарь содержит пароль для документа; иначе,  false .

### add(String filePath, String password) {#add-java.lang.String-java.lang.String-}
```
public abstract void add(String filePath, String password)
```


Добавляет пароль для документа в словарь.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | filePath | java.lang.String | Путь к файлу документа. |
|
|  | пароль | java.lang.String | Пароль документа. |
|

### remove(String filePath) {#remove-java.lang.String-}
```
public abstract boolean remove(String filePath)
```


Удаляет пароль указанного документа из словаря.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | filePath | java.lang.String | Путь к файлу документа. |
|

**Returns:**
boolean -  true  если пароль был успешно удалён; иначе,  false . Этот метод также возвращает  false , если  filePath  не найден в словаре.

### iterator() {#iterator--}
```
public abstract Iterator<String> iterator()
```


Возвращает итератор, который проходит по коллекции.


**Returns:**
java.util.Iterator<java.lang.String> - Итератор, который можно использовать для перебора элементов коллекции.

