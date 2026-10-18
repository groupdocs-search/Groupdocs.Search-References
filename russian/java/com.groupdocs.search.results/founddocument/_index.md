---
title: "FoundDocument"
second_title: "GroupDocs.Search для Java API Reference"
description: "Представляет найденный документ."
type: docs
weight: 14
url: /ru/java/com.groupdocs.search.results/founddocument/
---
**Inheritance:**
java.lang.Object
```
public abstract class FoundDocument
```

Представляет найденный документ.


**Learn more**

* [Search results](../https://docs.groupdocs.com/display/searchjava/Search+results)

## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [FoundDocument()](#FoundDocument--) |  |
## Методы

| Метод | Описание |
| --- | --- |
|  | [getDocumentInfo()](#getDocumentInfo--) | Получает информацию о документе. |
|
|  | [getRelevance()](#getRelevance--) | Получает релевантность результата поиска. |
|
|  | [getOccurrenceCount()](#getOccurrenceCount--) | Получает количество найденных вхождений. |
|
|  | [getFoundFields()](#getFoundFields--) | Получает найденные поля документа. |
|
|  | [getTerms()](#getTerms--) | Получает найденные термины. |
|
|  | [getTermSequences()](#getTermSequences--) | Получает найденные последовательности терминов. |
|
|  | [getAttributes()](#getAttributes--) | Получает атрибуты, связанные с найденным документом. |
|
|  | [toString()](#toString--) | Возвращает строковое представление найденного документа. |
|
|  | [serialize()](#serialize--) | Сериализует текущий экземпляр в массив байтов. |
|
|  | [deserialize(byte[] array)](#deserialize-byte---) | Десериализует экземпляр из массива байтов. |
|
### FoundDocument() {#FoundDocument--}
```
public FoundDocument()
```


### getDocumentInfo() {#getDocumentInfo--}
```
public abstract DocumentInfo getDocumentInfo()
```


Получает информацию о документе.


**Returns:**
[DocumentInfo](../../com.groupdocs.search.results/documentinfo) - The document info.

### getRelevance() {#getRelevance--}
```
public abstract double getRelevance()
```


Получает релевантность результата поиска.


**Returns:**
double - Релевантность результата поиска.

### getOccurrenceCount() {#getOccurrenceCount--}
```
public abstract int getOccurrenceCount()
```


Получает количество найденных вхождений.


**Returns:**
int - Количество найденных вхождений.

### getFoundFields() {#getFoundFields--}
```
public abstract FoundDocumentField[] getFoundFields()
```


Получает найденные поля документа.


**Returns:**
com.groupdocs.search.results.FoundDocumentField[] - Найденные поля документа.

### getTerms() {#getTerms--}
```
public abstract String[] getTerms()
```


Получает найденные термы. Значение вычисляется каждый раз при доступе к свойству.


**Returns:**
java.lang.String[] - Найденные термины.

### getTermSequences() {#getTermSequences--}
```
public abstract String[][] getTermSequences()
```


Получает найденные последовательности терминов.


**Returns:**
java.lang.String[][] - Найденные последовательности терминов.

### getAttributes() {#getAttributes--}
```
public abstract String[] getAttributes()
```


Получает атрибуты, связанные с найденным документом. Соответствующая опция должна быть включена в параметрах поиска для получения атрибутов.


**Returns:**
java.lang.String[] - Атрибуты, связанные с найденным документом.

### toString() {#toString--}
```
public abstract String toString()
```


Возвращает строковое представление найденного документа.


**Returns:**
java.lang.String - Строка, представляющая найденный документ.

### serialize() {#serialize--}
```
public abstract byte[] serialize()
```


Сериализует текущий экземпляр в массив байтов.


**Returns:**
byte[] — массив байтов, представляющий текущий экземпляр.

### deserialize(byte[] array) {#deserialize-byte---}
```
public static FoundDocument deserialize(byte[] array)
```


Десериализует экземпляр из массива байтов.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | массив | byte[] | Массив байтов, из которого происходит десериализация. |
|

**Returns:**
[FoundDocument](../../com.groupdocs.search.results/founddocument) - An instance deserialized from a byte array.

