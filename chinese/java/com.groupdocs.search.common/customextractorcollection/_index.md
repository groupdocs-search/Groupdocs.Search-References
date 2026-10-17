---
title: "CustomExtractorCollection"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "包含自定义提取器的集合。"
type: docs
weight: 13
url: /zh/java/com.groupdocs.search.common/customextractorcollection/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public abstract class CustomExtractorCollection implements Iterable
```

包含自定义提取器的集合。如果集合中包含针对某些文件扩展名的提取器，而该扩展名已被内置提取器覆盖，则将使用此提取器而不是内置提取器。


**Learn more**

* [Custom text extractors](../https://docs.groupdocs.com/display/searchjava/Custom+text+extractors)

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [CustomExtractorCollection()](#CustomExtractorCollection--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [size()](#size--) | 获取集合中包含的提取器数量。 |
|
|  | [isReadOnly()](#isReadOnly--) | 获取一个值，指示集合是否为只读。 |
|
|  | [iterator()](#iterator--) | 返回此集合的迭代器。 |
|
|  | [addItem(IFieldExtractor extractor)](#addItem-com.groupdocs.search.common.IFieldExtractor-) | 向集合中添加提取器。 |
|
|  | [clear()](#clear--) | 从集合中移除所有提取器。 |
|
|  | [containsItem(IFieldExtractor item)](#containsItem-com.groupdocs.search.common.IFieldExtractor-) | 确定集合是否包含特定的提取器。 |
|
|  | [copyToTArray(IFieldExtractor[] array, int arrayIndex)](#copyToTArray-com.groupdocs.search.common.IFieldExtractor---int-) | 将集合的元素复制到数组中，从特定的数组索引开始。 |
|
|  | [removeItem(IFieldExtractor extractor)](#removeItem-com.groupdocs.search.common.IFieldExtractor-) | 从集合中移除提取器。 |
|
### CustomExtractorCollection() {#CustomExtractorCollection--}
```
public CustomExtractorCollection()
```


### size() {#size--}
```
public abstract int size()
```


获取集合中包含的提取器数量。


**Returns:**
int - 集合中包含的提取器数量。

### isReadOnly() {#isReadOnly--}
```
public abstract boolean isReadOnly()
```


获取一个值，指示集合是否为只读。


**Returns:**
boolean - 指示集合是否为只读的值。

### iterator() {#iterator--}
```
public abstract Iterator<IFieldExtractor> iterator()
```


返回此集合的迭代器。


**Returns:**
java.util.Iterator<com.groupdocs.search.common.IFieldExtractor> - 可用于遍历集合的迭代器对象。

### addItem(IFieldExtractor extractor) {#addItem-com.groupdocs.search.common.IFieldExtractor-}
```
public abstract void addItem(IFieldExtractor extractor)
```


向集合中添加提取器。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | extractor | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | 要添加到集合中的提取器。 |
|

### clear() {#clear--}
```
public abstract void clear()
```


从集合中移除所有提取器。


### containsItem(IFieldExtractor item) {#containsItem-com.groupdocs.search.common.IFieldExtractor-}
```
public abstract boolean containsItem(IFieldExtractor item)
```


确定集合是否包含特定的提取器。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | item | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | 要在集合中定位的提取器。 |
|

**Returns:**
boolean - 如果在集合中找到项则为 true；否则为 false。

### copyToTArray(IFieldExtractor[] array, int arrayIndex) {#copyToTArray-com.groupdocs.search.common.IFieldExtractor---int-}
```
public abstract void copyToTArray(IFieldExtractor[] array, int arrayIndex)
```


将集合的元素复制到数组中，从特定的数组索引开始。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | array | [IFieldExtractor\[\]](../../com.groupdocs.search.common/ifieldextractor) | 从集合复制的元素的目标一维数组。该数组必须使用从零开始的索引。 |
|
|  | arrayIndex | int | 复制开始时数组中的零基索引。 |
|

### removeItem(IFieldExtractor extractor) {#removeItem-com.groupdocs.search.common.IFieldExtractor-}
```
public abstract boolean removeItem(IFieldExtractor extractor)
```


从集合中移除提取器。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | extractor | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | 要从集合中移除的提取器。 |
|

**Returns:**
boolean - 如果成功从集合中移除提取器则为 true；否则为 false。若在原始集合中未找到提取器，此方法也返回 false。

