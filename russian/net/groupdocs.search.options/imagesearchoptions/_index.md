---
title: ImageSearchOptions
second_title: GroupDocs.Search для справочника API .NET
description: Предоставляет опции для обратного поиска изображения.
type: docs
weight: 880
url: /ru/net/groupdocs.search.options/imagesearchoptions/
---
## ImageSearchOptions class

Предоставляет опции для обратного поиска изображения.

```csharp
public class ImageSearchOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [ImageSearchOptions](imagesearchoptions)() | Инициализирует новый экземпляр[`ImageSearchOptions`](../imagesearchoptions) класс. |

## Характеристики

| Имя | Описание |
| --- | --- |
| [HashDifferences](../../groupdocs.search.options/imagesearchoptions/hashdifferences) { get; set; } | Получает или задает максимальное количество несовпадающих битов в хеше изображения. Значение по умолчанию:`5` . |
| [MaxResultCount](../../groupdocs.search.options/imagesearchoptions/maxresultcount) { get; set; } | Получает или задает максимальное количество найденных изображений для запроса обратного поиска изображения. Значение по умолчанию:`1000` . |
| [SearchDocumentFilter](../../groupdocs.search.options/imagesearchoptions/searchdocumentfilter) { get; set; } | Получает или задает фильтр документов поиска. [`SearchDocumentFilter`](./searchdocumentfilter) работает по логике включения. Использование[`SearchDocumentFilter`](../searchdocumentfilter) класс для создания экземпляров фильтра поискового документа. Значение по умолчанию:`нулевой` , а это значит, что будут возвращены все найденные документы. |

### Смотрите также

* пространство имен [GroupDocs.Search.Options](../../groupdocs.search.options)
* сборка [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->