---
title: "com.groupdocs.search"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "このパッケージは、さまざまな形式のドキュメント内のテキストデータをインデックス作成および検索するためのクラスを提供します。"
type: docs
weight: 10
url: /ja/java/com.groupdocs.search/
---

このパッケージは、さまざまな形式のドキュメント内のテキストデータをインデックス作成および検索するためのクラスを提供します。このパッケージの主なクラスは次のとおりです:

Index は、インデックス作成および検索操作のエントリーポイントです。

SearchQuery は、オブジェクト形式のすべての検索クエリタイプの基底クラスおよびファクトリです。

IndexRepository は、複数のインデックスを結合し、それらに対して共通操作を実行するためのコンテナクラスです。



## クラス

| クラス | 説明 |
| --- | --- |
| [Action](../com.groupdocs.search/action) | パラメーターを持たず、戻り値もないメソッドをカプセル化します。 |
| [Action1<T>](../com.groupdocs.search/action1) | 単一のパラメータを持ち、戻り値を返さないメソッドをカプセル化します。 |
| [Action2<T1,T2>](../com.groupdocs.search/action2) | 2つのパラメータを持ち、戻り値を返さないメソッドをカプセル化します。 |
| [Document](../com.groupdocs.search/document) | ファイルシステム、ストリーム、または構造からインデックスに追加されるドキュメントの基底クラスを表します。 |
| [DocumentFilter](../com.groupdocs.search/documentfilter) | ドキュメントフィルタの基底クラスを表します。 |
| [ExtractedData](../com.groupdocs.search/extracteddata) | ドキュメントから取得され、インデックス作成のために準備されたデータを表します。 |
| [Extractor](../com.groupdocs.search/extractor) | 後続の高速インデックス作成段階を分離するために、ドキュメントからの事前データ抽出ツールを表します。 |
| [Index](../com.groupdocs.search/index) | ドキュメントのインデックス作成と検索を行うメインクラスを表します。 |
| [IndexRepository](../com.groupdocs.search/indexrepository) | 複数のインデックスを結合し、共通の操作を実行するためのコンテナを表します。 |
| [IndexSettings](../com.groupdocs.search/indexsettings) | インデックス作成操作をカスタマイズできるインデックス設定を表します。 |
| [IndexUpdater](../com.groupdocs.search/indexupdater) | インデックスアップデータを表します。 |
| [LicenseRestrictionException](../com.groupdocs.search/licenserestrictionexception) | ライセンス制限がトリガーされたときにスローされる例外です。 |
| [Notification](../com.groupdocs.search/notification) | インデックスへのすべての通知の基底クラスです。 |
| [PleaseReportException](../com.groupdocs.search/pleasereportexception) | ライブラリでエラーが発生したときにスローされる例外を表します。 |
| [SearchDocumentFilter](../com.groupdocs.search/searchdocumentfilter) | 検索ドキュメントフィルタを作成するメソッドを含みます。 |
| [SearchQuery](../com.groupdocs.search/searchquery) | オブジェクト形式の検索クエリを表します。 |
