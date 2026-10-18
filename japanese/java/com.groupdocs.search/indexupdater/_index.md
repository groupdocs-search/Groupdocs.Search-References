---
title: "IndexUpdater"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "インデックスアップデータを表します。"
type: docs
weight: 20
url: /ja/java/com.groupdocs.search/indexupdater/
---
**Inheritance:**
java.lang.Object
```
public class IndexUpdater
```

インデックスアップデータを表します。このクラスは古いバージョンのインデックス内のドキュメントの再インデックス化を実行します。


**Learn more**

* [Update index](../https://docs.groupdocs.com/display/searchjava/Update+index)


この例はクラスの典型的な使用方法を示しています。

````
 ```

String sourceIndexFolder = "c:\\MyOldIndex\\";
String targetIndexFolder = "c:\\MyNewIndex\\";
IndexUpdater updater = new IndexUpdater();
if (updater.canUpdateVersion(sourceIndexFolder)) {
int result = updater.updateVersion(sourceIndexFolder, targetIndexFolder);
}
 
```
 
````


## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [IndexUpdater()](#IndexUpdater--) | IndexUpdater クラスの新しいインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [isLatestVersion(String indexPath)](#isLatestVersion-java.lang.String-) | 指定されたディレクトリに最新バージョンのインデックスが含まれているかどうかを確認します。 |
|
|  | [canUpdateVersion(String indexPath)](#canUpdateVersion-java.lang.String-) | 指定されたディレクトリ内のインデックスが最新バージョンに更新できるかどうかを確認します。 |
|
|  | [updateVersion(String indexPath, String newIndexPath)](#updateVersion-java.lang.String-java.lang.String-) | 古いバージョンのインデックス内のドキュメントを再インデックス化します。 |
|
### IndexUpdater() {#IndexUpdater--}
```
public IndexUpdater()
```


IndexUpdater クラスの新しいインスタンスを初期化します。


### isLatestVersion(String indexPath) {#isLatestVersion-java.lang.String-}
```
public final boolean isLatestVersion(String indexPath)
```


指定されたディレクトリに最新バージョンのインデックスが含まれているかどうかを確認します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | indexPath | java.lang.String | インデックスディレクトリのパスです。 |
|

**Returns:**
boolean - 指定されたディレクトリに最新バージョンのインデックスが含まれている場合は true、そうでない場合は false。

### canUpdateVersion(String indexPath) {#canUpdateVersion-java.lang.String-}
```
public final boolean canUpdateVersion(String indexPath)
```


指定されたディレクトリ内のインデックスが最新バージョンに更新できるかどうかを確認します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | indexPath | java.lang.String | インデックスディレクトリのパスです。 |
|

**Returns:**
boolean - 指定されたディレクトリ内のインデックスが最新バージョンに更新できる場合は true、そうでない場合は false。

### updateVersion(String indexPath, String newIndexPath) {#updateVersion-java.lang.String-java.lang.String-}
```
public final VersionUpdateResult updateVersion(String indexPath, String newIndexPath)
```


古いバージョンのインデックス内のドキュメントを再インデックス化します。更新されたインデックスは newIndexPath ディレクトリに配置され、indexPath ディレクトリ内のインデックスは変更されません。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | indexPath | java.lang.String | インデックスディレクトリのパスです。 |
|
|  | newIndexPath | java.lang.String | 更新されたインデックス用のディレクトリです。 |
|

**Returns:**
[VersionUpdateResult](../../com.groupdocs.search.common/versionupdateresult) - The result of the index version update operation.

