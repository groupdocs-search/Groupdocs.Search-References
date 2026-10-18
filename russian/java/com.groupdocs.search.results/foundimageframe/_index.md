---
title: "FoundImageFrame"
second_title: "GroupDocs.Search для Java API Reference"
description: "Представляет найденный кадр изображения."
type: docs
weight: 16
url: /ru/java/com.groupdocs.search.results/foundimageframe/
---
**Inheritance:**
java.lang.Object
```
public abstract class FoundImageFrame
```

Представляет найденный кадр изображения.

## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [FoundImageFrame()](#FoundImageFrame--) |  |
## Методы

| Метод | Описание |
| --- | --- |
|  | [getDocumentInfo()](#getDocumentInfo--) | Получает информацию о документе. |
|
|  | [getImageIndex()](#getImageIndex--) | Возвращает порядковый номер изображения в документе. |
|
|  | [getFrameIndex()](#getFrameIndex--) | Получает индекс кадра в изображении. |
|
|  | [getHashDifferences()](#getHashDifferences--) | Получает количество несовпадающих битов в хэше изображения. |
|
|  | [toString()](#toString--) | Возвращает System.String, представляющий текущий FoundImageFrame. |
|
### FoundImageFrame() {#FoundImageFrame--}
```
public FoundImageFrame()
```


### getDocumentInfo() {#getDocumentInfo--}
```
public abstract DocumentInfo getDocumentInfo()
```


Получает информацию о документе.


**Returns:**
[DocumentInfo](../../com.groupdocs.search.results/documentinfo) - The document info.

### getImageIndex() {#getImageIndex--}
```
public abstract int getImageIndex()
```


Возвращает порядковый номер изображения в документе.


**Returns:**
int - Порядковый номер изображения в документе.

### getFrameIndex() {#getFrameIndex--}
```
public abstract int getFrameIndex()
```


Получает индекс кадра в изображении.


**Returns:**
int - Индекс кадра в изображении.

### getHashDifferences() {#getHashDifferences--}
```
public abstract int getHashDifferences()
```


Получает количество несовпадающих битов в хэше изображения.


**Returns:**
int - Количество несовпадающих битов в хэше изображения.

### toString() {#toString--}
```
public abstract String toString()
```


Возвращает System.String, представляющий текущий FoundImageFrame.


**Returns:**
java.lang.String - System.String, представляющий текущий FoundImageFrame.

