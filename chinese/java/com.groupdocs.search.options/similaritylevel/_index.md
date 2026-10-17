---
title: "SimilarityLevel"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "表示模糊搜索的算法，指定相似度水平。"
type: docs
weight: 35
url: /zh/java/com.groupdocs.search.options/similaritylevel/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.options.FuzzyAlgorithm](../../com.groupdocs.search.options/fuzzyalgorithm)
```
public class SimilarityLevel extends FuzzyAlgorithm
```

表示模糊搜索的算法，用于指定相似度级别。相似度级别算法根据单词长度的倒数比例计算单词的最大错误数。


**Learn more**

* [Fuzzy search](../https://docs.groupdocs.com/display/searchjava/Fuzzy+search)


此示例演示了该类的典型用法。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // 在指定文件夹中创建索引
index.add(documentsFolder); // 从指定文件夹索引文档
SearchOptions options = new SearchOptions();
options.getFuzzySearch().setEnabled(true); // 启用模糊搜索
options.getFuzzySearch().setFuzzyAlgorithm(new SimilarityLevel(0.8)); // 创建模糊搜索算法
// 此函数将 0 指定为 1 到 4 个字符的单词的最大错误数。
// 它将 1 指定为 5 到 9 个字符的单词的最大错误数。
// 它将 2 指定为 10 到 14 个字符的单词的最大错误数。依此类推。
SearchResult result = index.search(query, options); // 在索引中搜索
 
```
 
````


## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [SimilarityLevel(double value)](#SimilarityLevel-double-) | 初始化一个新的 SimilarityLevel 类实例。 |
|
|  | [SimilarityLevel(Object data)](#SimilarityLevel-java.lang.Object-) | 初始化一个新的 SimilarityLevel 类实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getSimilarityLevel(int termLength)](#getSimilarityLevel-int-) | 获取指定词长的相似度级别值。 |
|
|  | [getMaxMistakeCount(int termLength)](#getMaxMistakeCount-int-) | 获取指定词长允许的最大错误数。 |
|
### SimilarityLevel(double value) {#SimilarityLevel-double-}
```
public SimilarityLevel(double value)
```


初始化一个新的 SimilarityLevel 类实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | double | 相似度级别值。 |
|

### SimilarityLevel(Object data) {#SimilarityLevel-java.lang.Object-}
```
public SimilarityLevel(Object data)
```


初始化一个新的 SimilarityLevel 类实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 数据 | java.lang.Object | 序列化的数据。 |
|

### getSimilarityLevel(int termLength) {#getSimilarityLevel-int-}
```
public double getSimilarityLevel(int termLength)
```


获取指定词长的相似度级别值。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | termLength | int | 词长。 |
|

**Returns:**
double - 相似度级别值。

### getMaxMistakeCount(int termLength) {#getMaxMistakeCount-int-}
```
public int getMaxMistakeCount(int termLength)
```


获取指定词长允许的最大错误数。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | termLength | int | 词长。 |
|

**Returns:**
int - 允许的最大错误数。

