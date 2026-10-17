---
title: "ImageIndexingOptions"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "提供反向图像搜索的图像索引选项。"
type: docs
weight: 23
url: /zh/java/com.groupdocs.search.options/imageindexingoptions/
---
**Inheritance:**
java.lang.Object
```
public abstract class ImageIndexingOptions
```

提供反向图像搜索的图像索引选项。

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [ImageIndexingOptions()](#ImageIndexingOptions--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getEnabledForSeparateImages()](#getEnabledForSeparateImages--) | 获取指示是否索引单独图像文件的值。 |
|
|  | [setEnabledForSeparateImages(boolean value)](#setEnabledForSeparateImages-boolean-) | 设置指示是否索引单独图像文件的值。 |
|
|  | [getEnabledForContainerItemImages()](#getEnabledForContainerItemImages--) | 获取指示是否索引容器中的图像项（例如 ZIP 存档中的图像）的值。 |
|
|  | [setEnabledForContainerItemImages(boolean value)](#setEnabledForContainerItemImages-boolean-) | 设置指示是否索引容器中的图像项（例如 ZIP 存档中的图像）的值。 |
|
|  | [getEnabledForEmbeddedImages()](#getEnabledForEmbeddedImages--) | 获取指示是否索引嵌入式图像（例如 DOCX 文档中的图像）的值。 |
|
|  | [setEnabledForEmbeddedImages(boolean value)](#setEnabledForEmbeddedImages-boolean-) | 设置指示是否索引嵌入式图像（例如 DOCX 文档中的图像）的值。 |
|
### ImageIndexingOptions() {#ImageIndexingOptions--}
```
public ImageIndexingOptions()
```


### getEnabledForSeparateImages() {#getEnabledForSeparateImages--}
```
public abstract boolean getEnabledForSeparateImages()
```


获取指示是否索引单独图像文件的值。默认值为 false。


**Returns:**
boolean - 指示是否索引单独图像文件的值。

### setEnabledForSeparateImages(boolean value) {#setEnabledForSeparateImages-boolean-}
```
public abstract void setEnabledForSeparateImages(boolean value)
```


设置指示是否索引单独图像文件的值。默认值为 false。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | boolean | 指示是否索引单独图像文件的值。 |
|

### getEnabledForContainerItemImages() {#getEnabledForContainerItemImages--}
```
public abstract boolean getEnabledForContainerItemImages()
```


获取指示是否索引容器中的图像项（例如 ZIP 存档中的图像）的值。默认值为 false。


**Returns:**
boolean - 表示是否索引容器中项目的图像的值。

### setEnabledForContainerItemImages(boolean value) {#setEnabledForContainerItemImages-boolean-}
```
public abstract void setEnabledForContainerItemImages(boolean value)
```


设置一个值，指示是否索引容器中项目的图像（例如 ZIP 存档中的图像）。默认值为 false。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | boolean | 表示是否索引容器中项目的图像的值。 |
|

### getEnabledForEmbeddedImages() {#getEnabledForEmbeddedImages--}
```
public abstract boolean getEnabledForEmbeddedImages()
```


获取一个值，指示是否索引嵌入的图像（例如 DOCX 文档中的图像）。默认值为 false。


**Returns:**
boolean - 表示是否索引嵌入图像的值。

### setEnabledForEmbeddedImages(boolean value) {#setEnabledForEmbeddedImages-boolean-}
```
public abstract void setEnabledForEmbeddedImages(boolean value)
```


设置一个值，指示是否索引嵌入的图像（例如 DOCX 文档中的图像）。默认值为 false。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | boolean | 表示是否索引嵌入图像的值。 |
|

