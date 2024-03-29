---
title: OperationProgressEventArgs
second_title: GroupDocs.Search for .NET API リファレンス
description: インデックス操作の進行状況が更新されるイベントの引数を表します
type: docs
weight: 560
url: /ja/net/groupdocs.search.events/operationprogresseventargs/
---
## OperationProgressEventArgs class

インデックス操作の進行状況が更新されるイベントの引数を表します。

```csharp
public class OperationProgressEventArgs : BaseIndexEventArgs
```

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [IndexFolder](../../groupdocs.search.events/baseindexeventargs/indexfolder) { get; } | インデックス フォルダーを取得します。 |
| [IndexId](../../groupdocs.search.events/baseindexeventargs/indexid) { get; } | インデックス ID を取得します。 |
| [LastDocumentKey](../../groupdocs.search.events/operationprogresseventargs/lastdocumentkey) { get; } | 最後に処理されたドキュメントのキーを取得します。 |
| [LastDocumentPath](../../groupdocs.search.events/operationprogresseventargs/lastdocumentpath) { get; } | 最後に処理されたドキュメントのパスを取得します。 |
| [LastDocumentStatus](../../groupdocs.search.events/operationprogresseventargs/lastdocumentstatus) { get; } | 最後に処理されたドキュメントのステータスを取得します。 |
| [ProcessedDocuments](../../groupdocs.search.events/operationprogresseventargs/processeddocuments) { get; } | 正常に処理されたドキュメントの数を取得します。 |
| [ProgressPercentage](../../groupdocs.search.events/operationprogresseventargs/progresspercentage) { get; } | 進行状況のパーセンテージを取得します。 |
| [SkippedDocuments](../../groupdocs.search.events/operationprogresseventargs/skippeddocuments) { get; } | スキップされたドキュメントの数を取得します。 |
| [Status](../../groupdocs.search.events/baseindexeventargs/status) { get; } | インデックスの状態を取得します。 |
| [Time](../../groupdocs.search.events/baseindexeventargs/time) { get; } | イベントの時刻を取得します。 |
| [TotalDocuments](../../groupdocs.search.events/operationprogresseventargs/totaldocuments) { get; } | 処理されたドキュメントの総数を取得します。 |

### 備考

**もっと詳しく知る**

* [検索インデックス イベント](https://docs.groupdocs.com/display/searchnet/Search+index+events)

### 関連項目

* class [BaseIndexEventArgs](../baseindexeventargs)
* 名前空間 [GroupDocs.Search.Events](../../groupdocs.search.events)
* 組み立て [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
