---
title: "OcrIndexingOptions"
second_title: "GroupDocs.Search для Java API Reference"
description: "Предоставляет параметры для обработки OCR и индексирования распознанного текста."
type: docs
weight: 31
url: /ru/java/com.groupdocs.search.options/ocrindexingoptions/
---
**Inheritance:**
java.lang.Object
```
public abstract class OcrIndexingOptions
```

Предоставляет параметры для обработки OCR и индексирования распознанного текста.

## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [OcrIndexingOptions()](#OcrIndexingOptions--) |  |
## Методы

| Метод | Описание |
| --- | --- |
|  | [getEnabledForSeparateImages()](#getEnabledForSeparateImages--) | Получает значение, указывающее, следует ли распознавать текст в отдельных файлах изображений. |
|
|  | [setEnabledForSeparateImages(boolean value)](#setEnabledForSeparateImages-boolean-) | Устанавливает значение, указывающее, следует ли распознавать текст в отдельных файлах изображений. |
|
|  | [getEnabledForContainerItemImages()](#getEnabledForContainerItemImages--) | Получает значение, указывающее, следует ли распознавать текст на изображениях, являющихся элементами контейнера (например, изображения в ZIP‑архиве). |
|
|  | [setEnabledForContainerItemImages(boolean value)](#setEnabledForContainerItemImages-boolean-) | Устанавливает значение, указывающее, следует ли распознавать текст на изображениях, являющихся элементами контейнера (например, изображения в ZIP‑архиве). |
|
|  | [getEnabledForEmbeddedImages()](#getEnabledForEmbeddedImages--) | Получает значение, указывающее, следует ли распознавать текст во встроенных изображениях (например, изображения в документе DOCX). |
|
|  | [setEnabledForEmbeddedImages(boolean value)](#setEnabledForEmbeddedImages-boolean-) | Устанавливает значение, указывающее, следует ли распознавать текст во встроенных изображениях (например, изображения в документе DOCX). |
|
|  | [getOcrConnector()](#getOcrConnector--) | Получает OCR‑коннектор, используемый для обработки OCR. |
|
|  | [setOcrConnector(IOcrConnector value)](#setOcrConnector-com.groupdocs.search.options.IOcrConnector-) | Устанавливает OCR‑коннектор, используемый для обработки OCR. |
|
### OcrIndexingOptions() {#OcrIndexingOptions--}
```
public OcrIndexingOptions()
```


### getEnabledForSeparateImages() {#getEnabledForSeparateImages--}
```
public abstract boolean getEnabledForSeparateImages()
```


Получает значение, указывающее, следует ли распознавать текст в отдельных файлах изображений. Значение по умолчанию — false.


**Returns:**
boolean - Значение, указывающее, следует ли распознавать текст в отдельных файлах изображений.

### setEnabledForSeparateImages(boolean value) {#setEnabledForSeparateImages-boolean-}
```
public abstract void setEnabledForSeparateImages(boolean value)
```


Устанавливает значение, указывающее, следует ли распознавать текст в отдельных файлах изображений. Значение по умолчанию — false.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | значение | boolean | Значение, указывающее, следует ли распознавать текст в отдельных файлах изображений. |
|

### getEnabledForContainerItemImages() {#getEnabledForContainerItemImages--}
```
public abstract boolean getEnabledForContainerItemImages()
```


Получает значение, указывающее, следует ли распознавать текст на изображениях, являющихся элементами контейнера (например, изображения в ZIP‑архиве). Значение по умолчанию — false.


**Returns:**
boolean - Значение, указывающее, следует ли распознавать текст на изображениях, являющихся элементами контейнера.

### setEnabledForContainerItemImages(boolean value) {#setEnabledForContainerItemImages-boolean-}
```
public abstract void setEnabledForContainerItemImages(boolean value)
```


Устанавливает значение, указывающее, следует ли распознавать текст на изображениях, являющихся элементами контейнера (например, изображения в ZIP‑архиве). Значение по умолчанию — false.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | значение | boolean | Значение, указывающее, следует ли распознавать текст на изображениях, являющихся элементами контейнера. |
|

### getEnabledForEmbeddedImages() {#getEnabledForEmbeddedImages--}
```
public abstract boolean getEnabledForEmbeddedImages()
```


Получает значение, указывающее, следует ли распознавать текст во встроенных изображениях (например, изображения в документе DOCX). Значение по умолчанию — false.


**Returns:**
boolean - Значение, указывающее, следует ли распознавать текст во встроенных изображениях.

### setEnabledForEmbeddedImages(boolean value) {#setEnabledForEmbeddedImages-boolean-}
```
public abstract void setEnabledForEmbeddedImages(boolean value)
```


Устанавливает значение, указывающее, следует ли распознавать текст во встроенных изображениях (например, изображения в документе DOCX). Значение по умолчанию — false.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | значение | boolean | Значение, указывающее, следует ли распознавать текст во встроенных изображениях. |
|

### getOcrConnector() {#getOcrConnector--}
```
public abstract IOcrConnector getOcrConnector()
```


Получает OCR‑коннектор, используемый для обработки OCR. Значение по умолчанию — null, что означает отсутствие OCR.


**Returns:**
[IOcrConnector](../../com.groupdocs.search.options/iocrconnector) - An OCR connector that is used for OCR processing.

### setOcrConnector(IOcrConnector value) {#setOcrConnector-com.groupdocs.search.options.IOcrConnector-}
```
public abstract void setOcrConnector(IOcrConnector value)
```


Устанавливает OCR‑коннектор, используемый для обработки OCR. Значение по умолчанию — null, что означает отсутствие OCR.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | value | [IOcrConnector](../../com.groupdocs.search.options/iocrconnector) | OCR-коннектор, который используется для обработки OCR. |
|

