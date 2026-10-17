---
title: "IndexInfo"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "包含有关索引的基本信息。"
type: docs
weight: 24
url: /zh/java/com.groupdocs.search.common/indexinfo/
---
**Inheritance:**
java.lang.Object
```
public abstract class IndexInfo
```

包含索引的基本信息。

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [IndexInfo()](#IndexInfo--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getIndexId()](#getIndexId--) | 获取索引唯一标识符。 |
|
|  | [getIndexFolder()](#getIndexFolder--) | 获取索引所在的完整文件夹名称。 |
|
|  | [getIndexStatus()](#getIndexStatus--) | 获取索引状态。 |
|
|  | [getVersion()](#getVersion--) | 获取索引版本。 |
|
|  | [getSegmentCount()](#getSegmentCount--) | 获取索引段的数量。 |
|
|  | [getTermCount()](#getTermCount--) | 获取索引中的单词数量。 |
|
### IndexInfo() {#IndexInfo--}
```
public IndexInfo()
```


### getIndexId() {#getIndexId--}
```
public abstract UUID getIndexId()
```


获取索引唯一标识符。


**Returns:**
java.util.UUID - 索引唯一标识符。

### getIndexFolder() {#getIndexFolder--}
```
public abstract String getIndexFolder()
```


获取索引所在的完整文件夹名称。


**Returns:**
java.lang.String - 索引所在的完整文件夹名称。

### getIndexStatus() {#getIndexStatus--}
```
public abstract IndexStatus getIndexStatus()
```


获取索引状态。


**Returns:**
[IndexStatus](../../com.groupdocs.search.common/indexstatus) - The index status.

### getVersion() {#getVersion--}
```
public abstract String getVersion()
```


获取索引版本。


**Returns:**
java.lang.String - 索引版本。

### getSegmentCount() {#getSegmentCount--}
```
public abstract int getSegmentCount()
```


获取索引段的数量。


**Returns:**
int - 索引段的数量。

### getTermCount() {#getTermCount--}
```
public abstract int getTermCount()
```


获取索引中的单词数量。


**Returns:**
int - 索引中的单词数量。

