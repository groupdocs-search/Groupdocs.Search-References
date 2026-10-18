---
title: "DateFormatCollection"
second_title: "GroupDocs.Search для Java API Reference"
description: "Представляет коллекцию объектов DateFormat."
type: docs
weight: 14
url: /ru/java/com.groupdocs.search.options/dateformatcollection/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public abstract class DateFormatCollection implements Iterable<DateFormat>
```

Представляет коллекцию объектов DateFormat.


**Learn more**

* [Date range search](../https://docs.groupdocs.com/display/searchjava/Date+range+search)

## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [DateFormatCollection()](#DateFormatCollection--) |  |
## Методы

| Метод | Описание |
| --- | --- |
|  | [addItem(DateFormat item)](#addItem-com.groupdocs.search.options.DateFormat-) | Добавляет объект формата даты в коллекцию. |
|
|  | [clear()](#clear--) | Удаляет все элементы из коллекции. |
|
|  | [containsItem(DateFormat item)](#containsItem-com.groupdocs.search.options.DateFormat-) | Определяет, содержит ли коллекция конкретный элемент. |
|
|  | [copyToTArray(DateFormat[] array, int arrayIndex)](#copyToTArray-com.groupdocs.search.options.DateFormat---int-) | Копирует элементы коллекции в массив Array, начиная с указанного индекса массива. |
|
|  | [size()](#size--) | Возвращает количество элементов, содержащихся в коллекции. |
|
|  | [isReadOnly()](#isReadOnly--) | Возвращает значение, указывающее, является ли коллекция только для чтения. |
|
|  | [removeItem(DateFormat item)](#removeItem-com.groupdocs.search.options.DateFormat-) | Удаляет первое вхождение конкретного элемента из коллекции. |
|
|  | [iterator()](#iterator--) | Возвращает перечислитель, который перебирает элементы коллекции. |
|
### DateFormatCollection() {#DateFormatCollection--}
```
public DateFormatCollection()
```


### addItem(DateFormat item) {#addItem-com.groupdocs.search.options.DateFormat-}
```
public abstract void addItem(DateFormat item)
```


Добавляет объект формата даты в коллекцию.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | item | [DateFormat](../../com.groupdocs.search.options/dateformat) | Объект формата даты для добавления в коллекцию. |
|

### clear() {#clear--}
```
public abstract void clear()
```


Удаляет все элементы из коллекции.


### containsItem(DateFormat item) {#containsItem-com.groupdocs.search.options.DateFormat-}
```
public abstract boolean containsItem(DateFormat item)
```


Определяет, содержит ли коллекция конкретный элемент.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | item | [DateFormat](../../com.groupdocs.search.options/dateformat) | Элемент для поиска в коллекции. |
|

**Returns:**
boolean -  true  если элемент найден в коллекции; иначе,  false .

### copyToTArray(DateFormat[] array, int arrayIndex) {#copyToTArray-com.groupdocs.search.options.DateFormat---int-}
```
public abstract void copyToTArray(DateFormat[] array, int arrayIndex)
```


Копирует элементы коллекции в массив Array, начиная с указанного индекса массива.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | array | [DateFormat\[\]](../../com.groupdocs.search.options/dateformat) | Одномерный  Array  который является получателем элементов, скопированных из коллекции. |
|
|  | arrayIndex | int | Нулевой индекс в массиве, с которого начинается копирование. |
|

### size() {#size--}
```
public abstract int size()
```


Возвращает количество элементов, содержащихся в коллекции.


**Returns:**
int - Количество элементов, содержащихся в коллекции.

### isReadOnly() {#isReadOnly--}
```
public abstract boolean isReadOnly()
```


Возвращает значение, указывающее, является ли коллекция только для чтения.


**Returns:**
boolean -  true  если коллекция доступна только для чтения; иначе,  false .

### removeItem(DateFormat item) {#removeItem-com.groupdocs.search.options.DateFormat-}
```
public abstract boolean removeItem(DateFormat item)
```


Удаляет первое вхождение конкретного элемента из коллекции.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | item | [DateFormat](../../com.groupdocs.search.options/dateformat) | Элемент для удаления из коллекции. |
|

**Returns:**
boolean -  true  если элемент был успешно удалён из коллекции; иначе,  false . Этот метод также возвращает  false , если элемент не найден в коллекции.

### iterator() {#iterator--}
```
public abstract Iterator<DateFormat> iterator()
```


Возвращает перечислитель, который перебирает элементы коллекции.


**Returns:**
java.util.Iterator<com.groupdocs.search.options.DateFormat> - Перечислитель, который можно использовать для перебора элементов коллекции.

