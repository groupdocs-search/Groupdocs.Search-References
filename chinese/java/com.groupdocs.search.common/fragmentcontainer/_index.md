---
title: "FragmentContainer"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "表示包含单个文档字段中已高亮找到的词汇的文本片段的容器。"
type: docs
weight: 22
url: /zh/java/com.groupdocs.search.common/fragmentcontainer/
---
**Inheritance:**
java.lang.Object
```
public abstract class FragmentContainer
```

表示包含单个文档字段中已高亮找到的词汇的文本片段的容器。


**Learn more**

* [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [FragmentContainer()](#FragmentContainer--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getFieldName()](#getFieldName--) | 获取文档字段名称。 |
|
|  | [getCount()](#getCount--) | 获取包含的文本片段数量。 |
|
|  | [getFragments()](#getFragments--) | 获取包含的文本片段数组。 |
|
### FragmentContainer() {#FragmentContainer--}
```
public FragmentContainer()
```


### getFieldName() {#getFieldName--}
```
public abstract String getFieldName()
```


获取文档字段名称。


**Returns:**
java.lang.String - 文档字段名称。

### getCount() {#getCount--}
```
public abstract int getCount()
```


获取包含的文本片段数量。


**Returns:**
int - 包含的文本片段数量。

### getFragments() {#getFragments--}
```
public abstract String[] getFragments()
```


获取包含的文本片段数组。


**Returns:**
java.lang.String[] - 包含的文本片段数组。

