---
title: "HighlightOptions"
second_title: "Справочник API GroupDocs.Search для .NET"
description: "Предоставляет параметры для подсветки найденных терминов."
type: docs
weight: 910
url: /ru/net/groupdocs.search.options/highlightoptions/
---
## HighlightOptions class

Предоставляет параметры для подсветки найденных терминов.

```csharp
public class HighlightOptions : TextOptions
```

## Конструкторы

| Name | Описание |
| --- | --- |
| [HighlightOptions](highlightoptions)() | Инициализирует новый экземпляр класса [`HighlightOptions`](../highlightoptions). |

## Properties

| Name | Описание |
| --- | --- |
| [AdditionalFields](../../groupdocs.search.options/textoptions/additionalfields) { get; set; } | Получает или задает дополнительные поля документа, использованные для индексации. Значение по умолчанию — `null`. Обратите внимание, что это значение используется только если текст документа не был сохранён в индексе. |
| [AutoDetectEncoding](../../groupdocs.search.options/baseoptions/autodetectencoding) { get; set; } | Получает или задает значение, указывающее, следует ли автоматически определять кодировку. Значение по умолчанию — `false`. |
| [Cancellation](../../groupdocs.search.options/textoptions/cancellation) { get; set; } | Получает или задает объект отмены. Значение по умолчанию — `null`. |
| [CustomExtractor](../../groupdocs.search.options/textoptions/customextractor) { get; set; } | Получает или задает пользовательский извлекатель текста, использованный для индексации. Значение по умолчанию — `null`. Обратите внимание, что это значение используется только если текст документа не был сохранён в индексе. |
| [Encoding](../../groupdocs.search.options/baseoptions/encoding) { get; set; } | Получает или задает кодировку, используемую для извлечения текста из текстовых документов. Значение по умолчанию — `null`, что означает использование кодировки UTF-8 по умолчанию. Если AutoDetectEncoding равно `true`, то это значение используется как кодировка по умолчанию. |
| [GenerateHead](../../groupdocs.search.options/textoptions/generatehead) { get; set; } | Получает или задает значение, указывающее, генерируется ли тег Head в выводимом HTML. Значение по умолчанию — `true`. |
| [HighlightColor](../../groupdocs.search.options/highlightoptions/highlightcolor) { get; set; } | Получает или задает цвет, используемый для подсветки вхождений. Значение по умолчанию — #FFD800. |
| [ImageIndexingOptions](../../groupdocs.search.options/baseoptions/imageindexingoptions) { get; } | Получает параметры индексирования изображений для обратного поиска изображений. |
| [MetadataIndexingOptions](../../groupdocs.search.options/baseoptions/metadataindexingoptions) { get; } | Получает параметры индексирования полей метаданных. |
| [OcrIndexingOptions](../../groupdocs.search.options/baseoptions/ocrindexingoptions) { get; } | Получает параметры обработки OCR и индексирования распознанного текста. |
| [TermHighlightEndTag](../../groupdocs.search.options/highlightoptions/termhighlightendtag) { get; set; } | Получает или задает конечный тег выделения найденного слова. Этот тег используется только при выделении в простом тексте. Значение по умолчанию — пустая строка. |
| [TermHighlightStartTag](../../groupdocs.search.options/highlightoptions/termhighlightstarttag) { get; set; } | Получает или задает начальный тег выделения найденного слова. Этот тег используется только при выделении в простом тексте. Значение по умолчанию — пустая строка. |
| [TermsAfter](../../groupdocs.search.options/highlightoptions/termsafter) { get; set; } | Получает или задает максимальное количество слов в текстовом фрагменте после выделенного слова. Значение должно быть в диапазоне от 0 до 10000. Значение по умолчанию — `7`. |
| [TermsBefore](../../groupdocs.search.options/highlightoptions/termsbefore) { get; set; } | Получает или задает максимальное количество слов в текстовом фрагменте перед выделенным словом. Значение должно быть в диапазоне от 0 до 10000. Значение по умолчанию — `7`. |
| [TermsTotal](../../groupdocs.search.options/highlightoptions/termstotal) { get; set; } | Получает или задает максимальное количество слов в текстовом фрагменте. Значение должно быть в диапазоне от 0 до 10000. Значение по умолчанию — `21`. |
| [UseBackupPrivilege](../../groupdocs.search.options/baseoptions/usebackupprivilege) { get; set; } | Получает или задает значение, указывающее, следует ли процессу использовать SeBackupPrivilege и FILE_FLAG_BACKUP_SEMANTICS для доступа к файлам и каталогам. Значение по умолчанию — `false`. |
| [UseInlineStyles](../../groupdocs.search.options/highlightoptions/useinlinestyles) { get; set; } | Получает или задает значение, указывающее, используются ли встроенные стили для выделения вхождений. Значение по умолчанию — `true`. |
| [UseRawTextExtraction](../../groupdocs.search.options/baseoptions/userawtextextraction) { get; set; } | Получает или задает значение, указывающее, используется ли необработанный режим для извлечения текста, если это возможно. Значение по умолчанию — `false`. Необработанный режим может значительно увеличить скорость индексирования, но обычный режим улучшает форматирование извлечённого текста. |

### Примечания

**Learn more**

* [Highlighting search results](https://docs.groupdocs.com/display/searchnet/Highlighting+search+results)

### См. также

* class [TextOptions](../textoptions)
* namespace [GroupDocs.Search.Options](../../groupdocs.search.options)
* assembly [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.search.dll -->
