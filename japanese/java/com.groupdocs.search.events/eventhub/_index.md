---
title: "EventHub"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "サブスクライブ用のインデックスイベントを提供します。"
type: docs
weight: 12
url: /ja/java/com.groupdocs.search.events/eventhub/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventHubBase](../../com.groupdocs.search.events/eventhubbase)
```
public abstract class EventHub extends EventHubBase
```

サブスクライブ用のインデックスイベントを提供します。


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)


この例はクラスの典型的な使用方法を示しています。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
// インデックスを作成
Index index = new Index(indexFolder);
// イベントへのサブスクライブ
index.getEvents().ErrorOccurred.add(new EventHandler() {
public void invoke(Object sender, IndexErrorEventArgs args) {
System.out.println(args.getMessage());
}
});
// 指定されたフォルダーからドキュメントをインデックス化
index.add(documentsFolder);
// インデックスを検索
SearchResult result = index.search(query);
 
```
 
````


## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [EventHub()](#EventHub--) |  |
## Fields

| Field | 説明 |
| --- | --- |
|  | [OperationFinished](#OperationFinished) | インデックス操作が完了したときに発生します。 |
|
|  | [ErrorOccurred](#ErrorOccurred) | インデックス操作中にエラーが発生したときに発生します。 |
|
|  | [OperationProgressChanged](#OperationProgressChanged) | インデックス作成または更新操作の進行状況が変化したときに発生します。 |
|
|  | [OptimizationProgressChanged](#OptimizationProgressChanged) | 最適化操作の進行状況が変化したときに発生します。 |
|
|  | [PasswordRequired](#PasswordRequired) | document が開く際にパスワードが必要なときに発生します。 |
|
|  | [FileIndexing](#FileIndexing) | ドキュメントがインデックスに追加されるときに発生します。 |
|
|  | [ImagePreparing](#ImagePreparing) | image がインデックス作成のために準備されるときに発生します。 |
|
|  | [StatusChanged](#StatusChanged) | インデックスのステータスが変化したときに発生します。 |
|
|  | [SearchPhaseCompleted](#SearchPhaseCompleted) | 検索フェーズが完了したときに発生します。 |
|
### EventHub() {#EventHub--}
```
public EventHub()
```


### OperationFinished {#OperationFinished}
```
public final Event<EventHandler<OperationFinishedEventArgs>> OperationFinished
```


インデックス操作が完了したときに発生します。

この例はイベントの使用方法を示しています。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// インデックスを作成
Index index = new Index(indexFolder);
// イベントへのサブスクライブ
index.getEvents().OperationFinished.add(new EventHandler() {
public void invoke(Object sender, OperationFinishedEventArgs args) {
System.out.println("Operation finished: " + args.getOperationType());
System.out.println("Message: " + args.getMessage());
System.out.println("Index folder: " + args.getIndexFolder());
DateFormat df = new SimpleDateFormat("MM/dd/yyyy HH:mm:ss");
System.out.println("Time: " + df.format(args.getTime()));
}
});
// 指定されたフォルダーからドキュメントをインデックス化
index.add(documentsFolder);
 
```
 
````



### ErrorOccurred {#ErrorOccurred}
```
public final Event<EventHandler<IndexErrorEventArgs>> ErrorOccurred
```


インデックス操作中にエラーが発生したときに発生します。

この例はイベントの使用方法を示しています。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
// インデックスを作成
Index index = new Index(indexFolder);
// イベントへのサブスクライブ
index.getEvents().ErrorOccurred.add(new EventHandler() {
public void invoke(Object sender, IndexErrorEventArgs args) {
System.out.println(args.getMessage());
}
});
// 指定されたフォルダーからドキュメントをインデックス化
index.add(documentsFolder);
// インデックスを検索
SearchResult result = index.search(query);
 
```
 
````



### OperationProgressChanged {#OperationProgressChanged}
```
public final Event<EventHandler<OperationProgressEventArgs>> OperationProgressChanged
```


インデックス作成または更新操作の進行状況が変化したときに発生します。

この例はイベントの使用方法を示しています。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// インデックスを作成
Index index = new Index(indexFolder);
// イベントへのサブスクライブ
index.getEvents().OperationProgressChanged.add(new EventHandler() {
public void invoke(Object sender, OperationProgressEventArgs args) {
System.out.println("Last processed: " + args.getLastDocumentPath());
System.out.println("結果: " + args.getLastDocumentStatus());
System.out.println("処理されたドキュメント: " + args.getTotalDocuments());
System.out.println("進捗率: " + args.getProgressPercentage());
}
});
// 指定されたフォルダーからドキュメントをインデックス化
index.add(documentsFolder);
 
```
 
````



### OptimizationProgressChanged {#OptimizationProgressChanged}
```
public final Event<EventHandler<OptimizationProgressEventArgs>> OptimizationProgressChanged
```


最適化操作の進行状況が変化したときに発生します。


### PasswordRequired {#PasswordRequired}
```
public final Event<EventHandler<PasswordRequiredEventArgs>> PasswordRequired
```


document が開く際にパスワードが必要なときに発生します。

この例はイベントの使用方法を示しています。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// インデックスを作成
Index index = new Index(indexFolder);
// イベントへのサブスクライブ
index.getEvents().PasswordRequired.add(new EventHandler() {
public void invoke(Object sender, PasswordRequiredEventArgs args) {
if (args.getDocumentFullPath().endsWith("ProtectedDocument.pdf")) {
args.setPassword("123456");
}
}
});
// 指定されたフォルダーからドキュメントをインデックス化
index.add(documentsFolder);
 
```
 
````



### FileIndexing {#FileIndexing}
```
public final Event<EventHandler<FileIndexingEventArgs>> FileIndexing
```


ドキュメントがインデックスに追加されるときに発生します。

この例はイベントの使用方法を示しています。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// インデックスを作成
Index index = new Index(indexFolder);
// イベントへのサブスクライブ
index.getEvents().FileIndexing.add(new EventHandler() {
public void invoke(Object sender, FileIndexingEventArgs args) {
if (args.getDocumentFullPath().endsWith("Protected.pdf")) {
args.setAdditionalFields(new DocumentField[] {
new DocumentField("Tags", "Protected")
});
}
if (!args.getDocumentFullPath().toLowerCase().contains("重要")) {
args.setSkipIndexing(true);
}
}
});
// 指定されたフォルダーからドキュメントをインデックス化
index.add(documentsFolder);
 
```
 
````



### ImagePreparing {#ImagePreparing}
```
public final Event<EventHandler<ImagePreparingEventArgs>> ImagePreparing
```


image がインデックス作成のために準備されるときに発生します。


### StatusChanged {#StatusChanged}
```
public final Event<EventHandler<BaseIndexEventArgs>> StatusChanged
```


インデックスのステータスが変化したときに発生します。

この例はイベントの使用方法を示しています。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// インデックスを作成
Index index = new Index(indexFolder);
// イベントへのサブスクライブ
index.getEvents().StatusChanged.add(new EventHandler() {
public void invoke(Object sender, BaseIndexEventArgs args) {
if (args.getStatus() != IndexStatus.InProgress) {
// 操作完了の通知はここにあるはずです
}
}
});
// 非同期インデックス作成のフラグを設定する
IndexingOptions options = new IndexingOptions();
options.setAsync(true);
// 指定されたフォルダーからドキュメントを非同期でインデックス作成
// 操作が完了する前にメソッドが終了します
index.add(documentsFolder, options);
 
```
 
````



### SearchPhaseCompleted {#SearchPhaseCompleted}
```
public final Event<EventHandler<SearchPhaseEventArgs>> SearchPhaseCompleted
```


検索フェーズが完了したときに発生します。

この例はイベントの使用方法を示しています。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// インデックスを作成
Index index = new Index(indexFolder);
// 指定されたフォルダーからドキュメントをインデックス化
index.add(documentsFolder);
// イベントへのサブスクライブ
index.getEvents().SearchPhaseCompleted.add(new EventHandler() {
public void invoke(Object sender, SearchPhaseEventArgs args) {
System.out.println("検索フェーズ: " + args.getSearchPhase());
System.out.println("単語数: " + args.getWords().length);
}
});
SearchOptions options = new SearchOptions();
options.setUseSynonymSearch(true);
options.setUseWordFormsSearch(true);
options.getFuzzySearch().setEnabled(true);
options.setUseHomophoneSearch(true);
SearchResult result = index.search("Einstein", options);
 
```
 
````



