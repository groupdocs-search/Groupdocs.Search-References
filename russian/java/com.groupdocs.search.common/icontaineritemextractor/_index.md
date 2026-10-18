---
title: "IContainerItemExtractor"
second_title: "GroupDocs.Search для Java API Reference"
description: "Предоставляет методы для извлечения элементов из контейнерных документов."
type: docs
weight: 35
url: /ru/java/com.groupdocs.search.common/icontaineritemextractor/
---
**All Implemented Interfaces:**
[com.groupdocs.search.common.IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor)
```
public interface IContainerItemExtractor extends IFieldExtractor
```

Предоставляет методы для извлечения элементов из контейнерных документов.


**Learn more**

* [Custom text extractors](../https://docs.groupdocs.com/display/searchjava/Custom+text+extractors)

## Методы

| Метод | Описание |
| --- | --- |
|  | [getFormatFamily()](#getFormatFamily--) | Получает семейство форматов документа. |
|
|  | [getContainerItems(String filePath)](#getContainerItems-java.lang.String-) | Извлекает элементы из контейнерного документа. |
|
|  | [getContainerItems(InputStream stream)](#getContainerItems-java.io.InputStream-) | Извлекает элементы из контейнерного документа. |
|
### getFormatFamily() {#getFormatFamily--}
```
public abstract FormatFamily getFormatFamily()
```


Получает семейство форматов документа.


**Returns:**
[FormatFamily](../../com.groupdocs.search.results/formatfamily) - The document format family.

### getContainerItems(String filePath) {#getContainerItems-java.lang.String-}
```
public abstract ExtractedItemInfo[] getContainerItems(String filePath)
```


Извлекает элементы из контейнерного документа.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | filePath | java.lang.String | Путь к файлу. |
|

**Returns:**
com.groupdocs.search.common.ExtractedItemInfo[] - Массив извлечённых элементов.

### getContainerItems(InputStream stream) {#getContainerItems-java.io.InputStream-}
```
public abstract ExtractedItemInfo[] getContainerItems(InputStream stream)
```


Извлекает элементы из контейнерного документа.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | stream | java.io.InputStream | Поток документа. |
|

**Returns:**
com.groupdocs.search.common.ExtractedItemInfo[] - Массив извлечённых элементов.

