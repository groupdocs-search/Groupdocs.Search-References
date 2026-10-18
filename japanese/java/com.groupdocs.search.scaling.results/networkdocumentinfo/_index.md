---
title: "NetworkDocumentInfo"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "検索ネットワーク内のインデックス化されたドキュメントの記述子を表します。"
type: docs
weight: 10
url: /ja/java/com.groupdocs.search.scaling.results/networkdocumentinfo/
---
**Inheritance:**
java.lang.Object
```
public abstract class NetworkDocumentInfo
```

検索ネットワーク内のインデックス化されたドキュメントの記述子を表します。

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [NetworkDocumentInfo()](#NetworkDocumentInfo--) |  |
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getDocumentInfo()](#getDocumentInfo--) | インデックス化されたドキュメントの記述子を取得します。 |
|
|  | [getShardIndex()](#getShardIndex--) | シャードインデックスを取得します。 |
|
### NetworkDocumentInfo() {#NetworkDocumentInfo--}
```
public NetworkDocumentInfo()
```


### getDocumentInfo() {#getDocumentInfo--}
```
public abstract DocumentInfo getDocumentInfo()
```


インデックス化されたドキュメントの記述子を取得します。


**Returns:**
[DocumentInfo](../../com.groupdocs.search.results/documentinfo) - The descriptor for an indexed document.

### getShardIndex() {#getShardIndex--}
```
public abstract int getShardIndex()
```


シャードインデックスを取得します。


**Returns:**
int - シャードインデックス。

