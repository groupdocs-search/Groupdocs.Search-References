---
title: "PathDeleteResult"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "表示从索引中删除已索引文件或文件夹操作的结果。"
type: docs
weight: 18
url: /zh/java/com.groupdocs.search.results/pathdeleteresult/
---
**Inheritance:**
java.lang.Object
```
public class PathDeleteResult
```

表示从索引中删除已索引文件或文件夹操作的结果。


**Learn more**

* [Delete indexed paths](../https://docs.groupdocs.com/display/searchjava/Delete+indexed+paths)

## 方法

| 方法 | 描述 |
| --- | --- |
|  | [isSuccess()](#isSuccess--) | 返回删除操作的成功指示器。 |
|
|  | [getError()](#getError--) | 返回删除错误的描述。 |
|
|  | [getPath()](#getPath--) | 返回要删除的文件或文件夹的路径。 |
|
### isSuccess() {#isSuccess--}
```
public final boolean isSuccess()
```


返回删除操作的成功指示器。


**Returns:**
boolean -  true  如果删除操作成功；否则，返回  false 。

### getError() {#getError--}
```
public final String getError()
```


返回删除错误的描述。


**Returns:**
java.lang.String - 删除错误的描述。

### getPath() {#getPath--}
```
public final String getPath()
```


返回要删除的文件或文件夹的路径。


**Returns:**
java.lang.String - 要删除的文件或文件夹的路径。

