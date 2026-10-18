---
title: "com.groupdocs.search.events"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "このパッケージは、イベント引数のクラスを提供します。"
type: docs
weight: 13
url: /ja/java/com.groupdocs.search.events/
---

このパッケージは、イベント引数のクラスを提供します。



## クラス

| クラス | 説明 |
| --- | --- |
| [BaseIndexEventArgs](../com.groupdocs.search.events/baseindexeventargs) | イベント引数の基底クラスを表します。 |
| [Event<T>](../com.groupdocs.search.events/event) | このクラスはイベントをサブスクライブする際に継承されることを意図しています。 |
| [EventHub](../com.groupdocs.search.events/eventhub) | サブスクライブ用のインデックスイベントを提供します。 |
| [EventHubBase](../com.groupdocs.search.events/eventhubbase) | イベントハブの基底抽象クラスです。 |
| [FileIndexingEventArgs](../com.groupdocs.search.events/fileindexingeventargs) | ドキュメントのインデックス作成開始イベントの引数を表します。 |
| [ImagePreparingEventArgs](../com.groupdocs.search.events/imagepreparingeventargs) | 画像の準備開始イベントの引数を表します。 |
| [IndexErrorEventArgs](../com.groupdocs.search.events/indexerroreventargs) | インデックスエラーが発生したイベントの引数を表します。 |
| [OperationFinishedEventArgs](../com.groupdocs.search.events/operationfinishedeventargs) | インデックス作成操作が完了したイベントの引数を表します。 |
| [OperationProgressEventArgs](../com.groupdocs.search.events/operationprogresseventargs) | インデックス作成操作の進行状況が更新されたイベントの引数を表します。 |
| [OptimizationProgressEventArgs](../com.groupdocs.search.events/optimizationprogresseventargs) | インデックス作成操作の進行状況が更新されたイベントの引数を表します。 |
| [PasswordRequiredEventArgs](../com.groupdocs.search.events/passwordrequiredeventargs) | パスワードで保護されたドキュメントがインデックス作成される際に発生するイベントの引数を表します。 |
| [SearchPhaseEventArgs](../com.groupdocs.search.events/searchphaseeventargs) | 検索フェーズ変更イベントの引数を表します。 |

## インターフェイス

| インターフェイス | 説明 |
| --- | --- |
| [EventHandler<T>](../com.groupdocs.search.events/eventhandler) | イベントハンドラのインターフェイスを定義します。 |

## 列挙型

| 列挙型 | 説明 |
| --- | --- |
| [OperationType](../com.groupdocs.search.events/operationtype) | インデックス操作の種類を表します。 |
| [SearchPhase](../com.groupdocs.search.events/searchphase) | 検索フェーズを表します。 |
