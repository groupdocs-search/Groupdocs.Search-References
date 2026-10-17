---
title: "OcrContext"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "表示 OCR 处理上下文。"
type: docs
weight: 30
url: /zh/java/com.groupdocs.search.options/ocrcontext/
---
**Inheritance:**
java.lang.Object
```
public class OcrContext
```

表示 OCR 处理上下文。

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [OcrContext(InputStream imageStream, ImageLocation imageLocation, String imageFileExtension)](#OcrContext-java.io.InputStream-com.groupdocs.search.options.ImageLocation-java.lang.String-) | 初始化一个新的实例 |
OcrContext
类。
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getImageStream()](#getImageStream--) | 获取包含待处理图像的流。 |
|
|  | [getImageLocation()](#getImageLocation--) | 获取图像的位置。 |
|
|  | [getImageFileExtension()](#getImageFileExtension--) | 获取图像的文件扩展名。 |
|
### OcrContext(InputStream imageStream, ImageLocation imageLocation, String imageFileExtension) {#OcrContext-java.io.InputStream-com.groupdocs.search.options.ImageLocation-java.lang.String-}
```
public OcrContext(InputStream imageStream, ImageLocation imageLocation, String imageFileExtension)
```


初始化一个新的实例
OcrContext
类。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | imageStream | java.io.InputStream | 包含待处理图像的流。 |
|
|  | imageLocation | [ImageLocation](../../com.groupdocs.search.options/imagelocation) | 图像的位置。 |
|
|  | imageFileExtension | java.lang.String | 图像的文件扩展名。 |
|

### getImageStream() {#getImageStream--}
```
public final InputStream getImageStream()
```


获取包含待处理图像的流。


**Returns:**
java.io.InputStream - 包含待处理图像的流。

### getImageLocation() {#getImageLocation--}
```
public final ImageLocation getImageLocation()
```


获取图像的位置。


**Returns:**
[ImageLocation](../../com.groupdocs.search.options/imagelocation) - The location of the image.

### getImageFileExtension() {#getImageFileExtension--}
```
public final String getImageFileExtension()
```


获取图像的文件扩展名。
此值可用于确定图像的类型。


**Returns:**
java.lang.String - 图像的文件扩展名。

