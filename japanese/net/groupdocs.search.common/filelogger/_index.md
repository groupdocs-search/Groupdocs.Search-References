---
title: FileLogger
second_title: GroupDocs.Search for .NET API リファレンス
description: イベントとエラーをローカル ファイルに記録するロガーを表します
type: docs
weight: 140
url: /ja/net/groupdocs.search.common/filelogger/
---
## FileLogger class

イベントとエラーをローカル ファイルに記録するロガーを表します。

```csharp
public class FileLogger : ILogger
```

## コンストラクター

| 名前 | 説明 |
| --- | --- |
| [FileLogger](filelogger)(string, double) | の新しいインスタンスを初期化します[`FileLogger`](../filelogger)class. |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [FilePath](../../groupdocs.search.common/filelogger/filepath) { get; } | ログファイルのパスを取得します。 |
| [MaxSize](../../groupdocs.search.common/filelogger/maxsize) { get; } | ログ ファイルの最大サイズをメガバイト単位で取得します。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| [Error](../../groupdocs.search.common/filelogger/error)(string) | インデックスで発生したエラーを記録します。 |
| [Trace](../../groupdocs.search.common/filelogger/trace)(string) | インデックスで発生したイベントを記録します。 |

### 備考

**もっと詳しく知る**

* [ロギング](https://docs.groupdocs.com/display/searchnet/Logging)

### 例

この例は、クラスの典型的な使用法を示しています.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";
string logPath = @"c:\Log.txt";

IndexSettings settings = new IndexSettings();
settings.Logger = new FileLogger(logPath, 4.0); // ログ ファイルへのパスと最大長 4 MB を指定

Index index = new Index(indexFolder, settings); // 指定したフォルダにインデックスを作成

index.Add(documentsFolder); // 指定されたフォルダからのドキュメントのインデックス作成

SearchResult result = index.Search(query); // インデックスで検索
```

### 関連項目

* interface [ILogger](../ilogger)
* 名前空間 [GroupDocs.Search.Common](../../groupdocs.search.common)
* 組み立て [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->