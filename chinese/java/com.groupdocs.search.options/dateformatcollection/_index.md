---
title: "DateFormatCollection"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "表示 DateFormat 对象的集合。"
type: docs
weight: 14
url: /zh/java/com.groupdocs.search.options/dateformatcollection/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public abstract class DateFormatCollection implements Iterable<DateFormat>
```

表示 DateFormat 对象的集合。


**Learn more**

* [Date range search](../https://docs.groupdocs.com/display/searchjava/Date+range+search)

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [DateFormatCollection()](#DateFormatCollection--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [addItem(DateFormat item)](#addItem-com.groupdocs.search.options.DateFormat-) | 向集合中添加一个日期格式对象。 |
|
|  | [clear()](#clear--) | 从集合中移除所有元素。 |
|
|  | [containsItem(DateFormat item)](#containsItem-com.groupdocs.search.options.DateFormat-) | 确定集合是否包含特定项。 |
|
|  | [copyToTArray(DateFormat[] array, int arrayIndex)](#copyToTArray-com.groupdocs.search.options.DateFormat---int-) | 将集合的元素复制到一个 Array 中，从特定的 Array 索引开始。 |
|
|  | [size()](#size--) | 获取集合中包含的元素数量。 |
|
|  | [isReadOnly()](#isReadOnly--) | 获取一个值，指示集合是否为只读。 |
|
|  | [removeItem(DateFormat item)](#removeItem-com.groupdocs.search.options.DateFormat-) | 从集合中移除特定元素的第一次出现。 |
|
|  | [iterator()](#iterator--) | 返回一个遍历集合的枚举器。 |
|
### DateFormatCollection() {#DateFormatCollection--}
```
public DateFormatCollection()
```


### addItem(DateFormat item) {#addItem-com.groupdocs.search.options.DateFormat-}
```
public abstract void addItem(DateFormat item)
```


向集合中添加一个日期格式对象。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | item | [DateFormat](../../com.groupdocs.search.options/dateformat) | 要添加到集合中的日期格式对象。 |
|

### clear() {#clear--}
```
public abstract void clear()
```


从集合中移除所有元素。


### containsItem(DateFormat item) {#containsItem-com.groupdocs.search.options.DateFormat-}
```
public abstract boolean containsItem(DateFormat item)
```


确定集合是否包含特定项。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | item | [DateFormat](../../com.groupdocs.search.options/dateformat) | 在集合中定位的项。 |
|

**Returns:**
boolean - 如果在集合中找到项则为 true；否则为 false。

### copyToTArray(DateFormat[] array, int arrayIndex) {#copyToTArray-com.groupdocs.search.options.DateFormat---int-}
```
public abstract void copyToTArray(DateFormat[] array, int arrayIndex)
```


将集合的元素复制到一个 Array 中，从特定的 Array 索引开始。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | array | [DateFormat\[\]](../../com.groupdocs.search.options/dateformat) | 从集合中复制的元素的目标是一维 Array。 |
|
|  | arrayIndex | int | 复制开始时数组中的零基索引。 |
|

### size() {#size--}
```
public abstract int size()
```


获取集合中包含的元素数量。


**Returns:**
int - 集合中包含的元素数量。

### isReadOnly() {#isReadOnly--}
```
public abstract boolean isReadOnly()
```


获取一个值，指示集合是否为只读。


**Returns:**
boolean - 如果集合是只读的则为 true；否则为 false。

### removeItem(DateFormat item) {#removeItem-com.groupdocs.search.options.DateFormat-}
```
public abstract boolean removeItem(DateFormat item)
```


从集合中移除特定元素的第一次出现。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | item | [DateFormat](../../com.groupdocs.search.options/dateformat) | 要从集合中移除的项。 |
|

**Returns:**
boolean - 如果成功从集合中移除项则为 true；否则为 false。若在集合中未找到该项，此方法也返回 false。

### iterator() {#iterator--}
```
public abstract Iterator<DateFormat> iterator()
```


返回一个遍历集合的枚举器。


**Returns:**
java.util.Iterator<com.groupdocs.search.options.DateFormat> - 可用于遍历集合的枚举器。

