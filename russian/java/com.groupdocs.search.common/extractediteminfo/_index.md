---
title: "ExtractedItemInfo"
second_title: "GroupDocs.Search для Java API Reference"
description: "Представляет информацию о элементе контейнера."
type: docs
weight: 18
url: /ru/java/com.groupdocs.search.common/extractediteminfo/
---
**Inheritance:**
java.lang.Object
```
public class ExtractedItemInfo
```

Представляет информацию о элементе контейнера.


**Learn more**

* [Custom text extractors](../https://docs.groupdocs.com/display/searchjava/Custom+text+extractors)

## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [ExtractedItemInfo(FormatFamily formatFamily, DocumentField[] fields, String itemInfo, String innerPath)](#ExtractedItemInfo-com.groupdocs.search.results.FormatFamily-com.groupdocs.search.common.DocumentField---java.lang.String-java.lang.String-) | Инициализирует новый экземпляр класса  ExtractedItemInfo . |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getFormatFamily()](#getFormatFamily--) | Получает тип документа. |
|
|  | [getFields()](#getFields--) | Получает извлечённые поля. |
|
|  | [getItemInfo()](#getItemInfo--) | Получает информацию об элементе. |
|
|  | [getInnerPath()](#getInnerPath--) | Получает внутренний путь. |
|
### ExtractedItemInfo(FormatFamily formatFamily, DocumentField[] fields, String itemInfo, String innerPath) {#ExtractedItemInfo-com.groupdocs.search.results.FormatFamily-com.groupdocs.search.common.DocumentField---java.lang.String-java.lang.String-}
```
public ExtractedItemInfo(FormatFamily formatFamily, DocumentField[] fields, String itemInfo, String innerPath)
```


Инициализирует новый экземпляр класса  ExtractedItemInfo .


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | formatFamily | [FormatFamily](../../com.groupdocs.search.results/formatfamily) | Семейство форматов документов. |
|
|  | fields | [DocumentField\[\]](../../com.groupdocs.search.common/documentfield) | Извлечённые поля. |
|
|  | itemInfo | java.lang.String | Информация об элементе. |
|
|  | innerPath | java.lang.String | Путь к элементу в контейнере. |
|

### getFormatFamily() {#getFormatFamily--}
```
public final FormatFamily getFormatFamily()
```


Получает тип документа.


**Returns:**
[FormatFamily](../../com.groupdocs.search.results/formatfamily) - The document type.

### getFields() {#getFields--}
```
public final DocumentField[] getFields()
```


Получает извлечённые поля.


**Returns:**
com.groupdocs.search.common.DocumentField[] - Извлечённые поля.

### getItemInfo() {#getItemInfo--}
```
public final String getItemInfo()
```


Получает информацию об элементе.


**Returns:**
java.lang.String - Информация об элементе.

### getInnerPath() {#getInnerPath--}
```
public final String getInnerPath()
```


Получает внутренний путь.


**Returns:**
java.lang.String - Внутренний путь.

