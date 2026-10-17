---
title: "DocumentStatus"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "表示文档处理状态。"
type: docs
weight: 40
url: /zh/java/com.groupdocs.search.common/documentstatus/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum DocumentStatus extends Enum<DocumentStatus>
```

表示文档处理状态。

## Fields

| Field | 描述 |
| --- | --- |
|  | [SuccessfullyProcessed](#SuccessfullyProcessed) | 文档已成功索引。 |
|
|  | [Skipped](#Skipped) | 文档已跳过。 |
|
|  | [ProcessedWithError](#ProcessedWithError) | 文档索引期间发生错误。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### SuccessfullyProcessed {#SuccessfullyProcessed}
```
public static final DocumentStatus SuccessfullyProcessed
```


文档已成功索引。


### Skipped {#Skipped}
```
public static final DocumentStatus Skipped
```


文档已跳过。


### ProcessedWithError {#ProcessedWithError}
```
public static final DocumentStatus ProcessedWithError
```


文档索引期间发生错误。


### values() {#values--}
```
public static DocumentStatus[] values()
```




**Returns:**
com.groupdocs.search.common.DocumentStatus[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static DocumentStatus valueOf(String name)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String |  |

**Returns:**
[DocumentStatus](../../com.groupdocs.search.common/documentstatus)
