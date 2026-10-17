---
title: "FoundImageFrame"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "表示已找到的图像帧。"
type: docs
weight: 16
url: /zh/java/com.groupdocs.search.results/foundimageframe/
---
**Inheritance:**
java.lang.Object
```
public abstract class FoundImageFrame
```

表示已找到的图像帧。

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [FoundImageFrame()](#FoundImageFrame--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getDocumentInfo()](#getDocumentInfo--) | 获取文档信息。 |
|
|  | [getImageIndex()](#getImageIndex--) | 获取文档中图像的序号。 |
|
|  | [getFrameIndex()](#getFrameIndex--) | 获取图像中帧的索引。 |
|
|  | [getHashDifferences()](#getHashDifferences--) | 获取图像哈希中不匹配位的数量。 |
|
|  | [toString()](#toString--) | 返回一个  System.String  表示当前的  FoundImageFrame 。 |
|
### FoundImageFrame() {#FoundImageFrame--}
```
public FoundImageFrame()
```


### getDocumentInfo() {#getDocumentInfo--}
```
public abstract DocumentInfo getDocumentInfo()
```


获取文档信息。


**Returns:**
[DocumentInfo](../../com.groupdocs.search.results/documentinfo) - The document info.

### getImageIndex() {#getImageIndex--}
```
public abstract int getImageIndex()
```


获取文档中图像的序号。


**Returns:**
int - 文档中图像的序号。

### getFrameIndex() {#getFrameIndex--}
```
public abstract int getFrameIndex()
```


获取图像中帧的索引。


**Returns:**
int - 图像中帧的索引。

### getHashDifferences() {#getHashDifferences--}
```
public abstract int getHashDifferences()
```


获取图像哈希中不匹配位的数量。


**Returns:**
int - 图像哈希中不匹配位的数量。

### toString() {#toString--}
```
public abstract String toString()
```


返回一个  System.String  表示当前的  FoundImageFrame 。


**Returns:**
java.lang.String - 一个  System.String  表示当前的  FoundImageFrame 。

