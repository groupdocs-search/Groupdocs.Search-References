---
title: "NetworkIndexingProgressEventArgs"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "インデックス作成操作の進行状況変更イベントの引数を表します。"
type: docs
weight: 14
url: /ja/java/com.groupdocs.search.scaling.events/networkindexingprogresseventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class NetworkIndexingProgressEventArgs extends EventArgs
```

インデックス作成操作の進行状況変更イベントの引数を表します。

## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getNodeIndex()](#getNodeIndex--) | 検索ネットワークノードのインデックスを取得します。 |
|
|  | [getServiceIndex()](#getServiceIndex--) | 検索ネットワークノードサービスのインデックスを取得します。 |
|
|  | [getProcessedDocuments()](#getProcessedDocuments--) | 処理されたドキュメントの数を取得します。 |
|
|  | [getTotalDocuments()](#getTotalDocuments--) | 処理対象のドキュメント総数を取得します。 |
|
|  | [getProgressPercentage()](#getProgressPercentage--) | 進捗のパーセンテージを取得します。 |
|
### getNodeIndex() {#getNodeIndex--}
```
public final int getNodeIndex()
```


検索ネットワークノードのインデックスを取得します。


**Returns:**
int - 検索ネットワークノードのインデックス。

### getServiceIndex() {#getServiceIndex--}
```
public final int getServiceIndex()
```


検索ネットワークノードサービスのインデックスを取得します。


**Returns:**
int - 検索ネットワークノードサービスのインデックス。

### getProcessedDocuments() {#getProcessedDocuments--}
```
public final int getProcessedDocuments()
```


処理されたドキュメントの数を取得します。


**Returns:**
int - 処理されたドキュメントの数。

### getTotalDocuments() {#getTotalDocuments--}
```
public final int getTotalDocuments()
```


処理対象のドキュメント総数を取得します。


**Returns:**
int - 処理対象のドキュメント総数。

### getProgressPercentage() {#getProgressPercentage--}
```
public final double getProgressPercentage()
```


進捗のパーセンテージを取得します。


**Returns:**
double - 進捗のパーセンテージ。

