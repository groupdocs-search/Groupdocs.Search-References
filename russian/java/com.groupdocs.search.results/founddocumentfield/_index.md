---
title: "FoundDocumentField"
second_title: "GroupDocs.Search для Java API Reference"
description: "Представляет найденное поле документа."
type: docs
weight: 15
url: /ru/java/com.groupdocs.search.results/founddocumentfield/
---
**Inheritance:**
java.lang.Object
```
public abstract class FoundDocumentField
```

Представляет найденное поле документа.


**Learn more**

* [Search results](../https://docs.groupdocs.com/display/searchjava/Search+results)

## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [FoundDocumentField()](#FoundDocumentField--) |  |
## Методы

| Метод | Описание |
| --- | --- |
|  | [getFieldName()](#getFieldName--) | Возвращает имя поля. |
|
|  | [getOccurrenceCount()](#getOccurrenceCount--) | Получает количество найденных вхождений. |
|
|  | [getTerms()](#getTerms--) | Получает найденные термины. |
|
|  | [getTermsOccurrences()](#getTermsOccurrences--) | Получает вхождения найденных терминов. |
|
|  | [getTermSequences()](#getTermSequences--) | Получает найденные последовательности терминов. |
|
|  | [getTermSequencesOccurrences()](#getTermSequencesOccurrences--) | Получает вхождения найденных последовательностей терминов. |
|
|  | [toString()](#toString--) | Возвращает строковое представление найденного поля документа. |
|
|  | [serialize()](#serialize--) | Сериализует текущий экземпляр в массив байтов. |
|
|  | [deserialize(byte[] array)](#deserialize-byte---) | Десериализует экземпляр из массива байтов. |
|
### FoundDocumentField() {#FoundDocumentField--}
```
public FoundDocumentField()
```


### getFieldName() {#getFieldName--}
```
public abstract String getFieldName()
```


Возвращает имя поля.


**Returns:**
java.lang.String - Имя поля.

### getOccurrenceCount() {#getOccurrenceCount--}
```
public abstract int getOccurrenceCount()
```


Получает количество найденных вхождений.


**Returns:**
int - Количество найденных вхождений.

### getTerms() {#getTerms--}
```
public abstract String[] getTerms()
```


Получает найденные термины.


**Returns:**
java.lang.String[] - Найденные термины.

### getTermsOccurrences() {#getTermsOccurrences--}
```
public abstract int[] getTermsOccurrences()
```


Получает вхождения найденных терминов.


**Returns:**
int[] - Вхождения найденных терминов.

### getTermSequences() {#getTermSequences--}
```
public abstract String[][] getTermSequences()
```


Получает найденные последовательности терминов.


**Returns:**
java.lang.String[][] - Найденные последовательности терминов.

### getTermSequencesOccurrences() {#getTermSequencesOccurrences--}
```
public abstract int[] getTermSequencesOccurrences()
```


Получает вхождения найденных последовательностей терминов.


**Returns:**
int[] - Вхождения найденных последовательностей терминов.

### toString() {#toString--}
```
public abstract String toString()
```


Возвращает строковое представление найденного поля документа.


**Returns:**
java.lang.String - Строка, представляющая найденное поле документа.

### serialize() {#serialize--}
```
public abstract byte[] serialize()
```


Сериализует текущий экземпляр в массив байтов.


**Returns:**
byte[] — массив байтов, представляющий текущий экземпляр.

### deserialize(byte[] array) {#deserialize-byte---}
```
public static FoundDocumentField deserialize(byte[] array)
```


Десериализует экземпляр из массива байтов.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | массив | byte[] | Массив байтов, из которого происходит десериализация. |
|

**Returns:**
[FoundDocumentField](../../com.groupdocs.search.results/founddocumentfield) - An instance deserialized from a byte array.

