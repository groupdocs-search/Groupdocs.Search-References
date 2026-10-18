---
title: "NetworkSearchResult"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "検索クエリに一致する検索結果を表します。"
type: docs
weight: 14
url: /ja/java/com.groupdocs.search.scaling.results/networksearchresult/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public abstract class NetworkSearchResult implements Iterable<NetworkFoundDocument>
```

検索クエリに一致する検索結果を表します。

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [NetworkSearchResult()](#NetworkSearchResult--) |  |
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getDocumentCount()](#getDocumentCount--) | 見つかったドキュメント数を取得します。 |
|
|  | [getOccurrenceCount()](#getOccurrenceCount--) | 見つかった総出現回数を取得します。 |
|
|  | [getTruncated()](#getTruncated--) | 結果が切り詰められていることを示す値を取得します。 |
|
|  | [getWarnings()](#getWarnings--) | 結果を説明する警告を取得します。 |
|
|  | [getStartTime()](#getStartTime--) | 検索の開始時刻を取得します。 |
|
|  | [getEndTime()](#getEndTime--) | 検索の終了時刻を取得します。 |
|
|  | [getSearchDuration()](#getSearchDuration--) | 検索の所要時間（秒）を取得します。 |
|
|  | [getFoundDocument(int index)](#getFoundDocument-int-) | インデックスで見つかったドキュメントを取得します。 |
|
|  | [iterator()](#iterator--) | 見つかったドキュメントのコレクションを反復処理するイテレータを返します。 |
|
|  | [getNextChunkSearchToken()](#getNextChunkSearchToken--) | 次のチャンクを検索するためのチャンク検索トークンを取得します。 |
|
|  | [getNodeIndex()](#getNodeIndex--) | 結果が受信されたノードのインデックスを取得します。 |
|
### NetworkSearchResult() {#NetworkSearchResult--}
```
public NetworkSearchResult()
```


### getDocumentCount() {#getDocumentCount--}
```
public abstract int getDocumentCount()
```


見つかったドキュメント数を取得します。


**Returns:**
int - 見つかったドキュメント数。

### getOccurrenceCount() {#getOccurrenceCount--}
```
public abstract int getOccurrenceCount()
```


見つかった総出現回数を取得します。


**Returns:**
int - 見つかった総出現回数。

### getTruncated() {#getTruncated--}
```
public abstract boolean getTruncated()
```


結果が切り詰められていることを示す値を取得します。


**Returns:**
boolean - 結果が切り詰められていることを示す値。

### getWarnings() {#getWarnings--}
```
public abstract String getWarnings()
```


結果を説明する警告を取得します。


**Returns:**
java.lang.String - 結果を説明する警告。

### getStartTime() {#getStartTime--}
```
public abstract Date getStartTime()
```


検索の開始時刻を取得します。


**Returns:**
java.util.Date - 検索の開始時刻。

### getEndTime() {#getEndTime--}
```
public abstract Date getEndTime()
```


検索の終了時刻を取得します。


**Returns:**
java.util.Date - 検索の終了時刻。

### getSearchDuration() {#getSearchDuration--}
```
public abstract double getSearchDuration()
```


検索の所要時間（秒）を取得します。


**Returns:**
double - 検索の所要時間（秒）。

### getFoundDocument(int index) {#getFoundDocument-int-}
```
public abstract NetworkFoundDocument getFoundDocument(int index)
```


インデックスで見つかったドキュメントを取得します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | インデックス | int | 見つかったドキュメントのインデックス。 |
|

**Returns:**
[NetworkFoundDocument](../../com.groupdocs.search.scaling.results/networkfounddocument) - The found document.

### iterator() {#iterator--}
```
public abstract Iterator<NetworkFoundDocument> iterator()
```


見つかったドキュメントのコレクションを反復処理するイテレータを返します。


**Returns:**
java.util.Iterator<com.groupdocs.search.scaling.results.NetworkFoundDocument> - 見つかったドキュメントのコレクションを反復処理できるイテレータ。

### getNextChunkSearchToken() {#getNextChunkSearchToken--}
```
public abstract NetworkSearchToken getNextChunkSearchToken()
```


次のチャンクを検索するためのチャンク検索トークンを取得します。


**Returns:**
[NetworkSearchToken](../../com.groupdocs.search.scaling.results/networksearchtoken) - A chunk search token for searching the next chunk.

### getNodeIndex() {#getNodeIndex--}
```
public abstract int getNodeIndex()
```


結果が受信されたノードのインデックスを取得します。


**Returns:**
int - 結果が受信されたノードのインデックス。

