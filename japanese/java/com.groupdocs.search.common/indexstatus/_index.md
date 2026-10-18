---
title: "IndexStatus"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "インデックスのステータスを指定します。"
type: docs
weight: 41
url: /ja/java/com.groupdocs.search.common/indexstatus/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum IndexStatus extends Enum<IndexStatus>
```

インデックスのステータスを指定します。

## Fields

| Field | 説明 |
| --- | --- |
|  | [Ready](#Ready) | インデックスは空きがあり、変更の準備ができています。 |
|
|  | [Failed](#Failed) | エラーのため、インデックスを再読み込みする必要があります。 |
|
|  | [Indexing](#Indexing) | インデックスはインデックス作成操作を実行します。 |
|
|  | [Updating](#Updating) | インデックスは更新操作を実行します。 |
|
|  | [Merging](#Merging) | インデックスはマージ操作を実行します。 |
|
|  | [Optimizing](#Optimizing) | インデックスは最適化操作を実行します。 |
|
|  | [Deleting](#Deleting) | インデックスは削除操作を実行します。 |
|
|  | [Renaming](#Renaming) | インデックスは名前変更操作を実行します。 |
|
|  | [ChangingAttributes](#ChangingAttributes) | インデックスは属性を変更します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Ready {#Ready}
```
public static final IndexStatus Ready
```


インデックスは空きがあり、変更の準備ができています。


### Failed {#Failed}
```
public static final IndexStatus Failed
```


エラーのため、インデックスを再読み込みする必要があります。


### Indexing {#Indexing}
```
public static final IndexStatus Indexing
```


インデックスはインデックス作成操作を実行します。


### Updating {#Updating}
```
public static final IndexStatus Updating
```


インデックスは更新操作を実行します。


### Merging {#Merging}
```
public static final IndexStatus Merging
```


インデックスはマージ操作を実行します。


### Optimizing {#Optimizing}
```
public static final IndexStatus Optimizing
```


インデックスは最適化操作を実行します。


### Deleting {#Deleting}
```
public static final IndexStatus Deleting
```


インデックスは削除操作を実行します。


### Renaming {#Renaming}
```
public static final IndexStatus Renaming
```


インデックスは名前変更操作を実行します。


### ChangingAttributes {#ChangingAttributes}
```
public static final IndexStatus ChangingAttributes
```


インデックスは属性を変更します。


### values() {#values--}
```
public static IndexStatus[] values()
```




**Returns:**
com.groupdocs.search.common.IndexStatus[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static IndexStatus valueOf(String name)
```




**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[IndexStatus](../../com.groupdocs.search.common/indexstatus)
