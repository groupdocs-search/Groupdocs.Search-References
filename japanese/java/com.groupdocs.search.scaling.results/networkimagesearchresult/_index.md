---
title: "NetworkImageSearchResult"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "検索画像に一致する画像検索結果を表します。"
type: docs
weight: 12
url: /ja/java/com.groupdocs.search.scaling.results/networkimagesearchresult/
---
**Inheritance:**
java.lang.Object
```
public abstract class NetworkImageSearchResult
```

検索画像に一致する画像検索結果を表します。

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [NetworkImageSearchResult()](#NetworkImageSearchResult--) |  |
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getImageCount()](#getImageCount--) | 見つかった画像の数を取得します。 |
|
|  | [getFoundImage(int index)](#getFoundImage-int-) | インデックスで取得した画像を取得します。 |
|
|  | [getNetworkImageSearchToken()](#getNetworkImageSearchToken--) | 次のチャンクを検索するためのチャンク画像検索トークンを取得します。 |
|
|  | [getNodeIndex()](#getNodeIndex--) | 結果が受信されたノードのインデックスを取得します。 |
|
|  | [getShardIndex()](#getShardIndex--) | 結果が受信されたシャードのインデックスを取得します。 |
|
### NetworkImageSearchResult() {#NetworkImageSearchResult--}
```
public NetworkImageSearchResult()
```


### getImageCount() {#getImageCount--}
```
public abstract int getImageCount()
```


見つかった画像の数を取得します。


**Returns:**
int - 見つかった画像の数。

### getFoundImage(int index) {#getFoundImage-int-}
```
public abstract FoundImageFrame getFoundImage(int index)
```


インデックスで取得した画像を取得します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | インデックス | int | 見つかった画像のインデックス。 |
|

**Returns:**
[FoundImageFrame](../../com.groupdocs.search.results/foundimageframe) - The found image.

### getNetworkImageSearchToken() {#getNetworkImageSearchToken--}
```
public abstract NetworkImageSearchToken getNetworkImageSearchToken()
```


次のチャンクを検索するためのチャンク画像検索トークンを取得します。


**Returns:**
[NetworkImageSearchToken](../../com.groupdocs.search.scaling.results/networkimagesearchtoken) - A chunk image search token for searching the next chunk.

### getNodeIndex() {#getNodeIndex--}
```
public abstract int getNodeIndex()
```


結果が受信されたノードのインデックスを取得します。


**Returns:**
int - 結果が受信されたノードのインデックス。

### getShardIndex() {#getShardIndex--}
```
public abstract int getShardIndex()
```


結果が受信されたシャードのインデックスを取得します。


**Returns:**
int - 結果が受信されたシャードのインデックス。

