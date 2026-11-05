---
title: "NodeEventHub"
second_title: "GroupDocs.Search для Java API Reference"
description: "Предоставляет события узла для подписки."
type: docs
weight: 16
url: /ru/java/com.groupdocs.search.scaling.events/nodeeventhub/
---
**Inheritance:**
java.lang.Object
```
public abstract class NodeEventHub
```

Предоставляет события узла для подписки.

## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [NodeEventHub()](#NodeEventHub--) |  |
## Fields

| Field | Описание |
| --- | --- |
|  | [ConfigurationCompleted](#ConfigurationCompleted) | Происходит, когда процесс настройки поисковой сети завершён. |
|
|  | [IndexingCompleted](#IndexingCompleted) | Происходит, когда индексация всех поставленных в очередь документов завершена. |
|
|  | [DeletionCompleted](#DeletionCompleted) | Происходит, когда все поставленные в очередь удаления документов завершены. |
|
|  | [OptimizationCompleted](#OptimizationCompleted) | Происходит, когда оптимизация всех узлов завершена. |
|
|  | [SynchronizationCompleted](#SynchronizationCompleted) | Происходит, когда синхронизация со всеми узлами завершена. |
|
|  | [AttributeChangesCompleted](#AttributeChangesCompleted) | Происходит, когда все поставленные в очередь изменения атрибутов завершены. |
|
|  | [StatusChanged](#StatusChanged) | Происходит, когда статус поисковой сети изменяется. |
|
|  | [DataExtracted](#DataExtracted) | Происходит, когда данные извлечены из документа. |
|
|  | [DocumentIndexed](#DocumentIndexed) | Происходит, когда документ проиндексирован. |
|
|  | [DocumentDeleted](#DocumentDeleted) | Происходит, когда документ удалён. |
|
|  | [ErrorOccurred](#ErrorOccurred) | Происходит, когда в одном из узлов поисковой сети возникает ошибка. |
|
|  | [IndexingProgressChanged](#IndexingProgressChanged) | Происходит, когда прогресс операции индексации изменился. |
|
|  | [OptimizationProgressChanged](#OptimizationProgressChanged) | Происходит, когда прогресс операции оптимизации изменился. |
|
### NodeEventHub() {#NodeEventHub--}
```
public NodeEventHub()
```


### ConfigurationCompleted {#ConfigurationCompleted}
```
public final Event<EventHandler> ConfigurationCompleted
```


Происходит, когда процесс настройки поисковой сети завершён.


### IndexingCompleted {#IndexingCompleted}
```
public final Event<EventHandler> IndexingCompleted
```


Происходит, когда индексация всех поставленных в очередь документов завершена.


### DeletionCompleted {#DeletionCompleted}
```
public final Event<EventHandler> DeletionCompleted
```


Происходит, когда все поставленные в очередь удаления документов завершены.


### OptimizationCompleted {#OptimizationCompleted}
```
public final Event<EventHandler> OptimizationCompleted
```


Происходит, когда оптимизация всех узлов завершена.


### SynchronizationCompleted {#SynchronizationCompleted}
```
public final Event<EventHandler> SynchronizationCompleted
```


Происходит, когда синхронизация со всеми узлами завершена.


### AttributeChangesCompleted {#AttributeChangesCompleted}
```
public final Event<EventHandler> AttributeChangesCompleted
```


Происходит, когда все поставленные в очередь изменения атрибутов завершены.


### StatusChanged {#StatusChanged}
```
public final Event<EventHandler<StatusChangedEventArgs>> StatusChanged
```


Происходит, когда статус поисковой сети изменяется.


### DataExtracted {#DataExtracted}
```
public final Event<EventHandler<DataExtractedEventArgs>> DataExtracted
```


Происходит, когда данные извлечены из документа.


### DocumentIndexed {#DocumentIndexed}
```
public final Event<EventHandler<DocumentIndexedEventArgs>> DocumentIndexed
```


Происходит, когда документ проиндексирован.


### DocumentDeleted {#DocumentDeleted}
```
public final Event<EventHandler<DocumentDeletedEventArgs>> DocumentDeleted
```


Происходит, когда документ удалён.


### ErrorOccurred {#ErrorOccurred}
```
public final Event<EventHandler<ErrorOccurredEventArgs>> ErrorOccurred
```


Происходит, когда в одном из узлов поисковой сети возникает ошибка.


### IndexingProgressChanged {#IndexingProgressChanged}
```
public final Event<EventHandler<NetworkIndexingProgressEventArgs>> IndexingProgressChanged
```


Происходит, когда прогресс операции индексации изменился.


### OptimizationProgressChanged {#OptimizationProgressChanged}
```
public final Event<EventHandler<NetworkOptimizationProgressEventArgs>> OptimizationProgressChanged
```


Происходит, когда прогресс операции оптимизации изменился.


