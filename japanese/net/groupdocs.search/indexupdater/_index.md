---
title: IndexUpdater
second_title: GroupDocs.Search for .NET API リファレンス
description: インデックス アップデーターを表します このクラスは古いバージョンのインデックスでドキュメントの再インデックスを実行します
type: docs
weight: 710
url: /ja/net/groupdocs.search/indexupdater/
---
## IndexUpdater class

インデックス アップデーターを表します。 このクラスは、古いバージョンのインデックスでドキュメントの再インデックスを実行します。

```csharp
public class IndexUpdater
```

## コンストラクター

| 名前 | 説明 |
| --- | --- |
| [IndexUpdater](indexupdater)() | の新しいインスタンスを初期化します[`IndexUpdater`](../indexupdater)class. |

## メソッド

| 名前 | 説明 |
| --- | --- |
| [CanUpdateVersion](../../groupdocs.search/indexupdater/canupdateversion)(string) | 指定したディレクトリ内のインデックスを最新バージョンに更新できるかどうかを確認します。 |
| [IsLatestVersion](../../groupdocs.search/indexupdater/islatestversion)(string) | 指定したディレクトリに最新バージョンのインデックスが含まれているかどうかを確認します。 |
| [UpdateVersion](../../groupdocs.search/indexupdater/updateversion)(string, string) | 古いバージョンのインデックスでドキュメントの再インデックスを実行します。 更新されたインデックスは*newIndexPath*directory. のインデックス*indexPath*ディレクトリは変更されません. |

### 備考

**もっと詳しく知る**

* [インデックスを更新](https://docs.groupdocs.com/display/searchnet/Update+index)

### 例

この例は、クラスの典型的な使用法を示しています.

```csharp
string sourceIndexFolder = @"c:\MyOldIndex\";
string targetIndexFolder = @"c:\MyNewIndex\";

IndexUpdater updater = new IndexUpdater();

if (updater.CanUpdateVersion(sourceIndexFolder))
{
    VersionUpdateResult result = updater.UpdateVersion(sourceIndexFolder, targetIndexFolder);
}
```

### 関連項目

* 名前空間 [GroupDocs.Search](../../groupdocs.search)
* 組み立て [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->