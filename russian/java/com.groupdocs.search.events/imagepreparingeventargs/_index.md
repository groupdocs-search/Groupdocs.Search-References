---
title: "ImagePreparingEventArgs"
second_title: "GroupDocs.Search для Java API Reference"
description: "Представляет аргументы события начала подготовки изображения."
type: docs
weight: 15
url: /ru/java/com.groupdocs.search.events/imagepreparingeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class ImagePreparingEventArgs extends BaseIndexEventArgs
```

Представляет аргументы события начала подготовки изображения.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Методы

| Метод | Описание |
| --- | --- |
|  | [getDocumentKey()](#getDocumentKey--) | Получает ключ документа. |
|
|  | [getInnerPath()](#getInnerPath--) | Возвращает внутренний путь вложенного документа. |
|
|  | [getImageIndex()](#getImageIndex--) | Возвращает порядковый номер изображения в документе. |
|
|  | [getImageFrames()](#getImageFrames--) | Возвращает кадры изображения. |
|
|  | [getImageStream()](#getImageStream--) | Возвращает поток изображения. |
|
### getDocumentKey() {#getDocumentKey--}
```
public final String getDocumentKey()
```


Получает ключ документа.


**Returns:**
java.lang.String - Ключ документа.

### getInnerPath() {#getInnerPath--}
```
public final String[] getInnerPath()
```


Возвращает внутренний путь вложенного документа.


**Returns:**
java.lang.String[] - Внутренний путь вложенного документа.

### getImageIndex() {#getImageIndex--}
```
public final int getImageIndex()
```


Возвращает порядковый номер изображения в документе.


**Returns:**
int - Порядковый номер изображения в документе.

### getImageFrames() {#getImageFrames--}
```
public final ImageFrame[] getImageFrames()
```


Возвращает кадры изображения.


**Returns:**
com.groupdocs.search.common.ImageFrame[] - Кадры изображения.

### getImageStream() {#getImageStream--}
```
public final InputStream getImageStream()
```


Возвращает поток изображения.


**Returns:**
java.io.InputStream - Поток изображения.

