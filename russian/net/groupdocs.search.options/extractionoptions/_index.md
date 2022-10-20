---
title: ExtractionOptions
second_title: GroupDocs.Search для справочника API .NET
description: Предоставляет опции для извлечения данных из документов.
type: docs
weight: 790
url: /ru/net/groupdocs.search.options/extractionoptions/
---
## ExtractionOptions class

Предоставляет опции для извлечения данных из документов.

```csharp
public class ExtractionOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [ExtractionOptions](extractionoptions)() | Инициализирует новый экземпляр[`ExtractionOptions`](../extractionoptions) класс. |

## Характеристики

| Имя | Описание |
| --- | --- |
| [CustomExtractor](../../groupdocs.search.options/extractionoptions/customextractor) { get; set; } | Получает или задает пользовательский экстрактор текста. Значение по умолчанию:`нулевой` . |
| [Encoding](../../groupdocs.search.options/extractionoptions/encoding) { get; set; } | Получает или задает кодировку, используемую для извлечения из текстовых документов. |
| [ImageIndexingOptions](../../groupdocs.search.options/extractionoptions/imageindexingoptions) { get; } | Получает параметры индексации изображения для обратного поиска изображения. |
| [MetadataIndexingOptions](../../groupdocs.search.options/extractionoptions/metadataindexingoptions) { get; } | Получает параметры для индексации полей метаданных. |
| [OcrIndexingOptions](../../groupdocs.search.options/extractionoptions/ocrindexingoptions) { get; } | Получает параметры обработки OCR и индексации распознанного текста. |
| [UseRawTextExtraction](../../groupdocs.search.options/extractionoptions/userawtextextraction) { get; set; } | Получает или задает значение, указывающее, используется ли необработанный режим для извлечения текста, если это возможно. Значение по умолчанию:`истинный` . Необработанный режим может значительно увеличить скорость индексации, но обычный режим улучшает форматирование извлеченного текста. |

### Смотрите также

* пространство имен [GroupDocs.Search.Options](../../groupdocs.search.options)
* сборка [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->