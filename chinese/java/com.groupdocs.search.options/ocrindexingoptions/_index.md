---
title: "OcrIndexingOptions"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "提供 OCR 处理和索引已识别文本的选项。"
type: docs
weight: 31
url: /zh/java/com.groupdocs.search.options/ocrindexingoptions/
---
**Inheritance:**
java.lang.Object
```
public abstract class OcrIndexingOptions
```

提供 OCR 处理和索引已识别文本的选项。

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [OcrIndexingOptions()](#OcrIndexingOptions--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getEnabledForSeparateImages()](#getEnabledForSeparateImages--) | 获取指示是否在单独的图像文件中识别文本的值。 |
|
|  | [setEnabledForSeparateImages(boolean value)](#setEnabledForSeparateImages-boolean-) | 设置指示是否在单独的图像文件中识别文本的值。 |
|
|  | [getEnabledForContainerItemImages()](#getEnabledForContainerItemImages--) | 获取指示是否在容器中的图像项（例如 ZIP 存档中的图像）中识别文本的值。 |
|
|  | [setEnabledForContainerItemImages(boolean value)](#setEnabledForContainerItemImages-boolean-) | 设置指示是否在容器中的图像项（例如 ZIP 存档中的图像）中识别文本的值。 |
|
|  | [getEnabledForEmbeddedImages()](#getEnabledForEmbeddedImages--) | 获取指示是否在嵌入的图像（例如 DOCX 文档中的图像）中识别文本的值。 |
|
|  | [setEnabledForEmbeddedImages(boolean value)](#setEnabledForEmbeddedImages-boolean-) | 设置指示是否在嵌入的图像（例如 DOCX 文档中的图像）中识别文本的值。 |
|
|  | [getOcrConnector()](#getOcrConnector--) | 获取用于 OCR 处理的 OCR 连接器。 |
|
|  | [setOcrConnector(IOcrConnector value)](#setOcrConnector-com.groupdocs.search.options.IOcrConnector-) | 设置用于 OCR 处理的 OCR 连接器。 |
|
### OcrIndexingOptions() {#OcrIndexingOptions--}
```
public OcrIndexingOptions()
```


### getEnabledForSeparateImages() {#getEnabledForSeparateImages--}
```
public abstract boolean getEnabledForSeparateImages()
```


获取指示是否在单独的图像文件中识别文本的值。默认值为 false。


**Returns:**
boolean - 指示是否在单独的图像文件中识别文本的值。

### setEnabledForSeparateImages(boolean value) {#setEnabledForSeparateImages-boolean-}
```
public abstract void setEnabledForSeparateImages(boolean value)
```


设置指示是否在单独的图像文件中识别文本的值。默认值为 false。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | boolean | 指示是否在单独的图像文件中识别文本的值。 |
|

### getEnabledForContainerItemImages() {#getEnabledForContainerItemImages--}
```
public abstract boolean getEnabledForContainerItemImages()
```


获取指示是否在容器中的图像项（例如 ZIP 存档中的图像）中识别文本的值。默认值为 false。


**Returns:**
boolean - 指示是否在容器中的图像项中识别文本的值。

### setEnabledForContainerItemImages(boolean value) {#setEnabledForContainerItemImages-boolean-}
```
public abstract void setEnabledForContainerItemImages(boolean value)
```


设置指示是否在容器中的图像项（例如 ZIP 存档中的图像）中识别文本的值。默认值为 false。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | boolean | 指示是否在容器中的图像项中识别文本的值。 |
|

### getEnabledForEmbeddedImages() {#getEnabledForEmbeddedImages--}
```
public abstract boolean getEnabledForEmbeddedImages()
```


获取指示是否在嵌入的图像（例如 DOCX 文档中的图像）中识别文本的值。默认值为 false。


**Returns:**
boolean - 指示是否在嵌入的图像中识别文本的值。

### setEnabledForEmbeddedImages(boolean value) {#setEnabledForEmbeddedImages-boolean-}
```
public abstract void setEnabledForEmbeddedImages(boolean value)
```


设置指示是否在嵌入的图像（例如 DOCX 文档中的图像）中识别文本的值。默认值为 false。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | boolean | 指示是否在嵌入的图像中识别文本的值。 |
|

### getOcrConnector() {#getOcrConnector--}
```
public abstract IOcrConnector getOcrConnector()
```


获取用于 OCR 处理的 OCR 连接器。默认值为 null，表示未使用 OCR。


**Returns:**
[IOcrConnector](../../com.groupdocs.search.options/iocrconnector) - An OCR connector that is used for OCR processing.

### setOcrConnector(IOcrConnector value) {#setOcrConnector-com.groupdocs.search.options.IOcrConnector-}
```
public abstract void setOcrConnector(IOcrConnector value)
```


设置用于 OCR 处理的 OCR 连接器。默认值为 null，表示未使用 OCR。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | value | [IOcrConnector](../../com.groupdocs.search.options/iocrconnector) | 用于 OCR 处理的 OCR 连接器。 |
|

