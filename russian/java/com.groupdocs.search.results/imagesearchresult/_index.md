---
title: "ImageSearchResult"
second_title: "GroupDocs.Search для Java API Reference"
description: "Представляет результат обратного поиска изображения."
type: docs
weight: 17
url: /ru/java/com.groupdocs.search.results/imagesearchresult/
---
**Inheritance:**
java.lang.Object
```
public abstract class ImageSearchResult
```

Представляет результат обратного поиска изображения.

## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [ImageSearchResult()](#ImageSearchResult--) |  |
## Методы

| Метод | Описание |
| --- | --- |
|  | [getImageCount()](#getImageCount--) | Возвращает количество найденных изображений. |
|
|  | [getFoundImage(int index)](#getFoundImage-int-) | Возвращает найденное изображение по индексу. |
|
### ImageSearchResult() {#ImageSearchResult--}
```
public ImageSearchResult()
```


### getImageCount() {#getImageCount--}
```
public abstract int getImageCount()
```


Возвращает количество найденных изображений.


**Returns:**
int - Количество найденных изображений.

### getFoundImage(int index) {#getFoundImage-int-}
```
public abstract FoundImageFrame getFoundImage(int index)
```


Возвращает найденное изображение по индексу.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | индекс | int | Индекс найденного изображения. |
|

**Returns:**
[FoundImageFrame](../../com.groupdocs.search.results/foundimageframe) - The found image.

