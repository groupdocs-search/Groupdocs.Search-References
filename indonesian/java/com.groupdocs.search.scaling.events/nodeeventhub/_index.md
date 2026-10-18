---
title: "NodeEventHub"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Menyediakan peristiwa node untuk berlangganan."
type: docs
weight: 16
url: /id/java/com.groupdocs.search.scaling.events/nodeeventhub/
---
**Inheritance:**
java.lang.Object
```
public abstract class NodeEventHub
```

Menyediakan peristiwa node untuk berlangganan.

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [NodeEventHub()](#NodeEventHub--) |  |
## Fields

| Field | Deskripsi |
| --- | --- |
|  | [ConfigurationCompleted](#ConfigurationCompleted) | Terjadi ketika proses konfigurasi jaringan pencarian selesai. |
|
|  | [IndexingCompleted](#IndexingCompleted) | Terjadi ketika pengindeksan semua dokumen yang antre selesai. |
|
|  | [DeletionCompleted](#DeletionCompleted) | Terjadi ketika semua penghapusan dokumen yang antre selesai. |
|
|  | [OptimizationCompleted](#OptimizationCompleted) | Terjadi ketika optimasi semua node selesai. |
|
|  | [SynchronizationCompleted](#SynchronizationCompleted) | Terjadi ketika sinkronisasi dengan semua node selesai. |
|
|  | [AttributeChangesCompleted](#AttributeChangesCompleted) | Terjadi ketika semua perubahan atribut yang antre selesai. |
|
|  | [StatusChanged](#StatusChanged) | Terjadi ketika status jaringan pencarian berubah. |
|
|  | [DataExtracted](#DataExtracted) | Terjadi ketika data telah diekstrak dari sebuah dokumen. |
|
|  | [DocumentIndexed](#DocumentIndexed) | Terjadi ketika sebuah dokumen telah diindeks. |
|
|  | [DocumentDeleted](#DocumentDeleted) | Terjadi ketika sebuah dokumen telah dihapus. |
|
|  | [ErrorOccurred](#ErrorOccurred) | Terjadi ketika terjadi kesalahan pada salah satu node jaringan pencarian. |
|
|  | [IndexingProgressChanged](#IndexingProgressChanged) | Terjadi ketika kemajuan operasi pengindeksan berubah. |
|
|  | [OptimizationProgressChanged](#OptimizationProgressChanged) | Terjadi ketika kemajuan operasi optimasi berubah. |
|
### NodeEventHub() {#NodeEventHub--}
```
public NodeEventHub()
```


### ConfigurationCompleted {#ConfigurationCompleted}
```
public final Event<EventHandler> ConfigurationCompleted
```


Terjadi ketika proses konfigurasi jaringan pencarian selesai.


### IndexingCompleted {#IndexingCompleted}
```
public final Event<EventHandler> IndexingCompleted
```


Terjadi ketika pengindeksan semua dokumen yang antre selesai.


### DeletionCompleted {#DeletionCompleted}
```
public final Event<EventHandler> DeletionCompleted
```


Terjadi ketika semua penghapusan dokumen yang antre selesai.


### OptimizationCompleted {#OptimizationCompleted}
```
public final Event<EventHandler> OptimizationCompleted
```


Terjadi ketika optimasi semua node selesai.


### SynchronizationCompleted {#SynchronizationCompleted}
```
public final Event<EventHandler> SynchronizationCompleted
```


Terjadi ketika sinkronisasi dengan semua node selesai.


### AttributeChangesCompleted {#AttributeChangesCompleted}
```
public final Event<EventHandler> AttributeChangesCompleted
```


Terjadi ketika semua perubahan atribut yang antre selesai.


### StatusChanged {#StatusChanged}
```
public final Event<EventHandler<StatusChangedEventArgs>> StatusChanged
```


Terjadi ketika status jaringan pencarian berubah.


### DataExtracted {#DataExtracted}
```
public final Event<EventHandler<DataExtractedEventArgs>> DataExtracted
```


Terjadi ketika data telah diekstrak dari sebuah dokumen.


### DocumentIndexed {#DocumentIndexed}
```
public final Event<EventHandler<DocumentIndexedEventArgs>> DocumentIndexed
```


Terjadi ketika sebuah dokumen telah diindeks.


### DocumentDeleted {#DocumentDeleted}
```
public final Event<EventHandler<DocumentDeletedEventArgs>> DocumentDeleted
```


Terjadi ketika sebuah dokumen telah dihapus.


### ErrorOccurred {#ErrorOccurred}
```
public final Event<EventHandler<ErrorOccurredEventArgs>> ErrorOccurred
```


Terjadi ketika terjadi kesalahan pada salah satu node jaringan pencarian.


### IndexingProgressChanged {#IndexingProgressChanged}
```
public final Event<EventHandler<NetworkIndexingProgressEventArgs>> IndexingProgressChanged
```


Terjadi ketika kemajuan operasi pengindeksan berubah.


### OptimizationProgressChanged {#OptimizationProgressChanged}
```
public final Event<EventHandler<NetworkOptimizationProgressEventArgs>> OptimizationProgressChanged
```


Terjadi ketika kemajuan operasi optimasi berubah.


