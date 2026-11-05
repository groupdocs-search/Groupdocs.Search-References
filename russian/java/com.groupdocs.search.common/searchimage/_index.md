---
title: "SearchImage"
second_title: "GroupDocs.Search для Java API Reference"
description: "Представляет изображение для поиска."
type: docs
weight: 29
url: /ru/java/com.groupdocs.search.common/searchimage/
---
**Inheritance:**
java.lang.Object
```
public abstract class SearchImage
```

Представляет изображение для поиска.

## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [SearchImage()](#SearchImage--) |  |
## Методы

| Метод | Описание |
| --- | --- |
|  | [create(String filePath)](#create-java.lang.String-) | Создаёт изображение из файла для поиска. |
|
|  | [create(String filePath, int imageIndex)](#create-java.lang.String-int-) | Создаёт изображение из файла для поиска. |
|
|  | [create(InputStream stream)](#create-java.io.InputStream-) | Создаёт изображение из потока для поиска. |
|
|  | [create(InputStream stream, int imageIndex)](#create-java.io.InputStream-int-) | Создаёт изображение из потока для поиска. |
|
### SearchImage() {#SearchImage--}
```
public SearchImage()
```


### create(String filePath) {#create-java.lang.String-}
```
public static SearchImage create(String filePath)
```


Создаёт изображение из файла для поиска.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | filePath | java.lang.String | Путь к файлу изображения. |
|

**Returns:**
[SearchImage](../../com.groupdocs.search.common/searchimage) - An image to search.

### create(String filePath, int imageIndex) {#create-java.lang.String-int-}
```
public static SearchImage create(String filePath, int imageIndex)
```


Создаёт изображение из файла для поиска.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | filePath | java.lang.String | Путь к файлу изображения. |
|
|  | imageIndex | int | Индекс изображения в многостраничных изображениях. |
|

**Returns:**
[SearchImage](../../com.groupdocs.search.common/searchimage) - An image to search.

### create(InputStream stream) {#create-java.io.InputStream-}
```
public static SearchImage create(InputStream stream)
```


Создаёт изображение из потока для поиска.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | stream | java.io.InputStream | Поток изображения. |
|

**Returns:**
[SearchImage](../../com.groupdocs.search.common/searchimage) - An image to search.

### create(InputStream stream, int imageIndex) {#create-java.io.InputStream-int-}
```
public static SearchImage create(InputStream stream, int imageIndex)
```


Создаёт изображение из потока для поиска.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | stream | java.io.InputStream | Поток изображения. |
|
|  | imageIndex | int | Индекс изображения в многостраничных изображениях. |
|

**Returns:**
[SearchImage](../../com.groupdocs.search.common/searchimage) - An image to search.

