---
title: IDocumentLoader
second_title: GroupDocs.Search for .NET API リファレンス
description: 遅延ドキュメントをロードするために使用されるドキュメント ローダー インターフェイスを定義します
type: docs
weight: 180
url: /ja/net/groupdocs.search.common/idocumentloader/
---
## IDocumentLoader interface

遅延ドキュメントをロードするために使用されるドキュメント ローダー インターフェイスを定義します。

```csharp
public interface IDocumentLoader
```

## メソッド

| 名前 | 説明 |
| --- | --- |
| [CloseDocument](../../groupdocs.search.common/idocumentloader/closedocument)() | ロードされたドキュメントを閉じます。 このメソッドは、ドキュメントの処理が終了したときにインデックスによって呼び出されます。 |
| [LoadDocument](../../groupdocs.search.common/idocumentloader/loaddocument)() | ドキュメントをロードします。 このメソッドは、ドキュメントを処理する準備ができたときにインデックスによって呼び出されます。 |

### 関連項目

* 名前空間 [GroupDocs.Search.Common](../../groupdocs.search.common)
* 組み立て [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
