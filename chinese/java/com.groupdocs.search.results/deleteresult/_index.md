---
title: "DeleteResult"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "表示从索引中删除已索引文件或文件夹操作的结果。"
type: docs
weight: 10
url: /zh/java/com.groupdocs.search.results/deleteresult/
---
**Inheritance:**
java.lang.Object
```
public class DeleteResult
```

表示从索引中删除已索引文件或文件夹操作的结果。


**Learn more**

* [Delete indexed paths](../https://docs.groupdocs.com/display/searchjava/Delete+indexed+paths)

## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getItemResults()](#getItemResults--) | 返回每个路径删除的结果。 |
|
|  | [getTotalCount()](#getTotalCount--) | 返回要删除的路径总数。 |
|
|  | [getSuccessCount()](#getSuccessCount--) | 返回成功删除的路径数量。 |
|
|  | [getFailedCount()](#getFailedCount--) | 返回因错误未删除的路径数量。 |
|
|  | [getErrors()](#getErrors--) | 返回删除错误的描述。 |
|
### getItemResults() {#getItemResults--}
```
public final PathDeleteResult[] getItemResults()
```


返回每个路径删除的结果。


**Returns:**
com.groupdocs.search.results.PathDeleteResult[] - 每个路径删除的结果。

### getTotalCount() {#getTotalCount--}
```
public final int getTotalCount()
```


返回要删除的路径总数。


**Returns:**
int - 要删除的路径总数。

### getSuccessCount() {#getSuccessCount--}
```
public final int getSuccessCount()
```


返回成功删除的路径数量。


**Returns:**
int - 成功删除的路径数量。

### getFailedCount() {#getFailedCount--}
```
public final int getFailedCount()
```


返回因错误未删除的路径数量。


**Returns:**
int - 因错误未删除的路径数量。

### getErrors() {#getErrors--}
```
public final String[] getErrors()
```


返回删除错误的描述。


**Returns:**
java.lang.String[] - 删除错误的描述。

