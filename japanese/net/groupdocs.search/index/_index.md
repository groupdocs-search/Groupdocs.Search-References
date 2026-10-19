---
title: "Index"
second_title: "GroupDocs.Search for .NET API リファレンス"
description: "ドキュメントのインデックス作成と検索を行うメインクラスを表します。"
type: docs
weight: 700
url: /ja/net/groupdocs.search/index/
---
## Index class

ドキュメントのインデックス作成と検索を行うメインクラスを表します。

```csharp
public class Index : IDisposable
```

## コンストラクタ

| 名前 | 説明 |
| --- | --- |
| [Index](index#constructor)() | メモリ内で[`Index`](../index)クラスの新しいインスタンスを初期化します。 |
| [Index](index#constructor_1)(IndexSettings) | 特定のインデックス設定を使用して、メモリ内で[`Index`](../index)クラスの新しいインスタンスを初期化します。 |
| [Index](index#constructor_2)(string) | [`Index`](../index)クラスの新しいインスタンスを初期化します。ディスク上に新しいインデックスを作成するか、既存のインデックスを開きます。 |
| [Index](index#constructor_3)(string, bool) | [`Index`](../index) クラスの新しいインスタンスを初期化します。*overwriteIfExists* が `false` の場合はディスク上の既存インデックスをロードし、そうでなければディスク上に新しいインデックスを作成します。 |
| [Index](index#constructor_4)(string, IndexSettings) | [`Index`](../index) クラスの新しいインスタンスを初期化します。特定の設定で新しいインデックスを作成するか、ディスク上の既存インデックスを開きます。 |
| [Index](index#constructor_5)(string, IndexSettings, bool) | [`Index`](../index) クラスの新しいインスタンスを初期化します。*overwriteIfExists* が `false` の場合はディスク上の既存インデックスをロードし、そうでなければ特定のインデックス設定でディスク上に新しいインデックスを作成します。 |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [Dictionaries](../../groupdocs.search/index/dictionaries) { get; } | 辞書リポジトリを取得します。 |
| [Events](../../groupdocs.search/index/events) { get; } | イベントの購読用にイベントハブを取得します。 |
| [IndexInfo](../../groupdocs.search/index/indexinfo) { get; } | インデックスの基本情報を取得します。 |
| [IndexSettings](../../groupdocs.search/index/indexsettings) { get; } | インデックス設定を取得します。 |
| [Repository](../../groupdocs.search/index/repository) { get; } | インデックスが含まれている場合、インデックスリポジトリオブジェクトを取得します。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| static [LoadIntoMemoryCompletely](../../groupdocs.search/index/loadintomemorycompletely#loadintomemorycompletely)(string) | インデックス全体をメモリにロードします。インデックスへの変更は元のフォルダーに自動的に保存されません。 |
| static [LoadIntoMemoryCompletely](../../groupdocs.search/index/loadintomemorycompletely#loadintomemorycompletely_1)(string, IndexSettings) | インデックス全体をメモリにロードします。インデックスへの変更は元のフォルダーに自動的に保存されません。 |
| [Add](../../groupdocs.search/index/add#add_2)(string) | インデックス作成操作を実行します。絶対パスまたは相対パスでファイルまたはフォルダーを追加します。すべてのサブフォルダーのドキュメントがインデックスされます。 |
| [Add](../../groupdocs.search/index/add#add_4)(string[]) | インデックス作成操作を実行します。絶対パスまたは相対パスでファイルやフォルダーを追加します。すべてのサブフォルダーのドキュメントがインデックスされます。 |
| [Add](../../groupdocs.search/index/add#add)(Document[], IndexingOptions) | インデックス作成操作を実行します。ファイルシステム、ストリーム、または構造からドキュメントを追加します。 |
| [Add](../../groupdocs.search/index/add#add_1)(ExtractedData[], IndexingOptions) | インデックス作成操作を実行します。抽出されたデータをインデックスに追加します。 |
| [Add](../../groupdocs.search/index/add#add_3)(string, IndexingOptions) | インデックス作成操作を実行します。絶対パスまたは相対パスでファイルまたはフォルダーを追加します。すべてのサブフォルダーのドキュメントがインデックスされます。 |
| [Add](../../groupdocs.search/index/add#add_5)(string[], IndexingOptions) | インデックス作成操作を実行します。絶対パスまたは相対パスでファイルやフォルダーを追加します。すべてのサブフォルダーのドキュメントがインデックスされます。 |
| [ChangeAttributes](../../groupdocs.search/index/changeattributes)(AttributeChangeBatch) | 更新操作中に再インデックス化せず、指定された属性変更バッチをインデックス済みドキュメントに適用します。 |
| [CheckSegments](../../groupdocs.search/index/checksegments)(bool) | ディスク上の破損したセグメントファイルがないかインデックスをチェックします。*fixIndexFunctionality* が true の場合、破損したセグメントが存在してもインデックス機能を修復します。そうでない場合は修復しません。 |
| [Delete](../../groupdocs.search/index/delete#delete_1)(string[], UpdateOptions) | インデックスからインデックス済みのファイルまたはフォルダーを削除します。その後、削除されたパスなしでインデックスを更新します。フォルダーの一部としてインデックスに追加された場合、個々のドキュメントはインデックスから削除できないことに注意してください。 |
| [Delete](../../groupdocs.search/index/delete#delete)(UpdateOptions, string[]) | ストリームまたは構造からインデックスされたドキュメントを削除します。その後、削除されたドキュメントなしでインデックスを更新します。 |
| [Dispose](../../groupdocs.search/index/dispose)() | [`Index`](../index) が使用するすべてのリソースを解放します。 |
| [GetAttributes](../../groupdocs.search/index/getattributes)(string) | 指定されたインデックス済みドキュメントに関連付けられたすべての属性を取得します。 |
| [GetDocumentText](../../groupdocs.search/index/getdocumenttext#getdocumenttext)(DocumentInfo, OutputAdapter) | インデックス済みドキュメントのテキストを生成し、出力アダプターを通して渡します。 |
| [GetDocumentText](../../groupdocs.search/index/getdocumenttext#getdocumenttext_1)(DocumentInfo, OutputAdapter, TextOptions) | インデックス済みドキュメントの HTML 形式テキストを生成し、出力アダプターを通して転送します。 |
| [GetIndexedDocument](../../groupdocs.search/index/getindexeddocument)(string) | ドキュメントキーでインデックス済みドキュメントを取得します。 |
| [GetIndexedDocumentItems](../../groupdocs.search/index/getindexeddocumentitems)(DocumentInfo) | 指定されたドキュメントのネストされた項目の配列を取得します（ZIP、OST、PST などのコンテナドキュメント用）。 |
| [GetIndexedDocuments](../../groupdocs.search/index/getindexeddocuments)() | すべてのインデックス済みドキュメントの配列を取得します。 |
| [GetIndexedPaths](../../groupdocs.search/index/getindexedpaths)() | インデックスされたパス（ドキュメントまたはフォルダー）の配列を取得します。 |
| [GetIndexingReports](../../groupdocs.search/index/getindexingreports)() | インデックス操作に関するレポートを取得します。 |
| [GetSearchReports](../../groupdocs.search/index/getsearchreports)() | 検索操作に関するレポートを取得します。 |
| [Highlight](../../groupdocs.search/index/highlight#highlight)(FoundDocument, Highlighter) | 見つかった用語をハイライトしたHTML形式のテキストを生成します。 |
| [Highlight](../../groupdocs.search/index/highlight#highlight_1)(FoundDocument, Highlighter, HighlightOptions) | 見つかった用語をハイライトしたHTML形式のテキストを生成します。 |
| [Merge](../../groupdocs.search/index/merge#merge)(Index, MergeOptions) | 指定されたインデックスを現在のインデックスにマージします。なお、他方のインデックスは変更されません。 |
| [Merge](../../groupdocs.search/index/merge#merge_1)(IndexRepository, MergeOptions) | 指定されたインデックスリポジトリからインデックスを現在のインデックスにマージします。リポジトリ内のインデックスは変更されません。 |
| [Notify](../../groupdocs.search/index/notify)(Notification) | 指定された通知オブジェクトをインデックスに渡して通知を実行します。 |
| [Optimize](../../groupdocs.search/index/optimize#optimize)() | インデックスセグメントの数を相互にマージすることで最小化します。この操作により検索パフォーマンスが向上します。 |
| [Optimize](../../groupdocs.search/index/optimize#optimize_1)(MergeOptions) | インデックスセグメントの数を相互にマージすることで最小化します。この操作により検索パフォーマンスが向上します。 |
| [SaveTo](../../groupdocs.search/index/saveto)(string) | インメモリインデックスをディスクに保存します。また、通常のインデックスを別のフォルダーに保存します。このインデックスの設定は変更されません。 |
| [Search](../../groupdocs.search/index/search#search_1)(SearchQuery) | インデックス内を検索します。 |
| [Search](../../groupdocs.search/index/search#search_3)(string) | インデックス内を検索します。 |
| [Search](../../groupdocs.search/index/search#search)(SearchImage, ImageSearchOptions) | インデックスで逆画像検索を実行します。 |
| [Search](../../groupdocs.search/index/search#search_2)(SearchQuery, SearchOptions) | インデックス内を検索します。 |
| [Search](../../groupdocs.search/index/search#search_4)(string, SearchOptions) | インデックス内を検索します。 |
| [SearchNext](../../groupdocs.search/index/searchnext#searchnext)(ChunkSearchToken) | メソッドSearchで開始されたチャンク検索を続行します。 |
| [SearchNext](../../groupdocs.search/index/searchnext#searchnext_1)(ChunkSearchToken, Cancellation) | メソッドSearchで開始されたチャンク検索を続行します。 |
| [Update](../../groupdocs.search/index/update#update)() | 前回の更新以降に変更または削除されたドキュメントを再インデックス化します。インデックス対象フォルダーに追加された新しいファイルを追加します。 |
| [Update](../../groupdocs.search/index/update#update_1)(UpdateOptions) | 前回の更新以降に変更または削除されたドキュメントを再インデックス化します。インデックス対象フォルダーに追加された新しいファイルを追加します。 |

### 備考

**Learn more**

* [Creating an index](https://docs.groupdocs.com/display/searchnet/Creating+an+index)
* [Indexing](https://docs.groupdocs.com/display/searchnet/Indexing)
* [Searching](https://docs.groupdocs.com/display/searchnet/Searching)

### 例

この例はクラスの典型的な使用方法を示しています。

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

SearchResult result = index.Search(query); // Searching in index
```

### 関連項目

* namespace [GroupDocs.Search](../../groupdocs.search)
* assembly [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.search.dll -->
