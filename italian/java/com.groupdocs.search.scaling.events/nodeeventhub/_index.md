---
title: "NodeEventHub"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Fornisce eventi dei nodi per l'iscrizione."
type: docs
weight: 16
url: /it/java/com.groupdocs.search.scaling.events/nodeeventhub/
---
**Inheritance:**
java.lang.Object
```
public abstract class NodeEventHub
```

Fornisce eventi dei nodi per l'iscrizione.

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [NodeEventHub()](#NodeEventHub--) |  |
## Fields

| Field | Descrizione |
| --- | --- |
|  | [ConfigurationCompleted](#ConfigurationCompleted) | Si verifica quando il processo di configurazione della rete di ricerca è terminato. |
|
|  | [IndexingCompleted](#IndexingCompleted) | Si verifica quando l'indicizzazione di tutti i documenti in coda è terminata. |
|
|  | [DeletionCompleted](#DeletionCompleted) | Si verifica quando tutte le eliminazioni di documenti in coda sono terminate. |
|
|  | [OptimizationCompleted](#OptimizationCompleted) | Si verifica quando l'ottimizzazione di tutti i nodi è terminata. |
|
|  | [SynchronizationCompleted](#SynchronizationCompleted) | Si verifica quando la sincronizzazione con tutti i nodi è terminata. |
|
|  | [AttributeChangesCompleted](#AttributeChangesCompleted) | Si verifica quando tutte le modifiche di attributi in coda sono terminate. |
|
|  | [StatusChanged](#StatusChanged) | Si verifica quando lo stato della rete di ricerca cambia. |
|
|  | [DataExtracted](#DataExtracted) | Si verifica quando i dati sono stati estratti da un documento. |
|
|  | [DocumentIndexed](#DocumentIndexed) | Si verifica quando un documento è stato indicizzato. |
|
|  | [DocumentDeleted](#DocumentDeleted) | Si verifica quando un documento è stato eliminato. |
|
|  | [ErrorOccurred](#ErrorOccurred) | Si verifica quando si verifica un errore in uno dei nodi della rete di ricerca. |
|
|  | [IndexingProgressChanged](#IndexingProgressChanged) | Si verifica quando il progresso dell'operazione di indicizzazione è cambiato. |
|
|  | [OptimizationProgressChanged](#OptimizationProgressChanged) | Si verifica quando il progresso dell'operazione di ottimizzazione è cambiato. |
|
### NodeEventHub() {#NodeEventHub--}
```
public NodeEventHub()
```


### ConfigurationCompleted {#ConfigurationCompleted}
```
public final Event<EventHandler> ConfigurationCompleted
```


Si verifica quando il processo di configurazione della rete di ricerca è terminato.


### IndexingCompleted {#IndexingCompleted}
```
public final Event<EventHandler> IndexingCompleted
```


Si verifica quando l'indicizzazione di tutti i documenti in coda è terminata.


### DeletionCompleted {#DeletionCompleted}
```
public final Event<EventHandler> DeletionCompleted
```


Si verifica quando tutte le eliminazioni di documenti in coda sono terminate.


### OptimizationCompleted {#OptimizationCompleted}
```
public final Event<EventHandler> OptimizationCompleted
```


Si verifica quando l'ottimizzazione di tutti i nodi è terminata.


### SynchronizationCompleted {#SynchronizationCompleted}
```
public final Event<EventHandler> SynchronizationCompleted
```


Si verifica quando la sincronizzazione con tutti i nodi è terminata.


### AttributeChangesCompleted {#AttributeChangesCompleted}
```
public final Event<EventHandler> AttributeChangesCompleted
```


Si verifica quando tutte le modifiche di attributi in coda sono terminate.


### StatusChanged {#StatusChanged}
```
public final Event<EventHandler<StatusChangedEventArgs>> StatusChanged
```


Si verifica quando lo stato della rete di ricerca cambia.


### DataExtracted {#DataExtracted}
```
public final Event<EventHandler<DataExtractedEventArgs>> DataExtracted
```


Si verifica quando i dati sono stati estratti da un documento.


### DocumentIndexed {#DocumentIndexed}
```
public final Event<EventHandler<DocumentIndexedEventArgs>> DocumentIndexed
```


Si verifica quando un documento è stato indicizzato.


### DocumentDeleted {#DocumentDeleted}
```
public final Event<EventHandler<DocumentDeletedEventArgs>> DocumentDeleted
```


Si verifica quando un documento è stato eliminato.


### ErrorOccurred {#ErrorOccurred}
```
public final Event<EventHandler<ErrorOccurredEventArgs>> ErrorOccurred
```


Si verifica quando si verifica un errore in uno dei nodi della rete di ricerca.


### IndexingProgressChanged {#IndexingProgressChanged}
```
public final Event<EventHandler<NetworkIndexingProgressEventArgs>> IndexingProgressChanged
```


Si verifica quando il progresso dell'operazione di indicizzazione è cambiato.


### OptimizationProgressChanged {#OptimizationProgressChanged}
```
public final Event<EventHandler<NetworkOptimizationProgressEventArgs>> OptimizationProgressChanged
```


Si verifica quando il progresso dell'operazione di ottimizzazione è cambiato.


