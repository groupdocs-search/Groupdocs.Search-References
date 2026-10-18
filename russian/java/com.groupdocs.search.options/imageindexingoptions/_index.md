---
title: "ImageIndexingOptions"
second_title: "GroupDocs.Search для Java API Reference"
description: "Предоставляет параметры индексирования изображений для обратного поиска изображений."
type: docs
weight: 23
url: /ru/java/com.groupdocs.search.options/imageindexingoptions/
---
**Inheritance:**
java.lang.Object
```
public abstract class ImageIndexingOptions
```

Предоставляет параметры индексирования изображений для обратного поиска изображений.

## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [ImageIndexingOptions()](#ImageIndexingOptions--) |  |
## Методы

| Метод | Описание |
| --- | --- |
|  | [getEnabledForSeparateImages()](#getEnabledForSeparateImages--) | Получает значение, указывающее, следует ли индексировать отдельные файлы изображений. |
|
|  | [setEnabledForSeparateImages(boolean value)](#setEnabledForSeparateImages-boolean-) | Устанавливает значение, указывающее, следует ли индексировать отдельные файлы изображений. |
|
|  | [getEnabledForContainerItemImages()](#getEnabledForContainerItemImages--) | Получает значение, указывающее, следует ли индексировать изображения, являющиеся элементами контейнера (например, изображения в ZIP-архиве). |
|
|  | [setEnabledForContainerItemImages(boolean value)](#setEnabledForContainerItemImages-boolean-) | Устанавливает значение, указывающее, следует ли индексировать изображения, являющиеся элементами контейнера (например, изображения в ZIP-архиве). |
|
|  | [getEnabledForEmbeddedImages()](#getEnabledForEmbeddedImages--) | Получает значение, указывающее, следует ли индексировать встроенные изображения (например, изображения в документе DOCX). |
|
|  | [setEnabledForEmbeddedImages(boolean value)](#setEnabledForEmbeddedImages-boolean-) | Устанавливает значение, указывающее, следует ли индексировать встроенные изображения (например, изображения в документе DOCX). |
|
### ImageIndexingOptions() {#ImageIndexingOptions--}
```
public ImageIndexingOptions()
```


### getEnabledForSeparateImages() {#getEnabledForSeparateImages--}
```
public abstract boolean getEnabledForSeparateImages()
```


Получает значение, указывающее, следует ли индексировать отдельные файлы изображений. Значение по умолчанию — false.


**Returns:**
boolean — Значение, указывающее, следует ли индексировать отдельные файлы изображений.

### setEnabledForSeparateImages(boolean value) {#setEnabledForSeparateImages-boolean-}
```
public abstract void setEnabledForSeparateImages(boolean value)
```


Устанавливает значение, указывающее, следует ли индексировать отдельные файлы изображений. Значение по умолчанию — false.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | значение | boolean | Значение, указывающее, следует ли индексировать отдельные файлы изображений. |
|

### getEnabledForContainerItemImages() {#getEnabledForContainerItemImages--}
```
public abstract boolean getEnabledForContainerItemImages()
```


Получает значение, указывающее, следует ли индексировать изображения, являющиеся элементами контейнера (например, изображения в ZIP-архиве). Значение по умолчанию — false.


**Returns:**
boolean - Значение, указывающее, следует ли индексировать изображения, которые являются элементами контейнера.

### setEnabledForContainerItemImages(boolean value) {#setEnabledForContainerItemImages-boolean-}
```
public abstract void setEnabledForContainerItemImages(boolean value)
```


Устанавливает значение, указывающее, следует ли индексировать изображения, которые являются элементами контейнера (например, изображения в ZIP‑архиве). Значение по умолчанию — false.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | значение | boolean | Значение, указывающее, следует ли индексировать изображения, которые являются элементами контейнера. |
|

### getEnabledForEmbeddedImages() {#getEnabledForEmbeddedImages--}
```
public abstract boolean getEnabledForEmbeddedImages()
```


Получает значение, указывающее, следует ли индексировать встроенные изображения (например, изображения в документе DOCX). Значение по умолчанию — false.


**Returns:**
boolean - Значение, указывающее, следует ли индексировать встроенные изображения.

### setEnabledForEmbeddedImages(boolean value) {#setEnabledForEmbeddedImages-boolean-}
```
public abstract void setEnabledForEmbeddedImages(boolean value)
```


Устанавливает значение, указывающее, следует ли индексировать встроенные изображения (например, изображения в документе DOCX). Значение по умолчанию — false.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | значение | boolean | Значение, указывающее, следует ли индексировать встроенные изображения. |
|

