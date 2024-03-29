---
title: DocumentHighlighter
second_title: GroupDocs.Search for .NET API リファレンス
description: ドキュメント テキスト全体で検索結果を強調表示する検索結果ハイライターを表します
type: docs
weight: 630
url: /ja/net/groupdocs.search.highlighters/documenthighlighter/
---
## DocumentHighlighter class

ドキュメント テキスト全体で検索結果を強調表示する検索結果ハイライターを表します。

```csharp
public class DocumentHighlighter : Highlighter
```

## コンストラクター

| 名前 | 説明 |
| --- | --- |
| [DocumentHighlighter](documenthighlighter)(OutputAdapter) | の新しいインスタンスを初期化します[`DocumentHighlighter`](../documenthighlighter)class. |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [OutputAdapter](../../groupdocs.search.highlighters/documenthighlighter/outputadapter) { get; } | コンストラクターで渡された出力アダプターを取得します。 |
| [OutputFormat](../../groupdocs.search.common/resultbuilderfactory/outputformat) { get; } | 出力形式を取得します。 |

### 備考

**もっと詳しく知る**

* [検索結果のハイライト](https://docs.groupdocs.com/display/searchnet/Highlighting+search+results)

### 例

この例は、クラスの典型的な使用法を示しています.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

// インデックスを作成する
Index index = new Index(indexFolder);

// 指定されたフォルダからのドキュメントのインデックス作成
index.Add(documentsFolder);

// フェーズ「相対性理論」を検索します
SearchResult result = index.Search("\"Theory of Relativity\"");

// ドキュメントのテキストで見つかった単語を強調表示する
FoundDocument document = result.GetFoundDocument(0);
OutputAdapter outputAdapter = new FileOutputAdapter(OutputFormat.Html, "Highlighted.html");
Highlighter highlighter = new DocumentHighlighter(outputAdapter);
index.Highlight(document, highlighter);
```

### 関連項目

* class [Highlighter](../highlighter)
* 名前空間 [GroupDocs.Search.Highlighters](../../groupdocs.search.highlighters)
* 組み立て [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
