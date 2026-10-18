---
title: "ImageLocation"
second_title: "GroupDocs.Search для Java API Reference"
description: "Указывает расположение изображения."
type: docs
weight: 48
url: /ru/java/com.groupdocs.search.options/imagelocation/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum ImageLocation extends Enum<ImageLocation>
```

Указывает расположение изображения.

## Fields

| Field | Описание |
| --- | --- |
|  | [Separate](#Separate) | Изображение в отдельном файле. |
|
|  | [Embedded](#Embedded) | Изображение, встроенное в другой документ. |
|
|  | [ContainerItem](#ContainerItem) | Изображение, являющееся элементом в контейнерном файле. |
|
## Методы

| Метод | Описание |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Separate {#Separate}
```
public static final ImageLocation Separate
```


Изображение в отдельном файле.


### Embedded {#Embedded}
```
public static final ImageLocation Embedded
```


Изображение, встроенное в другой документ.


### ContainerItem {#ContainerItem}
```
public static final ImageLocation ContainerItem
```


Изображение, являющееся элементом в контейнерном файле.


### values() {#values--}
```
public static ImageLocation[] values()
```




**Returns:**
com.groupdocs.search.options.ImageLocation[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static ImageLocation valueOf(String name)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| имя | java.lang.String |  |

**Returns:**
[ImageLocation](../../com.groupdocs.search.options/imagelocation)
