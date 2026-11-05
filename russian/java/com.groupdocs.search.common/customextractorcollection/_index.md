---
title: "CustomExtractorCollection"
second_title: "GroupDocs.Search для Java API Reference"
description: "Содержит коллекцию пользовательских экстракторов."
type: docs
weight: 13
url: /ru/java/com.groupdocs.search.common/customextractorcollection/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public abstract class CustomExtractorCollection implements Iterable
```

Содержит коллекцию пользовательских извлекателей. Если коллекция содержит извлекатель для какого-то расширения файла, которое покрывается встроенными извлекателями, то будет использован этот извлекатель вместо встроенного.


**Learn more**

* [Custom text extractors](../https://docs.groupdocs.com/display/searchjava/Custom+text+extractors)

## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [CustomExtractorCollection()](#CustomExtractorCollection--) |  |
## Методы

| Метод | Описание |
| --- | --- |
|  | [size()](#size--) | Получает количество извлекателей, содержащихся в коллекции. |
|
|  | [isReadOnly()](#isReadOnly--) | Возвращает значение, указывающее, является ли коллекция только для чтения. |
|
|  | [iterator()](#iterator--) | Возвращает итератор для этой коллекции. |
|
|  | [addItem(IFieldExtractor extractor)](#addItem-com.groupdocs.search.common.IFieldExtractor-) | Добавляет извлекатель в коллекцию. |
|
|  | [clear()](#clear--) | Удаляет все извлекатели из коллекции. |
|
|  | [containsItem(IFieldExtractor item)](#containsItem-com.groupdocs.search.common.IFieldExtractor-) | Определяет, содержит ли коллекция конкретный извлекатель. |
|
|  | [copyToTArray(IFieldExtractor[] array, int arrayIndex)](#copyToTArray-com.groupdocs.search.common.IFieldExtractor---int-) | Копирует элементы коллекции в массив, начиная с определённого индекса массива. |
|
|  | [removeItem(IFieldExtractor extractor)](#removeItem-com.groupdocs.search.common.IFieldExtractor-) | Удаляет извлекатель из коллекции. |
|
### CustomExtractorCollection() {#CustomExtractorCollection--}
```
public CustomExtractorCollection()
```


### size() {#size--}
```
public abstract int size()
```


Получает количество извлекателей, содержащихся в коллекции.


**Returns:**
int — количество извлекателей, содержащихся в коллекции.

### isReadOnly() {#isReadOnly--}
```
public abstract boolean isReadOnly()
```


Возвращает значение, указывающее, является ли коллекция только для чтения.


**Returns:**
boolean — значение, указывающее, является ли коллекция только для чтения.

### iterator() {#iterator--}
```
public abstract Iterator<IFieldExtractor> iterator()
```


Возвращает итератор для этой коллекции.


**Returns:**
java.util.Iterator<com.groupdocs.search.common.IFieldExtractor> — объект‑итератор, который можно использовать для перебора элементов коллекции.

### addItem(IFieldExtractor extractor) {#addItem-com.groupdocs.search.common.IFieldExtractor-}
```
public abstract void addItem(IFieldExtractor extractor)
```


Добавляет извлекатель в коллекцию.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | extractor | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | Извлекатель, который следует добавить в коллекцию. |
|

### clear() {#clear--}
```
public abstract void clear()
```


Удаляет все извлекатели из коллекции.


### containsItem(IFieldExtractor item) {#containsItem-com.groupdocs.search.common.IFieldExtractor-}
```
public abstract boolean containsItem(IFieldExtractor item)
```


Определяет, содержит ли коллекция конкретный извлекатель.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | item | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | Извлекатель, который следует найти в коллекции. |
|

**Returns:**
boolean —  true  если  элемент  найден в коллекции; иначе  false .

### copyToTArray(IFieldExtractor[] array, int arrayIndex) {#copyToTArray-com.groupdocs.search.common.IFieldExtractor---int-}
```
public abstract void copyToTArray(IFieldExtractor[] array, int arrayIndex)
```


Копирует элементы коллекции в массив, начиная с определённого индекса массива.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | array | [IFieldExtractor\[\]](../../com.groupdocs.search.common/ifieldextractor) | Одномерный массив, который является получателем элементов, скопированных из коллекции. Массив должен использовать нулевую индексацию. |
|
|  | arrayIndex | int | Нулевой индекс в массиве, с которого начинается копирование. |
|

### removeItem(IFieldExtractor extractor) {#removeItem-com.groupdocs.search.common.IFieldExtractor-}
```
public abstract boolean removeItem(IFieldExtractor extractor)
```


Удаляет извлекатель из коллекции.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | extractor | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | Извлекатель, который следует удалить из коллекции. |
|

**Returns:**
boolean —  true  если  извлекатель  был успешно удалён из коллекции; иначе  false . Этот метод также возвращает  false , если  извлекатель  не найден в исходной коллекции.

