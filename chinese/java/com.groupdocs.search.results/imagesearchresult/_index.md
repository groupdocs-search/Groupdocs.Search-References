---
title: "ImageSearchResult"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "表示反向图像搜索的结果。"
type: docs
weight: 17
url: /zh/java/com.groupdocs.search.results/imagesearchresult/
---
**Inheritance:**
java.lang.Object
```
public abstract class ImageSearchResult
```

表示反向图像搜索的结果。

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [ImageSearchResult()](#ImageSearchResult--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getImageCount()](#getImageCount--) | 获取找到的图像数量。 |
|
|  | [getFoundImage(int index)](#getFoundImage-int-) | 按索引获取找到的图像。 |
|
### ImageSearchResult() {#ImageSearchResult--}
```
public ImageSearchResult()
```


### getImageCount() {#getImageCount--}
```
public abstract int getImageCount()
```


获取找到的图像数量。


**Returns:**
int - 找到的图像数量。

### getFoundImage(int index) {#getFoundImage-int-}
```
public abstract FoundImageFrame getFoundImage(int index)
```


按索引获取找到的图像。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 索引 | int | 找到的图像索引。 |
|

**Returns:**
[FoundImageFrame](../../com.groupdocs.search.results/foundimageframe) - The found image.

