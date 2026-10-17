---
title: "ImageLocation"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "指定图像位置。"
type: docs
weight: 48
url: /zh/java/com.groupdocs.search.options/imagelocation/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum ImageLocation extends Enum<ImageLocation>
```

指定图像位置。

## Fields

| Field | 描述 |
| --- | --- |
|  | [Separate](#Separate) | 单独文件中的图像。 |
|
|  | [Embedded](#Embedded) | 嵌入到另一个文档中的图像。 |
|
|  | [ContainerItem](#ContainerItem) | 容器文件中作为元素的图像。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Separate {#Separate}
```
public static final ImageLocation Separate
```


单独文件中的图像。


### Embedded {#Embedded}
```
public static final ImageLocation Embedded
```


嵌入到另一个文档中的图像。


### ContainerItem {#ContainerItem}
```
public static final ImageLocation ContainerItem
```


容器文件中作为元素的图像。


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
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String |  |

**Returns:**
[ImageLocation](../../com.groupdocs.search.options/imagelocation)
