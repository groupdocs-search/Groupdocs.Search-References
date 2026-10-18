---
title: "NetworkOptimizationProgressEventArgs"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "最適化操作の進行状況変更イベントの引数を表します。"
type: docs
weight: 15
url: /ja/java/com.groupdocs.search.scaling.events/networkoptimizationprogresseventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class NetworkOptimizationProgressEventArgs extends EventArgs
```

最適化操作の進行状況変更イベントの引数を表します。

## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getNodeIndex()](#getNodeIndex--) | 検索ネットワークノードのインデックスを取得します。 |
|
|  | [getServiceIndex()](#getServiceIndex--) | 検索ネットワークノードサービスのインデックスを取得します。 |
|
|  | [getProcessedSegments()](#getProcessedSegments--) | 処理されたセグメント数を取得します。 |
|
|  | [getTotalSegments()](#getTotalSegments--) | 処理対象のセグメント総数を取得します。 |
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

### getProcessedSegments() {#getProcessedSegments--}
```
public final int getProcessedSegments()
```


処理されたセグメント数を取得します。


**Returns:**
int - 処理されたセグメント数。

### getTotalSegments() {#getTotalSegments--}
```
public final int getTotalSegments()
```


処理対象のセグメント総数を取得します。


**Returns:**
int - 処理対象のセグメント総数。

### getProgressPercentage() {#getProgressPercentage--}
```
public final double getProgressPercentage()
```


進捗のパーセンテージを取得します。


**Returns:**
double - 進捗のパーセンテージ。

