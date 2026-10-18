---
title: "NetworkFoundDocument"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "検索ネットワーク内で見つかったドキュメントを表します。"
type: docs
weight: 11
url: /ja/java/com.groupdocs.search.scaling.results/networkfounddocument/
---
**Inheritance:**
java.lang.Object
```
public abstract class NetworkFoundDocument
```

検索ネットワーク内で見つかったドキュメントを表します。

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [NetworkFoundDocument()](#NetworkFoundDocument--) |  |
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getFoundDocument()](#getFoundDocument--) | 見つかったドキュメントを取得します。 |
|
|  | [getShardIndex()](#getShardIndex--) | シャードインデックスを取得します。 |
|
### NetworkFoundDocument() {#NetworkFoundDocument--}
```
public NetworkFoundDocument()
```


### getFoundDocument() {#getFoundDocument--}
```
public abstract FoundDocument getFoundDocument()
```


見つかったドキュメントを取得します。


**Returns:**
[FoundDocument](../../com.groupdocs.search.results/founddocument) - The found document.

### getShardIndex() {#getShardIndex--}
```
public abstract int getShardIndex()
```


シャードインデックスを取得します。


**Returns:**
int - シャードインデックス。

