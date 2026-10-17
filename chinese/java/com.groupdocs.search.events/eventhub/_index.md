---
title: "EventHub"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "提供用于订阅的索引事件。"
type: docs
weight: 12
url: /zh/java/com.groupdocs.search.events/eventhub/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventHubBase](../../com.groupdocs.search.events/eventhubbase)
```
public abstract class EventHub extends EventHubBase
```

提供用于订阅的索引事件。


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)


此示例演示了该类的典型用法。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
// 创建索引
Index index = new Index(indexFolder);
// 订阅事件
index.getEvents().ErrorOccurred.add(new EventHandler() {
public void invoke(Object sender, IndexErrorEventArgs args) {
System.out.println(args.getMessage());
}
});
// 索引来自指定文件夹的文档
index.add(documentsFolder);
// 在索引中搜索
SearchResult result = index.search(query);
 
```
 
````


## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [EventHub()](#EventHub--) |  |
## Fields

| Field | 描述 |
| --- | --- |
|  | [OperationFinished](#OperationFinished) | 当索引操作完成时发生。 |
|
|  | [ErrorOccurred](#ErrorOccurred) | 当索引操作期间发生错误时发生。 |
|
|  | [OperationProgressChanged](#OperationProgressChanged) | 当索引或更新操作的进度变化时发生。 |
|
|  | [OptimizationProgressChanged](#OptimizationProgressChanged) | 当优化操作的进度变化时发生。 |
|
|  | [PasswordRequired](#PasswordRequired) | 在文档打开需要密码时出现。 |
|
|  | [FileIndexing](#FileIndexing) | 当文档即将被索引时发生。 |
|
|  | [ImagePreparing](#ImagePreparing) | 在准备图像进行索引时出现。 |
|
|  | [StatusChanged](#StatusChanged) | 当索引状态变化时发生。 |
|
|  | [SearchPhaseCompleted](#SearchPhaseCompleted) | 当搜索阶段完成时发生。 |
|
### EventHub() {#EventHub--}
```
public EventHub()
```


### OperationFinished {#OperationFinished}
```
public final Event<EventHandler<OperationFinishedEventArgs>> OperationFinished
```


当索引操作完成时发生。

示例演示如何使用该事件。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// 创建索引
Index index = new Index(indexFolder);
// 订阅事件
index.getEvents().OperationFinished.add(new EventHandler() {
public void invoke(Object sender, OperationFinishedEventArgs args) {
System.out.println("Operation finished: " + args.getOperationType());
System.out.println("消息: " + args.getMessage());
System.out.println("索引文件夹: " + args.getIndexFolder());
DateFormat df = new SimpleDateFormat("MM/dd/yyyy HH:mm:ss");
System.out.println("时间: " + df.format(args.getTime()));
}
});
// 索引来自指定文件夹的文档
index.add(documentsFolder);
 
```
 
````



### ErrorOccurred {#ErrorOccurred}
```
public final Event<EventHandler<IndexErrorEventArgs>> ErrorOccurred
```


当索引操作期间发生错误时发生。

示例演示如何使用该事件。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
// 创建索引
Index index = new Index(indexFolder);
// 订阅事件
index.getEvents().ErrorOccurred.add(new EventHandler() {
public void invoke(Object sender, IndexErrorEventArgs args) {
System.out.println(args.getMessage());
}
});
// 索引来自指定文件夹的文档
index.add(documentsFolder);
// 在索引中搜索
SearchResult result = index.search(query);
 
```
 
````



### OperationProgressChanged {#OperationProgressChanged}
```
public final Event<EventHandler<OperationProgressEventArgs>> OperationProgressChanged
```


当索引或更新操作的进度变化时发生。

示例演示如何使用该事件。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// 创建索引
Index index = new Index(indexFolder);
// 订阅事件
index.getEvents().OperationProgressChanged.add(new EventHandler() {
public void invoke(Object sender, OperationProgressEventArgs args) {
System.out.println("上次处理: " + args.getLastDocumentPath());
System.out.println("结果: " + args.getLastDocumentStatus());
System.out.println("已处理文档: " + args.getTotalDocuments());
System.out.println("进度百分比: " + args.getProgressPercentage());
}
});
// 索引来自指定文件夹的文档
index.add(documentsFolder);
 
```
 
````



### OptimizationProgressChanged {#OptimizationProgressChanged}
```
public final Event<EventHandler<OptimizationProgressEventArgs>> OptimizationProgressChanged
```


当优化操作的进度变化时发生。


### PasswordRequired {#PasswordRequired}
```
public final Event<EventHandler<PasswordRequiredEventArgs>> PasswordRequired
```


在文档打开需要密码时出现。

示例演示如何使用该事件。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// 创建索引
Index index = new Index(indexFolder);
// 订阅事件
index.getEvents().PasswordRequired.add(new EventHandler() {
public void invoke(Object sender, PasswordRequiredEventArgs args) {
if (args.getDocumentFullPath().endsWith("ProtectedDocument.pdf")) {
args.setPassword("123456");
}
}
});
// 索引来自指定文件夹的文档
index.add(documentsFolder);
 
```
 
````



### FileIndexing {#FileIndexing}
```
public final Event<EventHandler<FileIndexingEventArgs>> FileIndexing
```


当文档即将被索引时发生。

示例演示如何使用该事件。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// 创建索引
Index index = new Index(indexFolder);
// 订阅事件
index.getEvents().FileIndexing.add(new EventHandler() {
public void invoke(Object sender, FileIndexingEventArgs args) {
if (args.getDocumentFullPath().endsWith("Protected.pdf")) {
args.setAdditionalFields(new DocumentField[] {
new DocumentField("标签", "受保护")
});
}
if (!args.getDocumentFullPath().toLowerCase().contains("重要")) {
args.setSkipIndexing(true);
}
}
});
// 索引来自指定文件夹的文档
index.add(documentsFolder);
 
```
 
````



### ImagePreparing {#ImagePreparing}
```
public final Event<EventHandler<ImagePreparingEventArgs>> ImagePreparing
```


在准备图像进行索引时出现。


### StatusChanged {#StatusChanged}
```
public final Event<EventHandler<BaseIndexEventArgs>> StatusChanged
```


当索引状态变化时发生。

示例演示如何使用该事件。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// 创建索引
Index index = new Index(indexFolder);
// 订阅事件
index.getEvents().StatusChanged.add(new EventHandler() {
public void invoke(Object sender, BaseIndexEventArgs args) {
if (args.getStatus() != IndexStatus.InProgress) {
// 应在此处放置操作完成的通知
}
}
});
// 设置异步索引的标志
IndexingOptions options = new IndexingOptions();
options.setAsync(true);
// 异步索引指定文件夹中的文档
// 方法在操作完成前终止
index.add(documentsFolder, options);
 
```
 
````



### SearchPhaseCompleted {#SearchPhaseCompleted}
```
public final Event<EventHandler<SearchPhaseEventArgs>> SearchPhaseCompleted
```


当搜索阶段完成时发生。

示例演示如何使用该事件。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// 创建索引
Index index = new Index(indexFolder);
// 索引来自指定文件夹的文档
index.add(documentsFolder);
// 订阅事件
index.getEvents().SearchPhaseCompleted.add(new EventHandler() {
public void invoke(Object sender, SearchPhaseEventArgs args) {
System.out.println("Search phase: " + args.getSearchPhase());
System.out.println("Words: " + args.getWords().length);
}
});
SearchOptions options = new SearchOptions();
options.setUseSynonymSearch(true);
options.setUseWordFormsSearch(true);
options.getFuzzySearch().setEnabled(true);
options.setUseHomophoneSearch(true);
SearchResult result = index.search(\"Einstein\", options);
 
```
 
````



