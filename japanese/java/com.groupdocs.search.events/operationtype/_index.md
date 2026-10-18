---
title: "OperationType"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "インデックス操作の種類を表します。"
type: docs
weight: 23
url: /ja/java/com.groupdocs.search.events/operationtype/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum OperationType extends Enum<OperationType>
```

インデックス操作の種類を表します。

## Fields

| Field | 説明 |
| --- | --- |
|  | [Indexing](#Indexing) | インデックスにドキュメントを追加します。 |
|
|  | [Updating](#Updating) | インデックス内のドキュメントを更新します。 |
|
|  | [Merging](#Merging) | インデックスをマージします。 |
|
|  | [Optimizing](#Optimizing) | インデックスを最適化します。 |
|
|  | [Deleting](#Deleting) | インデックスからパスを削除します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Indexing {#Indexing}
```
public static final OperationType Indexing
```


インデックスにドキュメントを追加します。


### Updating {#Updating}
```
public static final OperationType Updating
```


インデックス内のドキュメントを更新します。


### Merging {#Merging}
```
public static final OperationType Merging
```


インデックスをマージします。


### Optimizing {#Optimizing}
```
public static final OperationType Optimizing
```


インデックスを最適化します。


### Deleting {#Deleting}
```
public static final OperationType Deleting
```


インデックスからパスを削除します。


### values() {#values--}
```
public static OperationType[] values()
```




**Returns:**
com.groupdocs.search.events.OperationType[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static OperationType valueOf(String name)
```




**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[OperationType](../../com.groupdocs.search.events/operationtype)
