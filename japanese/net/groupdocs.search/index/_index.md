---
title: Index
second_title: GroupDocs.Search for .NET API リファレンス
description: ドキュメントのインデックス作成と検索を行うためのメイン クラスを表します
type: docs
weight: 680
url: /ja/net/groupdocs.search/index/
---
## Index class

ドキュメントのインデックス作成と検索を行うためのメイン クラスを表します。

```csharp
public class Index : IDisposable
```

## コンストラクター

| 名前 | 説明 |
| --- | --- |
| [Index](index#constructor)() | の新しいインスタンスを初期化します[`Index`](../index)メモリ内のクラス. |
| [Index](index#constructor_1)(IndexSettings) | の新しいインスタンスを初期化します[`Index`](../index)特定のインデックス設定を持つメモリ内のクラス. |
| [Index](index#constructor_2)(string) | の新しいインスタンスを初期化します[`Index`](../index) class. ディスク上に新しいインデックスを作成するか、既存のインデックスを開きます。 |
| [Index](index#constructor_3)(string, bool) | の新しいインスタンスを初期化します[`Index`](../index) class. 次の場合に、ディスクから既存のインデックスをロードします。*overwriteIfExists*は`間違い`; それ以外の場合、ディスク上に新しいインデックスを作成します. |
| [Index](index#constructor_4)(string, IndexSettings) | の新しいインスタンスを初期化します[`Index`](../index) class. 特定の設定で新しいインデックスを作成するか、ディスク上の既存のインデックスを開きます。 |
| [Index](index#constructor_5)(string, IndexSettings, bool) | の新しいインスタンスを初期化します[`Index`](../index) class. 次の場合に、ディスクから既存のインデックスをロードします。*overwriteIfExists*は`間違い` ; は、特定のインデックス設定を使用して、ディスク上に新しいインデックスを作成します. |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [Dictionaries](../../groupdocs.search/index/dictionaries) { get; } | ディクショナリ リポジトリを取得します。 |
| [Events](../../groupdocs.search/index/events) { get; } | イベントをサブスクライブするためのイベント ハブを取得します。 |
| [IndexInfo](../../groupdocs.search/index/indexinfo) { get; } | インデックスの基本情報を取得します。 |
| [IndexSettings](../../groupdocs.search/index/indexsettings) { get; } | インデックス設定を取得します。 |
| [Repository](../../groupdocs.search/index/repository) { get; } | インデックスが含まれている場合、インデックス リポジトリ オブジェクトを取得します。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| [Add](../../groupdocs.search/index/add#add_2)(string) | インデックス作成操作を実行します. 絶対パスまたは相対パスでファイルまたはフォルダーを追加します. すべてのサブフォルダーのドキュメントがインデックス化されます. |
| [Add](../../groupdocs.search/index/add#add_4)(string[]) | インデックス作成操作を実行します。 絶対パスまたは相対パスでファイルまたはフォルダーを追加します。 すべてのサブフォルダーのドキュメントがインデックス作成されます。 |
| [Add](../../groupdocs.search/index/add#add)(Document[], IndexingOptions) | インデックス作成操作を実行します。 ファイル システム、ストリーム、または構造からドキュメントを追加します。 |
| [Add](../../groupdocs.search/index/add#add_1)(ExtractedData[], IndexingOptions) | インデックス操作を実行します。 抽出したデータをインデックスに追加します。 |
| [Add](../../groupdocs.search/index/add#add_3)(string, IndexingOptions) | インデックス作成操作を実行します. 絶対パスまたは相対パスでファイルまたはフォルダーを追加します. すべてのサブフォルダーのドキュメントがインデックス化されます. |
| [Add](../../groupdocs.search/index/add#add_5)(string[], IndexingOptions) | インデックス作成操作を実行します。 絶対パスまたは相対パスでファイルまたはフォルダーを追加します。 すべてのサブフォルダーのドキュメントがインデックス作成されます。 |
| [ChangeAttributes](../../groupdocs.search/index/changeattributes)(AttributeChangeBatch) | 更新操作中にインデックスを再作成せずに、属性変更の指定されたバッチをインデックス付きドキュメントに適用します。 |
| [Delete](../../groupdocs.search/index/delete#delete_1)(string[], UpdateOptions) | インデックス化されたファイルまたはフォルダーをインデックスから削除します。次に、パスを削除せずにインデックスを更新します。 フォルダーの一部としてインデックスに追加された場合、個々のドキュメントをインデックスから削除できないことに注意してください。 |
| [Delete](../../groupdocs.search/index/delete#delete)(UpdateOptions, string[]) | ストリームまたは構造から索引付けされた文書を削除します。次に、削除されたドキュメントなしでインデックスを更新します. |
| [Dispose](../../groupdocs.search/index/dispose)() | によって使用されているすべてのリソースを解放します。[`Index`](../index). |
| [GetAttributes](../../groupdocs.search/index/getattributes)(string) | 指定されたインデックス付きドキュメントに関連付けられているすべての属性を取得します。 |
| [GetDocumentText](../../groupdocs.search/index/getdocumenttext#getdocumenttext)(DocumentInfo, OutputAdapter) | インデックス付きドキュメントの HTML 形式のテキストを生成し、出力アダプターを介して転送します。 |
| [GetDocumentText](../../groupdocs.search/index/getdocumenttext#getdocumenttext_1)(DocumentInfo, OutputAdapter, TextOptions) | インデックス付きドキュメントの HTML 形式のテキストを生成し、出力アダプターを介して転送します。 |
| [GetIndexedDocumentItems](../../groupdocs.search/index/getindexeddocumentitems)(DocumentInfo) | 指定されたドキュメントのネストされたアイテムの配列を取得します (ZIP、OST、PST などのコンテナー ドキュメントの場合)。 |
| [GetIndexedDocuments](../../groupdocs.search/index/getindexeddocuments)() | すべてのインデックス付きドキュメントの配列を取得します。 |
| [GetIndexedPaths](../../groupdocs.search/index/getindexedpaths)() | インデックス付きパス (ドキュメントまたはフォルダー) の配列を取得します。 |
| [GetIndexingReports](../../groupdocs.search/index/getindexingreports)() | インデックス作成操作に関するレポートを取得します。 |
| [GetSearchReports](../../groupdocs.search/index/getsearchreports)() | 検索操作に関するレポートを取得します。 |
| [Highlight](../../groupdocs.search/index/highlight#highlight)(FoundDocument, Highlighter) | 見つかった用語が強調表示された HTML 形式のテキストを生成します。 |
| [Highlight](../../groupdocs.search/index/highlight#highlight_1)(FoundDocument, Highlighter, HighlightOptions) | 見つかった用語が強調表示された HTML 形式のテキストを生成します。 |
| [Merge](../../groupdocs.search/index/merge#merge)(Index, MergeOptions) | 指定されたインデックスを現在のインデックスにマージします。 他のインデックスは変更されないことに注意してください。 |
| [Merge](../../groupdocs.search/index/merge#merge_1)(IndexRepository, MergeOptions) | 指定したインデックス リポジトリのインデックスを現在のインデックスにマージします。 リポジトリ内のインデックスは変更されないことに注意してください。 |
| [Notify](../../groupdocs.search/index/notify)(Notification) | 指定された通知オブジェクトをインデックスに渡して、通知を実行します。 |
| [Optimize](../../groupdocs.search/index/optimize#optimize)() | インデックス セグメントをマージすることにより、インデックス セグメントの数を最小限に抑えます。 この操作により、検索のパフォーマンスが向上します。 |
| [Optimize](../../groupdocs.search/index/optimize#optimize_1)(MergeOptions) | インデックス セグメントをマージすることにより、インデックス セグメントの数を最小限に抑えます。 この操作により、検索のパフォーマンスが向上します。 |
| [Search](../../groupdocs.search/index/search#search_1)(SearchQuery) | index. で検索します。 |
| [Search](../../groupdocs.search/index/search#search_3)(string) | index. で検索します。 |
| [Search](../../groupdocs.search/index/search#search)(SearchImage, ImageSearchOptions) | インデックスで画像の逆検索を実行します。 |
| [Search](../../groupdocs.search/index/search#search_2)(SearchQuery, SearchOptions) | index. で検索します。 |
| [Search](../../groupdocs.search/index/search#search_4)(string, SearchOptions) | index. で検索します。 |
| [SearchNext](../../groupdocs.search/index/searchnext#searchnext)(ChunkSearchToken) | メソッド Search. で開始されたチャンク検索を続行します。 |
| [SearchNext](../../groupdocs.search/index/searchnext#searchnext_1)(ChunkSearchToken, Cancellation) | メソッド Search. で開始されたチャンク検索を続行します。 |
| [Update](../../groupdocs.search/index/update#update)() | 前回の更新以降に変更または削除されたドキュメントのインデックスを再作成します。 インデックス付きフォルダーに追加された新しいファイルを追加します。 |
| [Update](../../groupdocs.search/index/update#update_1)(UpdateOptions) | 前回の更新以降に変更または削除されたドキュメントのインデックスを再作成します。 インデックス付きフォルダーに追加された新しいファイルを追加します。 |

### 備考

**もっと詳しく知る**

* [索引の作成](https://docs.groupdocs.com/display/searchnet/Creating+an+index)
* [索引付け](https://docs.groupdocs.com/display/searchnet/Indexing)
* [検索中](https://docs.groupdocs.com/display/searchnet/Searching)

### 例

この例は、クラスの典型的な使用法を示しています.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

Index index = new Index(indexFolder); // 指定したフォルダにインデックスを作成
index.Add(documentsFolder); // 指定されたフォルダからのドキュメントのインデックス作成

SearchResult result = index.Search(query); // インデックスで検索
```

### 関連項目

* 名前空間 [GroupDocs.Search](../../groupdocs.search)
* 組み立て [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
