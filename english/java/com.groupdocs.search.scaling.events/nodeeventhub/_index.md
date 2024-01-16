---
title: NodeEventHub
second_title: GroupDocs.Search for Java API Reference
description: Provides node events for subscribing.
type: docs
weight: 16
url: /java/com.groupdocs.search.scaling.events/nodeeventhub/
---
**Inheritance:**
java.lang.Object
```
public abstract class NodeEventHub
```

Provides node events for subscribing.
## Constructors

| Constructor | Description |
| --- | --- |
| [NodeEventHub()](#NodeEventHub--) |  |
## Fields

| Field | Description |
| --- | --- |
| [ConfigurationCompleted](#ConfigurationCompleted) | Occurs when the search network configuration process is finished. |
| [IndexingCompleted](#IndexingCompleted) | Occurs when indexing of all enqueued documents is finished. |
| [DeletionCompleted](#DeletionCompleted) | Occurs when all enqueued deletions of documents are finished. |
| [OptimizationCompleted](#OptimizationCompleted) | Occurs when optimization of all nodes is finished. |
| [SynchronizationCompleted](#SynchronizationCompleted) | Occurs when synchronization with all nodes is finished. |
| [AttributeChangesCompleted](#AttributeChangesCompleted) | Occurs when all enqueued attribute changes are finished. |
| [StatusChanged](#StatusChanged) | Occurs when the search network status changes. |
| [DataExtracted](#DataExtracted) | Occurs when the data has been extracted from a document. |
| [DocumentIndexed](#DocumentIndexed) | Occurs when a document has been indexed. |
| [DocumentDeleted](#DocumentDeleted) | Occurs when a document has been deleted. |
| [ErrorOccurred](#ErrorOccurred) | Occurs when an error occurs in one of the nodes of the search network. |
| [IndexingProgressChanged](#IndexingProgressChanged) | Occurs when the progress of the indexing operation has changed. |
| [OptimizationProgressChanged](#OptimizationProgressChanged) | Occurs when the progress of the optimization operation has changed. |
### NodeEventHub() {#NodeEventHub--}
```
public NodeEventHub()
```


### ConfigurationCompleted {#ConfigurationCompleted}
```
public final Event<EventHandler> ConfigurationCompleted
```


Occurs when the search network configuration process is finished.

### IndexingCompleted {#IndexingCompleted}
```
public final Event<EventHandler> IndexingCompleted
```


Occurs when indexing of all enqueued documents is finished.

### DeletionCompleted {#DeletionCompleted}
```
public final Event<EventHandler> DeletionCompleted
```


Occurs when all enqueued deletions of documents are finished.

### OptimizationCompleted {#OptimizationCompleted}
```
public final Event<EventHandler> OptimizationCompleted
```


Occurs when optimization of all nodes is finished.

### SynchronizationCompleted {#SynchronizationCompleted}
```
public final Event<EventHandler> SynchronizationCompleted
```


Occurs when synchronization with all nodes is finished.

### AttributeChangesCompleted {#AttributeChangesCompleted}
```
public final Event<EventHandler> AttributeChangesCompleted
```


Occurs when all enqueued attribute changes are finished.

### StatusChanged {#StatusChanged}
```
public final Event<EventHandler<StatusChangedEventArgs>> StatusChanged
```


Occurs when the search network status changes.

### DataExtracted {#DataExtracted}
```
public final Event<EventHandler<DataExtractedEventArgs>> DataExtracted
```


Occurs when the data has been extracted from a document.

### DocumentIndexed {#DocumentIndexed}
```
public final Event<EventHandler<DocumentIndexedEventArgs>> DocumentIndexed
```


Occurs when a document has been indexed.

### DocumentDeleted {#DocumentDeleted}
```
public final Event<EventHandler<DocumentDeletedEventArgs>> DocumentDeleted
```


Occurs when a document has been deleted.

### ErrorOccurred {#ErrorOccurred}
```
public final Event<EventHandler<ErrorOccurredEventArgs>> ErrorOccurred
```


Occurs when an error occurs in one of the nodes of the search network.

### IndexingProgressChanged {#IndexingProgressChanged}
```
public final Event<EventHandler<NetworkIndexingProgressEventArgs>> IndexingProgressChanged
```


Occurs when the progress of the indexing operation has changed.

### OptimizationProgressChanged {#OptimizationProgressChanged}
```
public final Event<EventHandler<NetworkOptimizationProgressEventArgs>> OptimizationProgressChanged
```


Occurs when the progress of the optimization operation has changed.

