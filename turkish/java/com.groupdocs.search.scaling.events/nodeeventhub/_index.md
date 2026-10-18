---
title: "NodeEventHub"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Abonelik için düğüm olayları sağlar."
type: docs
weight: 16
url: /tr/java/com.groupdocs.search.scaling.events/nodeeventhub/
---
**Inheritance:**
java.lang.Object
```
public abstract class NodeEventHub
```

Abonelik için düğüm olayları sağlar.

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [NodeEventHub()](#NodeEventHub--) |  |
## Alanlar

| Alan | Açıklama |
| --- | --- |
|  | [ConfigurationCompleted](#ConfigurationCompleted) | Arama ağı yapılandırma süreci tamamlandığında gerçekleşir. |
|
|  | [IndexingCompleted](#IndexingCompleted) | Kuyruğa alınan tüm belgelerin indekslemesi tamamlandığında gerçekleşir. |
|
|  | [DeletionCompleted](#DeletionCompleted) | Tüm kuyruğa alınmış belge silme işlemleri tamamlandığında oluşur. |
|
|  | [OptimizationCompleted](#OptimizationCompleted) | Tüm düğümlerin optimizasyonu tamamlandığında oluşur. |
|
|  | [SynchronizationCompleted](#SynchronizationCompleted) | Tüm düğümlerle senkronizasyon tamamlandığında oluşur. |
|
|  | [AttributeChangesCompleted](#AttributeChangesCompleted) | Tüm kuyruğa alınmış öznitelik değişiklikleri tamamlandığında oluşur. |
|
|  | [StatusChanged](#StatusChanged) | Arama ağı durumu değiştiğinde oluşur. |
|
|  | [DataExtracted](#DataExtracted) | Veri bir belgeden çıkarıldığında oluşur. |
|
|  | [DocumentIndexed](#DocumentIndexed) | Bir belge indekslendiğinde oluşur. |
|
|  | [DocumentDeleted](#DocumentDeleted) | Bir belge silindiğinde oluşur. |
|
|  | [ErrorOccurred](#ErrorOccurred) | Arama ağının bir düğümünde bir hata oluştuğunda oluşur. |
|
|  | [IndexingProgressChanged](#IndexingProgressChanged) | İndeksleme işleminin ilerlemesi değiştiğinde oluşur. |
|
|  | [OptimizationProgressChanged](#OptimizationProgressChanged) | Optimizasyon işleminin ilerlemesi değiştiğinde oluşur. |
|
### NodeEventHub() {#NodeEventHub--}
```
public NodeEventHub()
```


### ConfigurationCompleted {#ConfigurationCompleted}
```
public final Event<EventHandler> ConfigurationCompleted
```


Arama ağı yapılandırma süreci tamamlandığında gerçekleşir.


### IndexingCompleted {#IndexingCompleted}
```
public final Event<EventHandler> IndexingCompleted
```


Kuyruğa alınan tüm belgelerin indekslemesi tamamlandığında gerçekleşir.


### DeletionCompleted {#DeletionCompleted}
```
public final Event<EventHandler> DeletionCompleted
```


Tüm kuyruğa alınmış belge silme işlemleri tamamlandığında oluşur.


### OptimizationCompleted {#OptimizationCompleted}
```
public final Event<EventHandler> OptimizationCompleted
```


Tüm düğümlerin optimizasyonu tamamlandığında oluşur.


### SynchronizationCompleted {#SynchronizationCompleted}
```
public final Event<EventHandler> SynchronizationCompleted
```


Tüm düğümlerle senkronizasyon tamamlandığında oluşur.


### AttributeChangesCompleted {#AttributeChangesCompleted}
```
public final Event<EventHandler> AttributeChangesCompleted
```


Tüm kuyruğa alınmış öznitelik değişiklikleri tamamlandığında oluşur.


### StatusChanged {#StatusChanged}
```
public final Event<EventHandler<StatusChangedEventArgs>> StatusChanged
```


Arama ağı durumu değiştiğinde oluşur.


### DataExtracted {#DataExtracted}
```
public final Event<EventHandler<DataExtractedEventArgs>> DataExtracted
```


Veri bir belgeden çıkarıldığında oluşur.


### DocumentIndexed {#DocumentIndexed}
```
public final Event<EventHandler<DocumentIndexedEventArgs>> DocumentIndexed
```


Bir belge indekslendiğinde oluşur.


### DocumentDeleted {#DocumentDeleted}
```
public final Event<EventHandler<DocumentDeletedEventArgs>> DocumentDeleted
```


Bir belge silindiğinde oluşur.


### ErrorOccurred {#ErrorOccurred}
```
public final Event<EventHandler<ErrorOccurredEventArgs>> ErrorOccurred
```


Arama ağının bir düğümünde bir hata oluştuğunda oluşur.


### IndexingProgressChanged {#IndexingProgressChanged}
```
public final Event<EventHandler<NetworkIndexingProgressEventArgs>> IndexingProgressChanged
```


İndeksleme işleminin ilerlemesi değiştiğinde oluşur.


### OptimizationProgressChanged {#OptimizationProgressChanged}
```
public final Event<EventHandler<NetworkOptimizationProgressEventArgs>> OptimizationProgressChanged
```


Optimizasyon işleminin ilerlemesi değiştiğinde oluşur.


