---
title: "SearchQuery"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "表示对象形式的搜索查询。"
type: docs
weight: 25
url: /zh/java/com.groupdocs.search/searchquery/
---
**Inheritance:**
java.lang.Object
```
public abstract class SearchQuery
```

表示对象形式的搜索查询。


**Learn more**

* [Searching](../https://docs.groupdocs.com/display/searchjava/Searching)
* [Queries in text and object form](../https://docs.groupdocs.com/display/searchjava/Queries+in+text+and+object+form)
* [Nesting search queries in object form](../https://docs.groupdocs.com/display/searchjava/Nesting+search+queries+in+object+form)


此示例演示了该类的典型用法。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
 
Index index = new Index(indexFolder); // 在指定文件夹中创建索引
index.add(documentsFolder); // 从指定文件夹索引文档
 
// 创建日期范围搜索的子查询
SearchQuery subquery1 = SearchQuery.createDateRangeQuery(new Date(2011, 6, 17), new Date(2013, 1, 1));
 
// 创建通配符子查询，漏词数量从 0 到 2
SearchQuery subquery2 = SearchQuery.createWildcardQuery(0, 2);
 
// 创建简单词的子查询
SearchQuery subquery3 = SearchQuery.createWordQuery("birth");
subquery3.setSearchOptions(new SearchOptions()); // 仅为子查询 3 设置搜索选项
subquery3.getSearchOptions().getFuzzySearch().setEnabled(true);
subquery3.getSearchOptions().getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(1));
 
// 将子查询组合成一个查询
SearchQuery query = SearchQuery.createPhraseSearchQuery(subquery1, subquery2, subquery3);
 
// 创建搜索选项对象，增加已发现出现次数的容量
SearchOptions options = new SearchOptions(); // 整体搜索选项
options.setMaxOccurrenceCountPerTerm(1000000);
options.setMaxTotalOccurrenceCount(10000000);
 
SearchResult result = index.search(query, options); // 正在搜索
 
```
 
````


## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getFieldName()](#getFieldName--) | 获取字段名称。 |
|
|  | [getChildCount()](#getChildCount--) | 获取子查询的数量。 |
|
|  | [getFirstChild()](#getFirstChild--) | 获取第一个子查询。 |
|
|  | [getSecondChild()](#getSecondChild--) | 获取第二个子查询。 |
|
|  | [getChild(int index)](#getChild-int-) | 通过索引获取子查询。 |
|
|  | [getSearchOptions()](#getSearchOptions--) | 获取或设置此搜索查询的搜索选项。 |
|
|  | [setSearchOptions(SearchOptions value)](#setSearchOptions-com.groupdocs.search.options.SearchOptions-) | 获取或设置此搜索查询的搜索选项。 |
|
|  | [toString()](#toString--) | 返回一个  System.String ，它表示当前的  SearchQuery  实例。 |
|
|  | [createWordQuery(String term)](#createWordQuery-java.lang.String-) | 创建一个简单词查询。 |
|
|  | [createWordPatternQuery(WordPattern pattern)](#createWordPatternQuery-com.groupdocs.search.common.WordPattern-) | 创建一个词模式查询。 |
|
|  | [createRegexQuery(String pattern)](#createRegexQuery-java.lang.String-) | 创建正则表达式查询。 |
|
|  | [createRegexQuery(String pattern, int options)](#createRegexQuery-java.lang.String-int-) | 创建正则表达式查询。 |
|
|  | [createNumericRangeQuery(long start, long end)](#createNumericRangeQuery-long-long-) | 创建数值范围查询。 |
|
|  | [createDateRangeQuery(Date start, Date end)](#createDateRangeQuery-java.util.Date-java.util.Date-) | 创建日期范围查询。 |
|
|  | [createPhraseSearchQuery(SearchQuery[] queries)](#createPhraseSearchQuery-com.groupdocs.search.SearchQuery...-) | 创建短语搜索查询。 |
|
|  | [createAndQuery(SearchQuery[] queries)](#createAndQuery-com.groupdocs.search.SearchQuery---) | 创建组合查询，仅查找每个原始查询都能匹配的文档。 |
|
|  | [createFieldQuery(String fieldName, SearchQuery query)](#createFieldQuery-java.lang.String-com.groupdocs.search.SearchQuery-) | 向指定查询添加字段。 |
|
|  | [createNotQuery(SearchQuery query)](#createNotQuery-com.groupdocs.search.SearchQuery-) | 创建反向查询，以在索引中查找未被原始查询匹配的其余文档。 |
|
|  | [createAndQuery(SearchQuery leftQuery, SearchQuery rightQuery)](#createAndQuery-com.groupdocs.search.SearchQuery-com.groupdocs.search.SearchQuery-) | 创建组合查询，仅查找每个原始查询都能匹配的文档。 |
|
|  | [createOrQuery(SearchQuery leftQuery, SearchQuery rightQuery)](#createOrQuery-com.groupdocs.search.SearchQuery-com.groupdocs.search.SearchQuery-) | 创建组合查询，查找至少被原始查询之一匹配的所有文档。 |
|
|  | [createOrQuery(SearchQuery[] queries)](#createOrQuery-com.groupdocs.search.SearchQuery---) | 创建组合查询，查找至少被原始查询之一匹配的所有文档。 |
|
|  | [createWildcardQuery(int count)](#createWildcardQuery-int-) | 为短语搜索创建通配符。 |
|
|  | [createWildcardQuery(int minCount, int maxCount)](#createWildcardQuery-int-int-) | 为短语搜索创建通配符。 |
|
### getFieldName() {#getFieldName--}
```
public String getFieldName()
```


获取字段名称。


**Returns:**
java.lang.String - 字段名称。

### getChildCount() {#getChildCount--}
```
public int getChildCount()
```


获取子查询的数量。


**Returns:**
int - 子查询的数量。

### getFirstChild() {#getFirstChild--}
```
public SearchQuery getFirstChild()
```


获取第一个子查询。


**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - The first child query.

### getSecondChild() {#getSecondChild--}
```
public SearchQuery getSecondChild()
```


获取第二个子查询。


**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - The second child query.

### getChild(int index) {#getChild-int-}
```
public abstract SearchQuery getChild(int index)
```


通过索引获取子查询。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 索引 | int | 索引。 |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A child query corresponding the specified index.

### getSearchOptions() {#getSearchOptions--}
```
public final SearchOptions getSearchOptions()
```


获取或设置此搜索查询的搜索选项。


**Returns:**
[SearchOptions](../../com.groupdocs.search.options/searchoptions) - The search options.

### setSearchOptions(SearchOptions value) {#setSearchOptions-com.groupdocs.search.options.SearchOptions-}
```
public final void setSearchOptions(SearchOptions value)
```


获取或设置此搜索查询的搜索选项。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | value | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | 搜索选项。 |
|

### toString() {#toString--}
```
public abstract String toString()
```


返回一个  System.String ，它表示当前的  SearchQuery  实例。


**Returns:**
java.lang.String - 表示当前  SearchQuery  实例的  System.String。

### createWordQuery(String term) {#createWordQuery-java.lang.String-}
```
public static SearchQuery createWordQuery(String term)
```


创建一个简单词查询。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 词项 | java.lang.String | 要搜索的词项。 |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A simple word query.

### createWordPatternQuery(WordPattern pattern) {#createWordPatternQuery-com.groupdocs.search.common.WordPattern-}
```
public static SearchQuery createWordPatternQuery(WordPattern pattern)
```


创建一个词模式查询。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | pattern | [WordPattern](../../com.groupdocs.search.common/wordpattern) | 单词模式。 |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A word pattern query.

### createRegexQuery(String pattern) {#createRegexQuery-java.lang.String-}
```
public static SearchQuery createRegexQuery(String pattern)
```


创建正则表达式查询。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | pattern | java.lang.String | 要匹配的正则表达式模式。 |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A regular expression query.

### createRegexQuery(String pattern, int options) {#createRegexQuery-java.lang.String-int-}
```
public static SearchQuery createRegexQuery(String pattern, int options)
```


创建正则表达式查询。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | pattern | java.lang.String | 要匹配的正则表达式模式。 |
|
|  | options | int | 对正则表达式进行修改的枚举值的按位组合。此值必须包含  RegexOptions.IgnoreCase  标志。 |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A regular expression query.

### createNumericRangeQuery(long start, long end) {#createNumericRangeQuery-long-long-}
```
public static SearchQuery createNumericRangeQuery(long start, long end)
```


创建数值范围查询。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 起始 | long | 范围的起始值。 |
|
|  | 结束 | long | 范围的结束值。 |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A numeric range query.

### createDateRangeQuery(Date start, Date end) {#createDateRangeQuery-java.util.Date-java.util.Date-}
```
public static SearchQuery createDateRangeQuery(Date start, Date end)
```


创建日期范围查询。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 起始 | java.util.Date | 范围的起始值。 |
|
|  | 结束 | java.util.Date | 范围的结束值。 |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A date range query.

### createPhraseSearchQuery(SearchQuery[] queries) {#createPhraseSearchQuery-com.groupdocs.search.SearchQuery...-}
```
public static SearchQuery createPhraseSearchQuery(SearchQuery[] queries)
```


创建短语搜索查询。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | queries | [SearchQuery\[\]](../../com.groupdocs.search/searchquery) | 子查询。 |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A phrase search query.

### createAndQuery(SearchQuery[] queries) {#createAndQuery-com.groupdocs.search.SearchQuery---}
```
public static SearchQuery createAndQuery(SearchQuery[] queries)
```


创建组合查询，仅查找每个原始查询都能匹配的文档。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | queries | [SearchQuery\[\]](../../com.groupdocs.search/searchquery) | 要搜索的字段名称。 |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A combined AND query.

### createFieldQuery(String fieldName, SearchQuery query) {#createFieldQuery-java.lang.String-com.groupdocs.search.SearchQuery-}
```
public static SearchQuery createFieldQuery(String fieldName, SearchQuery query)
```


向指定查询添加字段。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | fieldName | java.lang.String | 要搜索的字段名称。 |
|
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | 用于添加字段的查询。 |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A query with the field to search in.

### createNotQuery(SearchQuery query) {#createNotQuery-com.groupdocs.search.SearchQuery-}
```
public static SearchQuery createNotQuery(SearchQuery query)
```


创建反向查询，以在索引中查找未被原始查询匹配的其余文档。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | 用于取反的查询。 |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A combined NOT query.

### createAndQuery(SearchQuery leftQuery, SearchQuery rightQuery) {#createAndQuery-com.groupdocs.search.SearchQuery-com.groupdocs.search.SearchQuery-}
```
public static SearchQuery createAndQuery(SearchQuery leftQuery, SearchQuery rightQuery)
```


创建组合查询，仅查找每个原始查询都能匹配的文档。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | leftQuery | [SearchQuery](../../com.groupdocs.search/searchquery) | 左子查询。 |
|
|  | rightQuery | [SearchQuery](../../com.groupdocs.search/searchquery) | 右子查询。 |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A combined AND query.

### createOrQuery(SearchQuery leftQuery, SearchQuery rightQuery) {#createOrQuery-com.groupdocs.search.SearchQuery-com.groupdocs.search.SearchQuery-}
```
public static SearchQuery createOrQuery(SearchQuery leftQuery, SearchQuery rightQuery)
```


创建组合查询，查找至少被原始查询之一匹配的所有文档。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | leftQuery | [SearchQuery](../../com.groupdocs.search/searchquery) | 左子查询。 |
|
|  | rightQuery | [SearchQuery](../../com.groupdocs.search/searchquery) | 右子查询。 |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A combined OR query.

### createOrQuery(SearchQuery[] queries) {#createOrQuery-com.groupdocs.search.SearchQuery---}
```
public static SearchQuery createOrQuery(SearchQuery[] queries)
```


创建组合查询，查找至少被原始查询之一匹配的所有文档。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | queries | [SearchQuery\[\]](../../com.groupdocs.search/searchquery) | 子查询。 |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A combined OR query.

### createWildcardQuery(int count) {#createWildcardQuery-int-}
```
public static SearchQuery createWildcardQuery(int count)
```


为短语搜索创建通配符。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | count | int | 通配符中的单词数量。 |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A wildcard for the phrase search.

### createWildcardQuery(int minCount, int maxCount) {#createWildcardQuery-int-int-}
```
public static SearchQuery createWildcardQuery(int minCount, int maxCount)
```


为短语搜索创建通配符。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | minCount | int | 通配符中单词的最小数量。 |
|
|  | maxCount | int | 通配符中单词的最大数量。 |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A wildcard for the phrase search.

