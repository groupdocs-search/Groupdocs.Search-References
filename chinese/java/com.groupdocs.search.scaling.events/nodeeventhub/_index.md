---
title: "NodeEventHub"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "提供用于订阅的节点事件。"
type: docs
weight: 16
url: /zh/java/com.groupdocs.search.scaling.events/nodeeventhub/
---
**Inheritance:**
java.lang.Object
```
public abstract class NodeEventHub
```

提供用于订阅的节点事件。

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [NodeEventHub()](#NodeEventHub--) |  |
## Fields

| Field | 描述 |
| --- | --- |
|  | [ConfigurationCompleted](#ConfigurationCompleted) | 当搜索网络配置过程完成时触发。 |
|
|  | [IndexingCompleted](#IndexingCompleted) | 当所有已排队文档的索引完成时触发。 |
|
|  | [DeletionCompleted](#DeletionCompleted) | 当所有已排队文档的删除完成时触发。 |
|
|  | [OptimizationCompleted](#OptimizationCompleted) | 当所有节点的优化完成时触发。 |
|
|  | [SynchronizationCompleted](#SynchronizationCompleted) | 当与所有节点的同步完成时触发。 |
|
|  | [AttributeChangesCompleted](#AttributeChangesCompleted) | 当所有已排队属性更改完成时触发。 |
|
|  | [StatusChanged](#StatusChanged) | 当搜索网络状态更改时触发。 |
|
|  | [DataExtracted](#DataExtracted) | 当从文档中提取数据时触发。 |
|
|  | [DocumentIndexed](#DocumentIndexed) | 当文档已被索引时触发。 |
|
|  | [DocumentDeleted](#DocumentDeleted) | 当文档已被删除时触发。 |
|
|  | [ErrorOccurred](#ErrorOccurred) | 当搜索网络的某个节点出现错误时触发。 |
|
|  | [IndexingProgressChanged](#IndexingProgressChanged) | 当索引操作的进度发生变化时触发。 |
|
|  | [OptimizationProgressChanged](#OptimizationProgressChanged) | 当优化操作的进度发生变化时触发。 |
|
### NodeEventHub() {#NodeEventHub--}
```
public NodeEventHub()
```


### ConfigurationCompleted {#ConfigurationCompleted}
```
public final Event<EventHandler> ConfigurationCompleted
```


当搜索网络配置过程完成时触发。


### IndexingCompleted {#IndexingCompleted}
```
public final Event<EventHandler> IndexingCompleted
```


当所有已排队文档的索引完成时触发。


### DeletionCompleted {#DeletionCompleted}
```
public final Event<EventHandler> DeletionCompleted
```


当所有已排队文档的删除完成时触发。


### OptimizationCompleted {#OptimizationCompleted}
```
public final Event<EventHandler> OptimizationCompleted
```


当所有节点的优化完成时触发。


### SynchronizationCompleted {#SynchronizationCompleted}
```
public final Event<EventHandler> SynchronizationCompleted
```


当与所有节点的同步完成时触发。


### AttributeChangesCompleted {#AttributeChangesCompleted}
```
public final Event<EventHandler> AttributeChangesCompleted
```


当所有已排队属性更改完成时触发。


### StatusChanged {#StatusChanged}
```
public final Event<EventHandler<StatusChangedEventArgs>> StatusChanged
```


当搜索网络状态更改时触发。


### DataExtracted {#DataExtracted}
```
public final Event<EventHandler<DataExtractedEventArgs>> DataExtracted
```


当从文档中提取数据时触发。


### DocumentIndexed {#DocumentIndexed}
```
public final Event<EventHandler<DocumentIndexedEventArgs>> DocumentIndexed
```


当文档已被索引时触发。


### DocumentDeleted {#DocumentDeleted}
```
public final Event<EventHandler<DocumentDeletedEventArgs>> DocumentDeleted
```


当文档已被删除时触发。


### ErrorOccurred {#ErrorOccurred}
```
public final Event<EventHandler<ErrorOccurredEventArgs>> ErrorOccurred
```


当搜索网络的某个节点出现错误时触发。


### IndexingProgressChanged {#IndexingProgressChanged}
```
public final Event<EventHandler<NetworkIndexingProgressEventArgs>> IndexingProgressChanged
```


当索引操作的进度发生变化时触发。


### OptimizationProgressChanged {#OptimizationProgressChanged}
```
public final Event<EventHandler<NetworkOptimizationProgressEventArgs>> OptimizationProgressChanged
```


当优化操作的进度发生变化时触发。


