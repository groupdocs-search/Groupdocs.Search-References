---
title: "DocumentImage"
second_title: "GroupDocs.Search для Java API Reference"
description: "Представляет данные изображения документа."
type: docs
weight: 16
url: /ru/java/com.groupdocs.search.common/documentimage/
---
**Inheritance:**
java.lang.Object
```
public abstract class DocumentImage
```

Представляет данные изображения документа.

## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [DocumentImage()](#DocumentImage--) |  |
## Методы

| Метод | Описание |
| --- | --- |
|  | [getImageIndex()](#getImageIndex--) | Возвращает порядковый номер изображения в документе. |
|
|  | [getFields()](#getFields--) | Получает извлечённые поля. |
|
|  | [getFrames()](#getFrames--) | Возвращает кадры изображения. |
|
### DocumentImage() {#DocumentImage--}
```
public DocumentImage()
```


### getImageIndex() {#getImageIndex--}
```
public abstract int getImageIndex()
```


Возвращает порядковый номер изображения в документе.


**Returns:**
int - Порядковый номер изображения в документе.

### getFields() {#getFields--}
```
public abstract DocumentField[] getFields()
```


Получает извлечённые поля.


**Returns:**
com.groupdocs.search.common.DocumentField[] - Извлечённые поля.

### getFrames() {#getFrames--}
```
public abstract ImageFrame[] getFrames()
```


Возвращает кадры изображения.


**Returns:**
com.groupdocs.search.common.ImageFrame[] - Кадры изображения.

