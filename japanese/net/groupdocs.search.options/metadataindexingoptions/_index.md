---
title: MetadataIndexingOptions
second_title: GroupDocs.Search for .NET API リファレンス
description: メタデータ フィールドのインデックス作成のオプションを提供します
type: docs
weight: 970
url: /ja/net/groupdocs.search.options/metadataindexingoptions/
---
## MetadataIndexingOptions class

メタデータ フィールドのインデックス作成のオプションを提供します。

```csharp
public class MetadataIndexingOptions
```

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [DefaultFieldName](../../groupdocs.search.options/metadataindexingoptions/defaultfieldname) { get; set; } | 空のフィールド名のインデックスに使用されるデフォルトのフィールド名を取得または設定します。 デフォルト値は`"知らない"`. |
| [IndexingEmptyNames](../../groupdocs.search.options/metadataindexingoptions/indexingemptynames) { get; set; } | 空のフィールド名をインデックス化するかどうかを示す値を取得または設定します。 デフォルト値は`真実`. |
| [IndexingEmptyValues](../../groupdocs.search.options/metadataindexingoptions/indexingemptyvalues) { get; set; } | 空のフィールド値にインデックスを付けるかどうかを示す値を取得または設定します。 デフォルト値は`真実`. |
| [MaxBytesToIndexField](../../groupdocs.search.options/metadataindexingoptions/maxbytestoindexfield) { get; set; } | フィールドにインデックスを付けるためにバイト型の配列内の値の最大数を取得または設定します。 デフォルト値は`int.MaxValue`. |
| [MaxDoublesToIndexField](../../groupdocs.search.options/metadataindexingoptions/maxdoublestoindexfield) { get; set; } | フィールドにインデックスを付けるために double 型の配列内の値の最大数を取得または設定します。 デフォルト値は`int.MaxValue`. |
| [MaxIntsToIndexField](../../groupdocs.search.options/metadataindexingoptions/maxintstoindexfield) { get; set; } | int 型の配列内の値の最大数を取得または設定して、フィールドにインデックスを付けます。 デフォルト値は`int.MaxValue`. |
| [MaxLongsToIndexField](../../groupdocs.search.options/metadataindexingoptions/maxlongstoindexfield) { get; set; } | フィールドにインデックスを付けるために long 型の配列内の値の最大数を取得または設定します。 デフォルト値は`int.MaxValue`. |
| [SeparatorBetweenValues](../../groupdocs.search.options/metadataindexingoptions/separatorbetweenvalues) { get; set; } | 配列型のフィールドの値の間のセパレータを取得または設定します. デフォルト値はスペース記号です. |
| [SeparatorInCompoundName](../../groupdocs.search.options/metadataindexingoptions/separatorincompoundname) { get; set; } | フィールドの複合名のセパレーターを取得または設定します。 デフォルト値は`「。」`. |

### 備考

**もっと詳しく知る**

* [索引付けオプション](https://docs.groupdocs.com/display/searchnet/Indexing+options)
* MetadataIndexingOptions は、インデックスからドキュメント テキストを取得するときに使用されます: [インデックス付きドキュメントの取得](https://docs.groupdocs.com/display/searchnet/Getting+indexed+documents)
* MetadataIndexingOptions は、検索結果を強調表示するときに使用されます: [検索結果のハイライト](https://docs.groupdocs.com/display/searchnet/Highlighting+search+results)

### 関連項目

* 名前空間 [GroupDocs.Search.Options](../../groupdocs.search.options)
* 組み立て [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->