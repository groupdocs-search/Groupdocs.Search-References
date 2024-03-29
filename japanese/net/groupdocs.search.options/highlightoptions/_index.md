---
title: HighlightOptions
second_title: GroupDocs.Search for .NET API リファレンス
description: 見つかった用語を強調表示するためのオプションを提供します.
type: docs
weight: 860
url: /ja/net/groupdocs.search.options/highlightoptions/
---
## HighlightOptions class

見つかった用語を強調表示するためのオプションを提供します.

```csharp
public class HighlightOptions : TextOptions
```

## コンストラクター

| 名前 | 説明 |
| --- | --- |
| [HighlightOptions](highlightoptions)() | の新しいインスタンスを初期化します[`HighlightOptions`](../highlightoptions)class. |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [AdditionalFields](../../groupdocs.search.options/textoptions/additionalfields) { get; set; } | インデックス作成に使用された追加のドキュメント フィールドを取得または設定します。 デフォルト値は`ヌル`. この値は、ドキュメントのテキストがインデックスに保存されていない場合にのみ使用されることに注意してください. |
| [Cancellation](../../groupdocs.search.options/textoptions/cancellation) { get; set; } | キャンセル オブジェクトを取得または設定します。 デフォルト値は`ヌル`. |
| [CustomExtractor](../../groupdocs.search.options/textoptions/customextractor) { get; set; } | インデックス作成に使用されたカスタム テキスト エクストラクタを取得または設定します。 デフォルト値は`ヌル`. この値は、ドキュメントのテキストがインデックスに保存されていない場合にのみ使用されることに注意してください. |
| [GenerateHead](../../groupdocs.search.options/textoptions/generatehead) { get; set; } | 出力 HTML で Head タグが生成されるかどうかを示す値を取得または設定します。 デフォルト値は`真実`. |
| [HighlightColor](../../groupdocs.search.options/highlightoptions/highlightcolor) { get; set; } | オカレンスを強調表示するために使用される色を取得または設定します。 デフォルト値は #FFD800 です。 |
| [ImageIndexingOptions](../../groupdocs.search.options/textoptions/imageindexingoptions) { get; } | 画像逆検索の画像インデックス オプションを取得します。 |
| [MetadataIndexingOptions](../../groupdocs.search.options/textoptions/metadataindexingoptions) { get; } | メタデータ フィールドのインデックス作成のオプションを取得します。 |
| [OcrIndexingOptions](../../groupdocs.search.options/textoptions/ocrindexingoptions) { get; } | OCR 処理と認識されたテキストのインデックス作成のオプションを取得します。 |
| [TermHighlightEndTag](../../groupdocs.search.options/highlightoptions/termhighlightendtag) { get; set; } | 見つかった単語の強調表示の終了タグを取得します。 このタグは、プレーン テキストで強調表示する場合にのみ使用されます。 デフォルト値は空の文字列です。 |
| [TermHighlightStartTag](../../groupdocs.search.options/highlightoptions/termhighlightstarttag) { get; set; } | 見つかった単語の強調表示の開始タグを設定します。 このタグは、プレーン テキストで強調表示する場合にのみ使用されます。 デフォルト値は空の文字列です。 |
| [TermsAfter](../../groupdocs.search.options/highlightoptions/termsafter) { get; set; } | 強調表示された単語の後のテキスト フラグメント内の単語の最大数を取得または設定します。 値は 0 ～ 10000 の範囲内である必要があります。 デフォルト値は次のとおりです。`7`. |
| [TermsBefore](../../groupdocs.search.options/highlightoptions/termsbefore) { get; set; } | 強調表示された単語の前のテキスト フラグメント内の単語の最大数を取得または設定します。 値は 0 ～ 10000 の範囲内である必要があります。 デフォルト値は次のとおりです。`7`. |
| [TermsTotal](../../groupdocs.search.options/highlightoptions/termstotal) { get; set; } | テキスト フラグメント内の最大単語数を取得または設定します。 値は 0 ～ 10000 の範囲である必要があります。 デフォルト値は次のとおりです。`21`. |
| [UseInlineStyles](../../groupdocs.search.options/highlightoptions/useinlinestyles) { get; set; } | インライン スタイルを使用して出現箇所を強調表示するかどうかを示す値を取得または設定します。 デフォルト値は`真実`. |

### 備考

**もっと詳しく知る**

* [検索結果のハイライト](https://docs.groupdocs.com/display/searchnet/Highlighting+search+results)

### 関連項目

* class [TextOptions](../textoptions)
* 名前空間 [GroupDocs.Search.Options](../../groupdocs.search.options)
* 組み立て [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
