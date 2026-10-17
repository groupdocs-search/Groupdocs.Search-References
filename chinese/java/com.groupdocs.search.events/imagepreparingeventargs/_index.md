---
title: "ImagePreparingEventArgs"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "表示图像准备开始事件的参数。"
type: docs
weight: 15
url: /zh/java/com.groupdocs.search.events/imagepreparingeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class ImagePreparingEventArgs extends BaseIndexEventArgs
```

表示图像准备开始事件的参数。


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getDocumentKey()](#getDocumentKey--) | 获取文档键。 |
|
|  | [getInnerPath()](#getInnerPath--) | 获取嵌套文档的内部路径。 |
|
|  | [getImageIndex()](#getImageIndex--) | 获取文档中图像的序号。 |
|
|  | [getImageFrames()](#getImageFrames--) | 获取图像帧。 |
|
|  | [getImageStream()](#getImageStream--) | 获取图像流。 |
|
### getDocumentKey() {#getDocumentKey--}
```
public final String getDocumentKey()
```


获取文档键。


**Returns:**
java.lang.String - 文档键。

### getInnerPath() {#getInnerPath--}
```
public final String[] getInnerPath()
```


获取嵌套文档的内部路径。


**Returns:**
java.lang.String[] - 嵌套文档的内部路径。

### getImageIndex() {#getImageIndex--}
```
public final int getImageIndex()
```


获取文档中图像的序号。


**Returns:**
int - 文档中图像的序号。

### getImageFrames() {#getImageFrames--}
```
public final ImageFrame[] getImageFrames()
```


获取图像帧。


**Returns:**
com.groupdocs.search.common.ImageFrame[] - 图像帧。

### getImageStream() {#getImageStream--}
```
public final InputStream getImageStream()
```


获取图像流。


**Returns:**
java.io.InputStream - 图像流。

