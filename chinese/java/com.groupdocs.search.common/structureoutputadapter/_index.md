---
title: "StructureOutputAdapter"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "表示将输出收集为包含每个字段的结构体的输出适配器。"
type: docs
weight: 33
url: /zh/java/com.groupdocs.search.common/structureoutputadapter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.common.OutputAdapter](../../com.groupdocs.search.common/outputadapter)

**All Implemented Interfaces:**
[com.groupdocs.search.common.IStructureOutputAdapter](../../com.groupdocs.search.common/istructureoutputadapter)
```
public class StructureOutputAdapter extends OutputAdapter implements IStructureOutputAdapter
```

表示将输出收集为包含每个字段的结构体的输出适配器。

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [StructureOutputAdapter(OutputFormat outputFormat)](#StructureOutputAdapter-com.groupdocs.search.options.OutputFormat-) | 初始化 StructureOutputAdapter 类的新实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getResult()](#getResult--) | 获取结果字段数组。 |
|
### StructureOutputAdapter(OutputFormat outputFormat) {#StructureOutputAdapter-com.groupdocs.search.options.OutputFormat-}
```
public StructureOutputAdapter(OutputFormat outputFormat)
```


初始化 StructureOutputAdapter 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | outputFormat | [OutputFormat](../../com.groupdocs.search.options/outputformat) | 输出格式。 |
|

### getResult() {#getResult--}
```
public final DocumentField[] getResult()
```


获取结果字段数组。


**Returns:**
com.groupdocs.search.common.DocumentField[] - 结果字段数组。

