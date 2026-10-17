---
title: "FuzzySearchOptions"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "提供模糊搜索的选项。"
type: docs
weight: 21
url: /zh/java/com.groupdocs.search.options/fuzzysearchoptions/
---
**Inheritance:**
java.lang.Object
```
public abstract class FuzzySearchOptions
```

提供模糊搜索的选项。


**Learn more**

* [Fuzzy search](../https://docs.groupdocs.com/display/searchjava/Fuzzy+search)
* [Search options](../https://docs.groupdocs.com/display/searchjava/Search+options)

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [FuzzySearchOptions()](#FuzzySearchOptions--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getEnabled()](#getEnabled--) | 获取一个值，指示是否已启用模糊搜索功能。 |
|
|  | [setEnabled(boolean value)](#setEnabled-boolean-) | 设置一个指示是否启用模糊搜索功能的值。 |
|
|  | [getFuzzyAlgorithm()](#getFuzzyAlgorithm--) | 获取模糊搜索算法。 |
|
|  | [setFuzzyAlgorithm(FuzzyAlgorithm value)](#setFuzzyAlgorithm-com.groupdocs.search.options.FuzzyAlgorithm-) | 设置模糊搜索算法。 |
|
|  | [getOnlyBestResults()](#getOnlyBestResults--) | 获取指示是否仅返回最佳结果的值。 |
|
|  | [setOnlyBestResults(boolean value)](#setOnlyBestResults-boolean-) | 设置指示是否仅返回最佳结果的值。 |
|
|  | [getOnlyBestResultsRange()](#getOnlyBestResultsRange--) | 获取发现的最小错误数的最大超出值。 |
|
|  | [setOnlyBestResultsRange(byte value)](#setOnlyBestResultsRange-byte-) | 设置发现的最小错误数的最大超出值。 |
|
|  | [getConsiderTranspositions()](#getConsiderTranspositions--) | 获取一个指示模糊搜索算法是否必须将相邻两个字符的换位视为单个错误的值。 |
|
|  | [setConsiderTranspositions(boolean value)](#setConsiderTranspositions-boolean-) | 设置一个指示模糊搜索算法是否必须将相邻两个字符的换位视为单个错误的值。 |
|
### FuzzySearchOptions() {#FuzzySearchOptions--}
```
public FuzzySearchOptions()
```


### getEnabled() {#getEnabled--}
```
public abstract boolean getEnabled()
```


获取一个指示是否启用模糊搜索功能的值。默认值为 false。


**Returns:**
boolean - 指示是否启用模糊搜索功能的值。

### setEnabled(boolean value) {#setEnabled-boolean-}
```
public abstract void setEnabled(boolean value)
```


设置一个指示是否启用模糊搜索功能的值。默认值为 false。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | boolean | 指示是否启用模糊搜索功能的值。 |
|

### getFuzzyAlgorithm() {#getFuzzyAlgorithm--}
```
public abstract FuzzyAlgorithm getFuzzyAlgorithm()
```


获取模糊搜索算法。目前可用的模糊搜索算法有 SimilarityLevel 和 TableDiscreteFunction。默认值是一个 SimilarityLevel 实例，其相似度水平值为 0.5。


**Returns:**
[FuzzyAlgorithm](../../com.groupdocs.search.options/fuzzyalgorithm) - The fuzzy search algorithm.


示例演示了如何设置模糊搜索算法。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // 在指定文件夹中创建索引
index.add(documentsFolder); // 从指定文件夹索引文档
SearchOptions options = new SearchOptions();
options.getFuzzySearch().setEnabled(true); // 启用模糊搜索
options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(1, new Step(5, 2), new Step(8, 3))); // 创建模糊搜索算法
// 此函数将 1 指定为长度为 1 到 4 个字符的单词的最大错误数。
// 将 2 指定为长度为 5 到 7 个字符的单词的最大错误数。
// 将 3 指定为长度为 8 个及以上字符的单词的最大错误数。
SearchResult result = index.search(query, options); // 在索引中搜索
 
```
 
````


### setFuzzyAlgorithm(FuzzyAlgorithm value) {#setFuzzyAlgorithm-com.groupdocs.search.options.FuzzyAlgorithm-}
```
public abstract void setFuzzyAlgorithm(FuzzyAlgorithm value)
```


设置模糊搜索算法。目前可用的模糊搜索算法有 SimilarityLevel 和 TableDiscreteFunction。默认值是一个 SimilarityLevel 实例，其相似度水平值为 0.5。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | value | [FuzzyAlgorithm](../../com.groupdocs.search.options/fuzzyalgorithm) | 模糊搜索算法。 |


示例演示了如何设置模糊搜索算法。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // 在指定文件夹中创建索引
index.add(documentsFolder); // 从指定文件夹索引文档
SearchOptions options = new SearchOptions();
options.getFuzzySearch().setEnabled(true); // 启用模糊搜索
options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(1, new Step(5, 2), new Step(8, 3))); // 创建模糊搜索算法
// 此函数将 1 指定为长度为 1 到 4 个字符的单词的最大错误数。
// 将 2 指定为长度为 5 到 7 个字符的单词的最大错误数。
// 将 3 指定为长度为 8 个及以上字符的单词的最大错误数。
SearchResult result = index.search(query, options); // 在索引中搜索
 
```
 
````

|

### getOnlyBestResults() {#getOnlyBestResults--}
```
public abstract boolean getOnlyBestResults()
```


获取一个值，指示是否仅返回最佳结果。默认值为 false。


**Returns:**
boolean - true 如果仅返回最佳结果；否则 false。

### setOnlyBestResults(boolean value) {#setOnlyBestResults-boolean-}
```
public abstract void setOnlyBestResults(boolean value)
```


设置一个值，指示是否仅返回最佳结果。默认值为 false。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | boolean | true 如果仅返回最佳结果；否则 false。 |
|

### getOnlyBestResultsRange() {#getOnlyBestResultsRange--}
```
public abstract byte getOnlyBestResultsRange()
```


获取找到的最小错误数的最大超出值。默认值为 0。


**Returns:**
byte - 找到的最小错误数的最大超出值。

### setOnlyBestResultsRange(byte value) {#setOnlyBestResultsRange-byte-}
```
public abstract void setOnlyBestResultsRange(byte value)
```


设置找到的最小错误数的最大超出值。默认值为 0。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | byte | 找到的最小错误数的最大超出值。 |
|

### getConsiderTranspositions() {#getConsiderTranspositions--}
```
public abstract boolean getConsiderTranspositions()
```


获取一个指示模糊搜索算法是否必须将相邻两个字符的换位视为单个错误的值。默认值为 true。


**Returns:**
boolean - 如果模糊搜索算法考虑换位则为 true；否则为 false。

### setConsiderTranspositions(boolean value) {#setConsiderTranspositions-boolean-}
```
public abstract void setConsiderTranspositions(boolean value)
```


设置一个指示模糊搜索算法是否必须将相邻两个字符的换位视为单个错误的值。默认值为 true。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | boolean | :  true  如果模糊搜索算法考虑换位；否则  false 。 |
|

