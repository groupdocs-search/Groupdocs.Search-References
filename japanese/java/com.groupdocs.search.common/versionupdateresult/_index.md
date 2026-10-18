---
title: "VersionUpdateResult"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "インデックスバージョン更新操作の結果を表します。"
type: docs
weight: 42
url: /ja/java/com.groupdocs.search.common/versionupdateresult/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum VersionUpdateResult extends Enum<VersionUpdateResult>
```

インデックスバージョン更新操作の結果を表します。

## Fields

| Field | 説明 |
| --- | --- |
|  | [Updated](#Updated) | インデックス バージョンが更新されました。 |
|
|  | [AlreadyUpToDate](#AlreadyUpToDate) | インデックス バージョンはすでに最新です。 |
|
|  | [Unsupported](#Unsupported) | インデックス バージョンはサポートされていないか、ディレクトリに有効なインデックス データが含まれていません。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Updated {#Updated}
```
public static final VersionUpdateResult Updated
```


インデックス バージョンが更新されました。


### AlreadyUpToDate {#AlreadyUpToDate}
```
public static final VersionUpdateResult AlreadyUpToDate
```


インデックス バージョンはすでに最新です。


### Unsupported {#Unsupported}
```
public static final VersionUpdateResult Unsupported
```


インデックス バージョンはサポートされていないか、ディレクトリに有効なインデックス データが含まれていません。


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
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[VersionUpdateResult](../../com.groupdocs.search.common/versionupdateresult)
