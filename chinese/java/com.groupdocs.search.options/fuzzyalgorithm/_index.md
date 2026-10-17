---
title: "FuzzyAlgorithm"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "表示模糊搜索算法的基类。"
type: docs
weight: 20
url: /zh/java/com.groupdocs.search.options/fuzzyalgorithm/
---
**Inheritance:**
java.lang.Object
```
public abstract class FuzzyAlgorithm
```

表示模糊搜索算法的基类。


**Learn more**

* [Fuzzy search](../https://docs.groupdocs.com/display/searchjava/Fuzzy+search)

## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getSimilarityLevel(int termLength)](#getSimilarityLevel-int-) | 获取指定词长的相似度水平。 |
|
|  | [getMaxMistakeCount(int termLength)](#getMaxMistakeCount-int-) | 获取指定词长允许的最大错误数。 |
|
| [getCore()](#getCore--) |  |
### getSimilarityLevel(int termLength) {#getSimilarityLevel-int-}
```
public abstract double getSimilarityLevel(int termLength)
```


获取指定词长的相似度水平。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | termLength | int | 词长。 |
|

**Returns:**
double - 相似度水平。

### getMaxMistakeCount(int termLength) {#getMaxMistakeCount-int-}
```
public abstract int getMaxMistakeCount(int termLength)
```


获取指定词长允许的最大错误数。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | termLength | int | 词长。 |
|

**Returns:**
int - 允许的最大错误数。

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
