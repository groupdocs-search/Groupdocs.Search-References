---
title: "TableDiscreteFunction"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "表示模糊搜索算法，其中包含词长与允许错误数之间的对应关系。"
type: docs
weight: 40
url: /zh/java/com.groupdocs.search.options/tablediscretefunction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.options.FuzzyAlgorithm](../../com.groupdocs.search.options/fuzzyalgorithm)
```
public class TableDiscreteFunction extends FuzzyAlgorithm
```

表示模糊搜索算法，该算法包含单词长度与允许错误数量之间的对应关系。此算法可以通过输出值表或步进函数来指定。


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
options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(1, new Step(5, 2), new Step(8, 3))); // 创建模糊搜索算法
// 此函数将 1 指定为长度为 1 到 4 个字符的单词的最大错误数。
// 将 2 指定为长度为 5 到 7 个字符的单词的最大错误数。
// 将 3 指定为长度为 8 个及以上字符的单词的最大错误数。
SearchResult result = index.search(query, options); // 在索引中搜索
 
```
 
````


## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [TableDiscreteFunction(int offsetOfInputs, int[] tableOfOutputs)](#TableDiscreteFunction-int-int---) | 初始化 TableDiscreteFunction 类的新实例。 |
|
|  | [TableDiscreteFunction(int firstStepLevel, Step[] steps)](#TableDiscreteFunction-int-com.groupdocs.search.options.Step...-) | 初始化 TableDiscreteFunction 类的新实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getSimilarityLevel(int termLength)](#getSimilarityLevel-int-) | 获取指定词长的相似度级别。 |
|
|  | [getMaxMistakeCount(int termLength)](#getMaxMistakeCount-int-) | 获取指定词长的最大允许错误数。 |
|
### TableDiscreteFunction(int offsetOfInputs, int[] tableOfOutputs) {#TableDiscreteFunction-int-int---}
```
public TableDiscreteFunction(int offsetOfInputs, int[] tableOfOutputs)
```


初始化 TableDiscreteFunction 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | offsetOfInputs | int | 表索引相对于输入值的偏移量。 |
|
|  | tableOfOutputs | int[] | 输出值表。 |
|

### TableDiscreteFunction(int firstStepLevel, Step[] steps) {#TableDiscreteFunction-int-com.groupdocs.search.options.Step...-}
```
public TableDiscreteFunction(int firstStepLevel, Step[] steps)
```


初始化 TableDiscreteFunction 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | firstStepLevel | int | 阶梯函数第一步的级别。 |
|
|  | steps | [Step\[\]](../../com.groupdocs.search.options/step) | 阶梯函数的后续步骤。 |
|

### getSimilarityLevel(int termLength) {#getSimilarityLevel-int-}
```
public double getSimilarityLevel(int termLength)
```


获取指定词长的相似度级别。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | termLength | int | 词长。 |
|

**Returns:**
double - 相似度级别。

### getMaxMistakeCount(int termLength) {#getMaxMistakeCount-int-}
```
public int getMaxMistakeCount(int termLength)
```


获取指定词长的最大允许错误数。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | termLength | int | 词长。 |
|

**Returns:**
int - 最大允许错误数。

