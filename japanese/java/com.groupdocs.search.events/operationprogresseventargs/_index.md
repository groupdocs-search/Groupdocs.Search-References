---
title: "OperationProgressEventArgs"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "インデックス作成操作の進行状況が更新されたイベントの引数を表します。"
type: docs
weight: 18
url: /ja/java/com.groupdocs.search.events/operationprogresseventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class OperationProgressEventArgs extends BaseIndexEventArgs
```

インデックス作成操作の進行状況が更新されたイベントの引数を表します。


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getTotalDocuments()](#getTotalDocuments--) | 処理対象のドキュメント総数を取得します。 |
|
|  | [getProcessedDocuments()](#getProcessedDocuments--) | 正常に処理されたドキュメントの数を取得します。 |
|
|  | [getSkippedDocuments()](#getSkippedDocuments--) | スキップされたドキュメントの数を取得します。 |
|
|  | [getProgressPercentage()](#getProgressPercentage--) | 進捗のパーセンテージを取得します。 |
|
|  | [getLastDocumentKey()](#getLastDocumentKey--) | 最後に処理されたドキュメントのキーを取得します。 |
|
|  | [getLastDocumentPath()](#getLastDocumentPath--) | 最後に処理されたドキュメントのパスを取得します。 |
|
|  | [getLastDocumentStatus()](#getLastDocumentStatus--) | 最後に処理されたドキュメントのステータスを取得します。 |
|
### getTotalDocuments() {#getTotalDocuments--}
```
public final int getTotalDocuments()
```


処理対象のドキュメント総数を取得します。


**Returns:**
int - 処理対象のドキュメント総数。

### getProcessedDocuments() {#getProcessedDocuments--}
```
public final int getProcessedDocuments()
```


正常に処理されたドキュメントの数を取得します。


**Returns:**
int - 正常に処理されたドキュメントの数。

### getSkippedDocuments() {#getSkippedDocuments--}
```
public final int getSkippedDocuments()
```


スキップされたドキュメントの数を取得します。


**Returns:**
int - スキップされたドキュメントの数。

### getProgressPercentage() {#getProgressPercentage--}
```
public final double getProgressPercentage()
```


進捗のパーセンテージを取得します。


**Returns:**
double - 進捗のパーセンテージ。

### getLastDocumentKey() {#getLastDocumentKey--}
```
public final String getLastDocumentKey()
```


最後に処理されたドキュメントのキーを取得します。


**Returns:**
java.lang.String - 最後に処理されたドキュメントのキー。

### getLastDocumentPath() {#getLastDocumentPath--}
```
public final String getLastDocumentPath()
```


最後に処理されたドキュメントのパスを取得します。


**Returns:**
java.lang.String - 最後に処理されたドキュメントのパス。

### getLastDocumentStatus() {#getLastDocumentStatus--}
```
public final DocumentStatus getLastDocumentStatus()
```


最後に処理されたドキュメントのステータスを取得します。


**Returns:**
[DocumentStatus](../../com.groupdocs.search.common/documentstatus) - The last processed document status.

