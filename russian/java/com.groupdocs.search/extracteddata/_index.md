---
title: "ExtractedData"
second_title: "GroupDocs.Search для Java API Reference"
description: "Представляет данные, полученные из документа и подготовленные для индексации."
type: docs
weight: 15
url: /ru/java/com.groupdocs.search/extracteddata/
---
**Inheritance:**
java.lang.Object
```
public class ExtractedData
```

Представляет данные, полученные из документа и подготовленные для индексации.

## Методы

| Метод | Описание |
| --- | --- |
|  | [serialize()](#serialize--) | Сериализует текущий экземпляр в массив байтов. |
|
|  | [deserialize(byte[] array)](#deserialize-byte---) | Десериализует экземпляр из массива байтов. |
|
### serialize() {#serialize--}
```
public final byte[] serialize()
```


Сериализует текущий экземпляр в массив байтов.


**Returns:**
byte[] — массив байтов, представляющий текущий экземпляр.

### deserialize(byte[] array) {#deserialize-byte---}
```
public static ExtractedData deserialize(byte[] array)
```


Десериализует экземпляр из массива байтов.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | массив | byte[] | Массив байтов, из которого происходит десериализация. |
|

**Returns:**
[ExtractedData](../../com.groupdocs.search/extracteddata) - An instance deserialized from a byte array.

