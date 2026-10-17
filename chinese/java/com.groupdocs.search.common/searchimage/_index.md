---
title: "SearchImage"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "表示用于搜索的图像。"
type: docs
weight: 29
url: /zh/java/com.groupdocs.search.common/searchimage/
---
**Inheritance:**
java.lang.Object
```
public abstract class SearchImage
```

表示用于搜索的图像。

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [SearchImage()](#SearchImage--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [create(String filePath)](#create-java.lang.String-) | 从文件创建用于搜索的图像。 |
|
|  | [create(String filePath, int imageIndex)](#create-java.lang.String-int-) | 从文件创建用于搜索的图像。 |
|
|  | [create(InputStream stream)](#create-java.io.InputStream-) | 从流创建用于搜索的图像。 |
|
|  | [create(InputStream stream, int imageIndex)](#create-java.io.InputStream-int-) | 从流创建用于搜索的图像。 |
|
### SearchImage() {#SearchImage--}
```
public SearchImage()
```


### create(String filePath) {#create-java.lang.String-}
```
public static SearchImage create(String filePath)
```


从文件创建用于搜索的图像。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 文件路径 | java.lang.String | 图像文件路径。 |
|

**Returns:**
[SearchImage](../../com.groupdocs.search.common/searchimage) - An image to search.

### create(String filePath, int imageIndex) {#create-java.lang.String-int-}
```
public static SearchImage create(String filePath, int imageIndex)
```


从文件创建用于搜索的图像。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 文件路径 | java.lang.String | 图像文件路径。 |
|
|  | imageIndex | int | 多页图像中的图像索引。 |
|

**Returns:**
[SearchImage](../../com.groupdocs.search.common/searchimage) - An image to search.

### create(InputStream stream) {#create-java.io.InputStream-}
```
public static SearchImage create(InputStream stream)
```


从流创建用于搜索的图像。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 流 | java.io.InputStream | 图像流。 |
|

**Returns:**
[SearchImage](../../com.groupdocs.search.common/searchimage) - An image to search.

### create(InputStream stream, int imageIndex) {#create-java.io.InputStream-int-}
```
public static SearchImage create(InputStream stream, int imageIndex)
```


从流创建用于搜索的图像。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 流 | java.io.InputStream | 图像流。 |
|
|  | imageIndex | int | 多页图像中的图像索引。 |
|

**Returns:**
[SearchImage](../../com.groupdocs.search.common/searchimage) - An image to search.

