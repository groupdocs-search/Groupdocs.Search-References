---
title: "ExtractorSettings"
second_title: "GroupDocs.Search для Java API Reference"
description: "Содержит настройки экстрактора данных документа."
type: docs
weight: 19
url: /ru/java/com.groupdocs.search.common/extractorsettings/
---
**Inheritance:**
java.lang.Object
```
public abstract class ExtractorSettings
```

Содержит настройки экстрактора данных документа.

## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [ExtractorSettings()](#ExtractorSettings--) |  |
## Методы

| Метод | Описание |
| --- | --- |
|  | [getIndexType()](#getIndexType--) | Получает тип индекса, для которого используется извлекатель. |
|
|  | [setIndexType(IndexType value)](#setIndexType-com.groupdocs.search.options.IndexType-) | Устанавливает тип индекса, для которого используется извлекатель. |
|
### ExtractorSettings() {#ExtractorSettings--}
```
public ExtractorSettings()
```


### getIndexType() {#getIndexType--}
```
public abstract IndexType getIndexType()
```


Получает тип индекса, для которого используется извлекатель. Значение по умолчанию — GroupDocs.Search.Options.IndexType.NormalIndex.


**Returns:**
[IndexType](../../com.groupdocs.search.options/indextype) - The index type the extractor is used for.

### setIndexType(IndexType value) {#setIndexType-com.groupdocs.search.options.IndexType-}
```
public abstract void setIndexType(IndexType value)
```


Устанавливает тип индекса, для которого используется извлекатель. Значение по умолчанию — GroupDocs.Search.Options.IndexType.NormalIndex.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | value | [IndexType](../../com.groupdocs.search.options/indextype) | Тип индекса, для которого используется извлекатель. |
|

