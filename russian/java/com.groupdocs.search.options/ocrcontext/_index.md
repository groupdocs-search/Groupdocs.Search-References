---
title: "OcrContext"
second_title: "GroupDocs.Search для Java API Reference"
description: "Представляет контекст обработки OCR."
type: docs
weight: 30
url: /ru/java/com.groupdocs.search.options/ocrcontext/
---
**Inheritance:**
java.lang.Object
```
public class OcrContext
```

Представляет контекст обработки OCR.

## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [OcrContext(InputStream imageStream, ImageLocation imageLocation, String imageFileExtension)](#OcrContext-java.io.InputStream-com.groupdocs.search.options.ImageLocation-java.lang.String-) | Инициализирует новый экземпляр |
OcrContext
класс.
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getImageStream()](#getImageStream--) | Получает поток, содержащий изображение для обработки. |
|
|  | [getImageLocation()](#getImageLocation--) | Получает расположение изображения. |
|
|  | [getImageFileExtension()](#getImageFileExtension--) | Получает расширение файла изображения. |
|
### OcrContext(InputStream imageStream, ImageLocation imageLocation, String imageFileExtension) {#OcrContext-java.io.InputStream-com.groupdocs.search.options.ImageLocation-java.lang.String-}
```
public OcrContext(InputStream imageStream, ImageLocation imageLocation, String imageFileExtension)
```


Инициализирует новый экземпляр
OcrContext
класс.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | imageStream | java.io.InputStream | Поток, содержащий изображение для обработки. |
|
|  | imageLocation | [ImageLocation](../../com.groupdocs.search.options/imagelocation) | Расположение изображения. |
|
|  | imageFileExtension | java.lang.String | Расширение файла изображения. |
|

### getImageStream() {#getImageStream--}
```
public final InputStream getImageStream()
```


Получает поток, содержащий изображение для обработки.


**Returns:**
java.io.InputStream - Поток, содержащий изображение для обработки.

### getImageLocation() {#getImageLocation--}
```
public final ImageLocation getImageLocation()
```


Получает расположение изображения.


**Returns:**
[ImageLocation](../../com.groupdocs.search.options/imagelocation) - The location of the image.

### getImageFileExtension() {#getImageFileExtension--}
```
public final String getImageFileExtension()
```


Получает расширение файла изображения.
Это значение можно использовать для определения типа изображения.


**Returns:**
java.lang.String - Расширение файла изображения.

