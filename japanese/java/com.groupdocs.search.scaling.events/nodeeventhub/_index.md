---
title: "NodeEventHub"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "サブスクライブ用のノードイベントを提供します。"
type: docs
weight: 16
url: /ja/java/com.groupdocs.search.scaling.events/nodeeventhub/
---
**Inheritance:**
java.lang.Object
```
public abstract class NodeEventHub
```

サブスクライブ用のノードイベントを提供します。

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [NodeEventHub()](#NodeEventHub--) |  |
## Fields

| Field | 説明 |
| --- | --- |
|  | [ConfigurationCompleted](#ConfigurationCompleted) | 検索ネットワーク構成プロセスが完了したときに発生します。 |
|
|  | [IndexingCompleted](#IndexingCompleted) | キューに入れられたすべてのドキュメントのインデックス作成が完了したときに発生します。 |
|
|  | [DeletionCompleted](#DeletionCompleted) | ドキュメントのすべてのキューイングされた削除が完了したときに発生します。 |
|
|  | [OptimizationCompleted](#OptimizationCompleted) | すべてのノードの最適化が完了したときに発生します。 |
|
|  | [SynchronizationCompleted](#SynchronizationCompleted) | すべてのノードとの同期が完了したときに発生します。 |
|
|  | [AttributeChangesCompleted](#AttributeChangesCompleted) | すべてのキューイングされた属性変更が完了したときに発生します。 |
|
|  | [StatusChanged](#StatusChanged) | 検索ネットワークのステータスが変更されたときに発生します。 |
|
|  | [DataExtracted](#DataExtracted) | ドキュメントからデータが抽出されたときに発生します。 |
|
|  | [DocumentIndexed](#DocumentIndexed) | ドキュメントがインデックス化されたときに発生します。 |
|
|  | [DocumentDeleted](#DocumentDeleted) | ドキュメントが削除されたときに発生します。 |
|
|  | [ErrorOccurred](#ErrorOccurred) | 検索ネットワークのノードの一つでエラーが発生したときに発生します。 |
|
|  | [IndexingProgressChanged](#IndexingProgressChanged) | インデックス作業の進捗が変更されたときに発生します。 |
|
|  | [OptimizationProgressChanged](#OptimizationProgressChanged) | 最適化作業の進捗が変更されたときに発生します。 |
|
### NodeEventHub() {#NodeEventHub--}
```
public NodeEventHub()
```


### ConfigurationCompleted {#ConfigurationCompleted}
```
public final Event<EventHandler> ConfigurationCompleted
```


検索ネットワーク構成プロセスが完了したときに発生します。


### IndexingCompleted {#IndexingCompleted}
```
public final Event<EventHandler> IndexingCompleted
```


キューに入れられたすべてのドキュメントのインデックス作成が完了したときに発生します。


### DeletionCompleted {#DeletionCompleted}
```
public final Event<EventHandler> DeletionCompleted
```


ドキュメントのすべてのキューイングされた削除が完了したときに発生します。


### OptimizationCompleted {#OptimizationCompleted}
```
public final Event<EventHandler> OptimizationCompleted
```


すべてのノードの最適化が完了したときに発生します。


### SynchronizationCompleted {#SynchronizationCompleted}
```
public final Event<EventHandler> SynchronizationCompleted
```


すべてのノードとの同期が完了したときに発生します。


### AttributeChangesCompleted {#AttributeChangesCompleted}
```
public final Event<EventHandler> AttributeChangesCompleted
```


すべてのキューイングされた属性変更が完了したときに発生します。


### StatusChanged {#StatusChanged}
```
public final Event<EventHandler<StatusChangedEventArgs>> StatusChanged
```


検索ネットワークのステータスが変更されたときに発生します。


### DataExtracted {#DataExtracted}
```
public final Event<EventHandler<DataExtractedEventArgs>> DataExtracted
```


ドキュメントからデータが抽出されたときに発生します。


### DocumentIndexed {#DocumentIndexed}
```
public final Event<EventHandler<DocumentIndexedEventArgs>> DocumentIndexed
```


ドキュメントがインデックス化されたときに発生します。


### DocumentDeleted {#DocumentDeleted}
```
public final Event<EventHandler<DocumentDeletedEventArgs>> DocumentDeleted
```


ドキュメントが削除されたときに発生します。


### ErrorOccurred {#ErrorOccurred}
```
public final Event<EventHandler<ErrorOccurredEventArgs>> ErrorOccurred
```


検索ネットワークのノードの一つでエラーが発生したときに発生します。


### IndexingProgressChanged {#IndexingProgressChanged}
```
public final Event<EventHandler<NetworkIndexingProgressEventArgs>> IndexingProgressChanged
```


インデックス作業の進捗が変更されたときに発生します。


### OptimizationProgressChanged {#OptimizationProgressChanged}
```
public final Event<EventHandler<NetworkOptimizationProgressEventArgs>> OptimizationProgressChanged
```


最適化作業の進捗が変更されたときに発生します。


