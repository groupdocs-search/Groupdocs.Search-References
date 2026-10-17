---
title: "VersionUpdateResult"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "表示索引版本更新操作的结果。"
type: docs
weight: 42
url: /zh/java/com.groupdocs.search.common/versionupdateresult/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum VersionUpdateResult extends Enum<VersionUpdateResult>
```

表示索引版本更新操作的结果。

## Fields

| Field | 描述 |
| --- | --- |
|  | [Updated](#Updated) | 索引版本已更新。 |
|
|  | [AlreadyUpToDate](#AlreadyUpToDate) | 索引版本已是最新的。 |
|
|  | [Unsupported](#Unsupported) | 索引版本不受支持，或目录不包含有效的索引数据。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Updated {#Updated}
```
public static final VersionUpdateResult Updated
```


索引版本已更新。


### AlreadyUpToDate {#AlreadyUpToDate}
```
public static final VersionUpdateResult AlreadyUpToDate
```


索引版本已是最新的。


### Unsupported {#Unsupported}
```
public static final VersionUpdateResult Unsupported
```


索引版本不受支持，或目录不包含有效的索引数据。


### values() {#values--}
```
public static VersionUpdateResult[] values()
```




**Returns:**
com.groupdocs.search.common.VersionUpdateResult[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static VersionUpdateResult valueOf(String name)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String |  |

**Returns:**
[VersionUpdateResult](../../com.groupdocs.search.common/versionupdateresult)
