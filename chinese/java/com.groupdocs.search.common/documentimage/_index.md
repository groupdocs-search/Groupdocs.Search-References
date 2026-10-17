---
title: "DocumentImage"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "表示文档图像数据。"
type: docs
weight: 16
url: /zh/java/com.groupdocs.search.common/documentimage/
---
**Inheritance:**
java.lang.Object
```
public abstract class DocumentImage
```

表示文档图像数据。

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [DocumentImage()](#DocumentImage--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getImageIndex()](#getImageIndex--) | 获取文档中图像的序号。 |
|
|  | [getFields()](#getFields--) | 获取提取的字段。 |
|
|  | [getFrames()](#getFrames--) | 获取图像帧。 |
|
### DocumentImage() {#DocumentImage--}
```
public DocumentImage()
```


### getImageIndex() {#getImageIndex--}
```
public abstract int getImageIndex()
```


获取文档中图像的序号。


**Returns:**
int - 文档中图像的序号。

### getFields() {#getFields--}
```
public abstract DocumentField[] getFields()
```


获取提取的字段。


**Returns:**
com.groupdocs.search.common.DocumentField[] - 提取的字段。

### getFrames() {#getFrames--}
```
public abstract ImageFrame[] getFrames()
```


获取图像帧。


**Returns:**
com.groupdocs.search.common.ImageFrame[] - 图像帧。

