---
title: "UpdateOptions"
second_title: "GroupDocs.Search для Java API Reference"
description: "Предоставляет параметры для операции обновления."
type: docs
weight: 43
url: /ru/java/com.groupdocs.search.options/updateoptions/
---
**Inheritance:**
java.lang.Object
```
public class UpdateOptions
```

Предоставляет параметры для операции обновления.


**Learn more**

* [Update index](../https://docs.groupdocs.com/display/searchjava/Update+index)
* [Delete indexed paths](../https://docs.groupdocs.com/display/searchjava/Delete+indexed+paths)

## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [UpdateOptions()](#UpdateOptions--) | Инициализирует новый экземпляр класса  UpdateOptions  . |
|
|  | [UpdateOptions(Object data)](#UpdateOptions-java.lang.Object-) | Инициализирует новый экземпляр класса  UpdateOptions  . |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getThreads()](#getThreads--) | Получает количество потоков, используемых для индексации. |
|
|  | [setThreads(int value)](#setThreads-int-) | Устанавливает количество потоков, используемых для индексации. |
|
|  | [isAsync()](#isAsync--) | Получает флаг асинхронного выполнения операции. |
|
|  | [setAsync(boolean value)](#setAsync-boolean-) | Устанавливает флаг асинхронного выполнения операции. |
|
|  | [getCancellation()](#getCancellation--) | Получает объект отмены операции. |
|
|  | [setCancellation(Cancellation value)](#setCancellation-com.groupdocs.search.common.Cancellation-) | Устанавливает объект отмены операции. |
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
### UpdateOptions() {#UpdateOptions--}
```
public UpdateOptions()
```


Инициализирует новый экземпляр класса  UpdateOptions  .


### UpdateOptions(Object data) {#UpdateOptions-java.lang.Object-}
```
public UpdateOptions(Object data)
```


Инициализирует новый экземпляр класса  UpdateOptions  .


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | данные | java.lang.Object | Сериализованные данные. |
|

### getThreads() {#getThreads--}
```
public int getThreads()
```


Получает количество потоков, используемых для индексации. Значение по умолчанию — 1.


**Returns:**
int — количество потоков, используемых для индексации.

### setThreads(int value) {#setThreads-int-}
```
public void setThreads(int value)
```


Устанавливает количество потоков, используемых для индексации. Значение по умолчанию — 1.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | значение | int | Количество потоков, используемых для индексации. |
|

### isAsync() {#isAsync--}
```
public boolean isAsync()
```


Получает флаг асинхронного выполнения операции. Значение по умолчанию — false.


**Returns:**
boolean — флаг асинхронного выполнения операции.

### setAsync(boolean value) {#setAsync-boolean-}
```
public void setAsync(boolean value)
```


Устанавливает флаг асинхронного выполнения операции. Значение по умолчанию — false.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | значение | boolean | Флаг асинхронного выполнения операции. |
|

### getCancellation() {#getCancellation--}
```
public Cancellation getCancellation()
```


Получает объект отмены операции. Значение по умолчанию — null.


**Returns:**
[Cancellation](../../com.groupdocs.search.common/cancellation) - The operation cancellation object.

### setCancellation(Cancellation value) {#setCancellation-com.groupdocs.search.common.Cancellation-}
```
public void setCancellation(Cancellation value)
```


Устанавливает объект отмены операции. Значение по умолчанию — null.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | value | [Cancellation](../../com.groupdocs.search.common/cancellation) | Объект отмены операции. |
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
