---
title: "TextOptions"
second_title: "GroupDocs.Search для Java API Reference"
description: "Предоставляет параметры для получения текста документа из индекса."
type: docs
weight: 41
url: /ru/java/com.groupdocs.search.options/textoptions/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.search.options.ITextOptions](../../com.groupdocs.search.options/itextoptions)
```
public class TextOptions implements ITextOptions
```

Предоставляет параметры для получения текста документа из индекса.


**Learn more**

* [Getting indexed documents](../https://docs.groupdocs.com/display/searchjava/Getting+indexed+documents)
* [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)

## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [TextOptions()](#TextOptions--) | Инициализирует новый экземпляр класса TextOptions. |
|
|  | [TextOptions(Object data)](#TextOptions-java.lang.Object-) | Инициализирует новый экземпляр класса TextOptions. |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getCustomExtractor()](#getCustomExtractor--) | Получает пользовательский извлекатель текста, использованный для индексации. |
|
|  | [setCustomExtractor(IFieldExtractor value)](#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-) | Устанавливает пользовательский извлекатель текста, использованный для индексации. |
|
|  | [getAdditionalFields()](#getAdditionalFields--) | Получает дополнительные поля документа, которые использовались для индексации. |
|
|  | [setAdditionalFields(DocumentField[] value)](#setAdditionalFields-com.groupdocs.search.common.DocumentField---) | Устанавливает дополнительные поля документа, которые использовались для индексации. |
|
|  | [getCancellation()](#getCancellation--) | Получает объект отмены. |
|
|  | [setCancellation(Cancellation value)](#setCancellation-com.groupdocs.search.common.Cancellation-) | Устанавливает объект отмены. |
|
|  | [getGenerateHead()](#getGenerateHead--) | Получает значение, указывающее, генерируется ли тег Head в выходном HTML. |
|
|  | [setGenerateHead(boolean value)](#setGenerateHead-boolean-) | Устанавливает значение, указывающее, генерируется ли тег Head в выходном HTML. |
|
|  | [getUseRawTextExtraction()](#getUseRawTextExtraction--) | Получает значение, указывающее, используется ли необработанный режим для извлечения текста, если это возможно. |
|
|  | [setUseRawTextExtraction(boolean value)](#setUseRawTextExtraction-boolean-) | Устанавливает значение, указывающее, используется ли необработанный режим для извлечения текста, если это возможно. |
|
|  | [getMetadataIndexingOptions()](#getMetadataIndexingOptions--) | Получает параметры индексации полей метаданных. |
|
|  | [getOcrIndexingOptions()](#getOcrIndexingOptions--) | Получает параметры обработки OCR и индексации распознанного текста. |
|
|  | [getImageIndexingOptions()](#getImageIndexingOptions--) | Получает параметры индексации изображений для обратного поиска изображений. |
|
| [getCore()](#getCore--) |  |
### TextOptions() {#TextOptions--}
```
public TextOptions()
```


Инициализирует новый экземпляр класса TextOptions.


### TextOptions(Object data) {#TextOptions-java.lang.Object-}
```
public TextOptions(Object data)
```


Инициализирует новый экземпляр класса TextOptions.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | данные | java.lang.Object | Сериализованные данные. |
|

### getCustomExtractor() {#getCustomExtractor--}
```
public IFieldExtractor getCustomExtractor()
```


Получает пользовательский извлекатель текста, который использовался для индексации. Значение по умолчанию — `null`. Обратите внимание, что это значение используется только если текст документа не был сохранён в индексе.


**Returns:**
[IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) - The custom text extractor that was used for indexing.

### setCustomExtractor(IFieldExtractor value) {#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-}
```
public void setCustomExtractor(IFieldExtractor value)
```


Устанавливает пользовательский извлекатель текста, который использовался для индексации. Значение по умолчанию — `null`. Обратите внимание, что это значение используется только если текст документа не был сохранён в индексе.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | value | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | Пользовательский извлекатель текста, который использовался для индексации. |
|

### getAdditionalFields() {#getAdditionalFields--}
```
public DocumentField[] getAdditionalFields()
```


Получает дополнительные поля документа, которые использовались для индексации. Значение по умолчанию — `null`. Обратите внимание, что это значение используется только если текст документа не был сохранён в индексе.


**Returns:**
com.groupdocs.search.common.DocumentField[] - Дополнительные поля документа, которые использовались для индексации.

### setAdditionalFields(DocumentField[] value) {#setAdditionalFields-com.groupdocs.search.common.DocumentField---}
```
public void setAdditionalFields(DocumentField[] value)
```


Устанавливает дополнительные поля документа, которые использовались для индексации. Значение по умолчанию — `null`. Обратите внимание, что это значение используется только если текст документа не был сохранён в индексе.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | value | [DocumentField\[\]](../../com.groupdocs.search.common/documentfield) | Дополнительные поля документа, которые использовались для индексации. |
|

### getCancellation() {#getCancellation--}
```
public Cancellation getCancellation()
```


Получает объект отмены. Значение по умолчанию — `null`.


**Returns:**
[Cancellation](../../com.groupdocs.search.common/cancellation) - The cancellation object.

### setCancellation(Cancellation value) {#setCancellation-com.groupdocs.search.common.Cancellation-}
```
public void setCancellation(Cancellation value)
```


Устанавливает объект отмены. Значение по умолчанию — `null`.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | value | [Cancellation](../../com.groupdocs.search.common/cancellation) | Объект отмены. |
|

### getGenerateHead() {#getGenerateHead--}
```
public boolean getGenerateHead()
```


Получает значение, указывающее, генерируется ли тег Head в выходном HTML. Значение по умолчанию — `true`.


**Returns:**
boolean - Значение, указывающее, генерируется ли тег Head в выходном HTML.

### setGenerateHead(boolean value) {#setGenerateHead-boolean-}
```
public void setGenerateHead(boolean value)
```


Устанавливает значение, указывающее, генерируется ли тег Head в выходном HTML. Значение по умолчанию — `true`.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | значение | boolean | Значение, указывающее, генерируется ли тег Head в выходном HTML. |
|

### getUseRawTextExtraction() {#getUseRawTextExtraction--}
```
public boolean getUseRawTextExtraction()
```


Получает значение, указывающее, используется ли необработанный режим для извлечения текста, если это возможно. Значение по умолчанию —  true . Необработанный режим может значительно увеличить скорость индексации, но обычный режим улучшает форматирование извлечённого текста.


**Returns:**
boolean - Значение, указывающее, используется ли необработанный режим для извлечения текста, если это возможно.

### setUseRawTextExtraction(boolean value) {#setUseRawTextExtraction-boolean-}
```
public void setUseRawTextExtraction(boolean value)
```


Устанавливает значение, указывающее, используется ли необработанный режим для извлечения текста, если это возможно. Значение по умолчанию —  true . Необработанный режим может значительно увеличить скорость индексации, но обычный режим улучшает форматирование извлечённого текста.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | значение | boolean | Значение, указывающее, используется ли необработанный режим для извлечения текста, если это возможно. |
|

### getMetadataIndexingOptions() {#getMetadataIndexingOptions--}
```
public MetadataIndexingOptions getMetadataIndexingOptions()
```


Получает параметры индексации полей метаданных.


**Returns:**
[MetadataIndexingOptions](../../com.groupdocs.search.options/metadataindexingoptions) - The options for indexing metadata fields.

### getOcrIndexingOptions() {#getOcrIndexingOptions--}
```
public OcrIndexingOptions getOcrIndexingOptions()
```


Получает параметры обработки OCR и индексации распознанного текста.


**Returns:**
[OcrIndexingOptions](../../com.groupdocs.search.options/ocrindexingoptions) - The options for OCR processing and indexing recognized text.

### getImageIndexingOptions() {#getImageIndexingOptions--}
```
public ImageIndexingOptions getImageIndexingOptions()
```


Получает параметры индексации изображений для обратного поиска изображений.


**Returns:**
[ImageIndexingOptions](../../com.groupdocs.search.options/imageindexingoptions) - The image indexing options for reverse image search.

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
