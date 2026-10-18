---
title: "SearchNetworkStatus"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "検索ネットワークのステータスを指定します。"
type: docs
weight: 13
url: /ja/java/com.groupdocs.search.scaling/searchnetworkstatus/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum SearchNetworkStatus extends Enum<SearchNetworkStatus>
```

検索ネットワークのステータスを指定します。

## Fields

| Field | 説明 |
| --- | --- |
|  | [Ready](#Ready) | 検索ネットワークは空きがあり、変更の準備ができています。 |
|
|  | [Configuring](#Configuring) | 検索ネットワークは構成操作を実行しています。 |
|
|  | [Indexing](#Indexing) | 検索ネットワークはインデックス作成操作を実行します。 |
|
|  | [Optimizing](#Optimizing) | 検索ネットワークは最適化操作を実行します。 |
|
|  | [Deleting](#Deleting) | 検索ネットワークは削除操作を実行します。 |
|
|  | [ChangingAttributes](#ChangingAttributes) | 検索ネットワークは属性を変更します。 |
|
|  | [Synchronizing](#Synchronizing) | 検索ネットワークは同期操作を実行します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Ready {#Ready}
```
public static final SearchNetworkStatus Ready
```


検索ネットワークは空きがあり、変更の準備ができています。


### Configuring {#Configuring}
```
public static final SearchNetworkStatus Configuring
```


検索ネットワークは構成操作を実行しています。


### Indexing {#Indexing}
```
public static final SearchNetworkStatus Indexing
```


検索ネットワークはインデックス作成操作を実行します。


### Optimizing {#Optimizing}
```
public static final SearchNetworkStatus Optimizing
```


検索ネットワークは最適化操作を実行します。


### Deleting {#Deleting}
```
public static final SearchNetworkStatus Deleting
```


検索ネットワークは削除操作を実行します。


### ChangingAttributes {#ChangingAttributes}
```
public static final SearchNetworkStatus ChangingAttributes
```


検索ネットワークは属性を変更します。


### Synchronizing {#Synchronizing}
```
public static final SearchNetworkStatus Synchronizing
```


検索ネットワークは同期操作を実行します。


### values() {#values--}
```
public static SearchNetworkStatus[] values()
```




**Returns:**
com.groupdocs.search.scaling.SearchNetworkStatus[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static SearchNetworkStatus valueOf(String name)
```




**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[SearchNetworkStatus](../../com.groupdocs.search.scaling/searchnetworkstatus)
