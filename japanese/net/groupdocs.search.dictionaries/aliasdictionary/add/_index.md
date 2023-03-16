---
title: Add
second_title: GroupDocs.Search for .NET API リファレンス
description: 指定されたエイリアスと関連付けられたテキストのペアをAliasDictionarygroupdocs.search.dictionaries/aliasdictionary.
type: docs
weight: 20
url: /ja/net/groupdocs.search.dictionaries/aliasdictionary/add/
---
## AliasDictionary.Add method

指定されたエイリアスと関連付けられたテキストのペアを、[`AliasDictionary`](../../aliasdictionary).

```csharp
public void Add(string alias, string text)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| alias | String | 辞書に追加するエイリアス。 |
| text | String | エイリアスに関連付けるテキスト。 |

### 例外

| 例外 | 調子 |
| --- | --- |
| ArgumentNullException | スローされるタイミング*alias*また*text*は`ヌル`. |
| ArgumentException | エイリアスに ab および 0-9 の範囲外の文字が含まれています。 |

### 関連項目

* class [AliasDictionary](../../aliasdictionary)
* 名前空間 [GroupDocs.Search.Dictionaries](../../aliasdictionary)
* 組み立て [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->