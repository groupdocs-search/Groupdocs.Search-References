---
title: "OptimizationProgressEventArgs"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "インデックス作成操作の進行状況が更新されたイベントの引数を表します。"
type: docs
weight: 19
url: /ja/java/com.groupdocs.search.events/optimizationprogresseventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class OptimizationProgressEventArgs extends BaseIndexEventArgs
```

インデックス作成操作の進行状況が更新されたイベントの引数を表します。


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getTotalSegments()](#getTotalSegments--) | 処理対象のセグメント総数を取得します。 |
|
|  | [getProcessedSegments()](#getProcessedSegments--) | 処理されたセグメント数を取得します。 |
|
|  | [getProgressPercentage()](#getProgressPercentage--) | 進捗のパーセンテージを取得します。 |
|
### getTotalSegments() {#getTotalSegments--}
```
public final int getTotalSegments()
```


処理対象のセグメント総数を取得します。


**Returns:**
int - 処理対象のセグメント総数。

### getProcessedSegments() {#getProcessedSegments--}
```
public final int getProcessedSegments()
```


処理されたセグメント数を取得します。


**Returns:**
int - 処理されたセグメント数。

### getProgressPercentage() {#getProgressPercentage--}
```
public final double getProgressPercentage()
```


進捗のパーセンテージを取得します。


**Returns:**
double - 進捗のパーセンテージ。

