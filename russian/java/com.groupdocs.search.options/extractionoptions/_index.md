---
title: "ExtractionOptions"
second_title: "GroupDocs.Search для Java API Reference"
description: "Предоставляет параметры для извлечения данных из документов."
type: docs
weight: 18
url: /ru/java/com.groupdocs.search.options/extractionoptions/
---
**Inheritance:**
java.lang.Object
```
public class ExtractionOptions
```

Предоставляет параметры для извлечения данных из документов.

## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [ExtractionOptions()](#ExtractionOptions--) | Инициализирует новый экземпляр класса ExtractionOptions. |
|
|  | [ExtractionOptions(Object data)](#ExtractionOptions-java.lang.Object-) | Инициализирует новый экземпляр класса ExtractionOptions. |
|
|  | [ExtractionOptions(IndexingOptions options, IFieldExtractor customExtractor, IOcrConnector ocrConnector)](#ExtractionOptions-com.groupdocs.search.options.IndexingOptions-com.groupdocs.search.common.IFieldExtractor-com.groupdocs.search.options.IOcrConnector-) | Инициализирует новый экземпляр класса ExtractionOptions. |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getCustomExtractor()](#getCustomExtractor--) | Получает пользовательский извлекатель текста. |
|
|  | [setCustomExtractor(IFieldExtractor value)](#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-) | Устанавливает или устанавливает пользовательский извлекатель текста. |
|
|  | [getAutoDetectEncoding()](#getAutoDetectEncoding--) | Получает значение, указывающее, следует ли автоматически определять кодировку. |
|
|  | [setAutoDetectEncoding(boolean value)](#setAutoDetectEncoding-boolean-) | Устанавливает значение, указывающее, следует ли автоматически определять кодировку. |
|
|  | [getEncoding()](#getEncoding--) | Получает кодировку, используемую для извлечения текста из текстовых документов. |
|
|  | [setEncoding(String value)](#setEncoding-java.lang.String-) | Устанавливает кодировку, используемую для извлечения текста из текстовых документов. |
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
### ExtractionOptions() {#ExtractionOptions--}
```
public ExtractionOptions()
```


Инициализирует новый экземпляр класса ExtractionOptions.


### ExtractionOptions(Object data) {#ExtractionOptions-java.lang.Object-}
```
public ExtractionOptions(Object data)
```


Инициализирует новый экземпляр класса ExtractionOptions.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | данные | java.lang.Object | Сериализованные данные. |
|

### ExtractionOptions(IndexingOptions options, IFieldExtractor customExtractor, IOcrConnector ocrConnector) {#ExtractionOptions-com.groupdocs.search.options.IndexingOptions-com.groupdocs.search.common.IFieldExtractor-com.groupdocs.search.options.IOcrConnector-}
```
public ExtractionOptions(IndexingOptions options, IFieldExtractor customExtractor, IOcrConnector ocrConnector)
```


Инициализирует новый экземпляр класса ExtractionOptions.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | Параметры. |
|
|  | customExtractor | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | Пользовательский извлекатель. |
|
|  | ocrConnector | [IOcrConnector](../../com.groupdocs.search.options/iocrconnector) | OCR-коннектор. |
|

### getCustomExtractor() {#getCustomExtractor--}
```
public IFieldExtractor getCustomExtractor()
```


Получает пользовательский извлекатель текста. Значение по умолчанию — null.


**Returns:**
[IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) - The custom text extractor.

### setCustomExtractor(IFieldExtractor value) {#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-}
```
public void setCustomExtractor(IFieldExtractor value)
```


Устанавливает или устанавливает пользовательский извлекатель текста. Значение по умолчанию — null.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | value | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | Пользовательский извлекатель текста. |
|

### getAutoDetectEncoding() {#getAutoDetectEncoding--}
```
public boolean getAutoDetectEncoding()
```


Получает значение, указывающее, следует ли автоматически определять кодировку. Значение по умолчанию — false.


**Returns:**
boolean — значение, указывающее, следует ли автоматически определять кодировку.

### setAutoDetectEncoding(boolean value) {#setAutoDetectEncoding-boolean-}
```
public void setAutoDetectEncoding(boolean value)
```


Устанавливает значение, указывающее, следует ли автоматически определять кодировку. Значение по умолчанию — false.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | значение | boolean | Значение, указывающее, следует ли автоматически определять кодировку. |
|

### getEncoding() {#getEncoding--}
```
public String getEncoding()
```


Получает кодировку, используемую для извлечения текста из текстовых документов. Значение по умолчанию — null, что означает использование кодировки UTF-8 по умолчанию. Если AutoDetectEncoding равно true, то это значение используется как кодировка по умолчанию.


**Returns:**
java.lang.String — кодировка, используемая для извлечения текста из текстовых документов.

### setEncoding(String value) {#setEncoding-java.lang.String-}
```
public void setEncoding(String value)
```


Устанавливает кодировку, используемую для извлечения текста из текстовых документов. Значение по умолчанию — null, что означает использование кодировки UTF-8 по умолчанию. Если AutoDetectEncoding равно true, то это значение используется как кодировка по умолчанию.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | значение | java.lang.String | Кодировка, используемая для извлечения текста из текстовых документов. |
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
