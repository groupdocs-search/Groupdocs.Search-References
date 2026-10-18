---
title: "NodeEventHub"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Proporciona eventos de nodo para suscribirse."
type: docs
weight: 16
url: /es/java/com.groupdocs.search.scaling.events/nodeeventhub/
---
**Inheritance:**
java.lang.Object
```
public abstract class NodeEventHub
```

Proporciona eventos de nodo para suscribirse.

## Constructores

| Constructor | Descripción |
| --- | --- |
| [NodeEventHub()](#NodeEventHub--) |  |
## Campos

| Campo | Descripción |
| --- | --- |
|  | [ConfigurationCompleted](#ConfigurationCompleted) | Ocurre cuando se termina el proceso de configuración de la red de búsqueda. |
|
|  | [IndexingCompleted](#IndexingCompleted) | Ocurre cuando se termina la indexación de todos los documentos en cola. |
|
|  | [DeletionCompleted](#DeletionCompleted) | Ocurre cuando se terminan todas las eliminaciones en cola de documentos. |
|
|  | [OptimizationCompleted](#OptimizationCompleted) | Ocurre cuando se termina la optimización de todos los nodos. |
|
|  | [SynchronizationCompleted](#SynchronizationCompleted) | Ocurre cuando se termina la sincronización con todos los nodos. |
|
|  | [AttributeChangesCompleted](#AttributeChangesCompleted) | Ocurre cuando se terminan todos los cambios de atributos en cola. |
|
|  | [StatusChanged](#StatusChanged) | Ocurre cuando cambia el estado de la red de búsqueda. |
|
|  | [DataExtracted](#DataExtracted) | Ocurre cuando los datos han sido extraídos de un documento. |
|
|  | [DocumentIndexed](#DocumentIndexed) | Ocurre cuando un documento ha sido indexado. |
|
|  | [DocumentDeleted](#DocumentDeleted) | Ocurre cuando un documento ha sido eliminado. |
|
|  | [ErrorOccurred](#ErrorOccurred) | Ocurre cuando se produce un error en uno de los nodos de la red de búsqueda. |
|
|  | [IndexingProgressChanged](#IndexingProgressChanged) | Ocurre cuando cambia el progreso de la operación de indexación. |
|
|  | [OptimizationProgressChanged](#OptimizationProgressChanged) | Ocurre cuando cambia el progreso de la operación de optimización. |
|
### NodeEventHub() {#NodeEventHub--}
```
public NodeEventHub()
```


### ConfigurationCompleted {#ConfigurationCompleted}
```
public final Event<EventHandler> ConfigurationCompleted
```


Ocurre cuando se termina el proceso de configuración de la red de búsqueda.


### IndexingCompleted {#IndexingCompleted}
```
public final Event<EventHandler> IndexingCompleted
```


Ocurre cuando se termina la indexación de todos los documentos en cola.


### DeletionCompleted {#DeletionCompleted}
```
public final Event<EventHandler> DeletionCompleted
```


Ocurre cuando se terminan todas las eliminaciones en cola de documentos.


### OptimizationCompleted {#OptimizationCompleted}
```
public final Event<EventHandler> OptimizationCompleted
```


Ocurre cuando se termina la optimización de todos los nodos.


### SynchronizationCompleted {#SynchronizationCompleted}
```
public final Event<EventHandler> SynchronizationCompleted
```


Ocurre cuando se termina la sincronización con todos los nodos.


### AttributeChangesCompleted {#AttributeChangesCompleted}
```
public final Event<EventHandler> AttributeChangesCompleted
```


Ocurre cuando se terminan todos los cambios de atributos en cola.


### StatusChanged {#StatusChanged}
```
public final Event<EventHandler<StatusChangedEventArgs>> StatusChanged
```


Ocurre cuando cambia el estado de la red de búsqueda.


### DataExtracted {#DataExtracted}
```
public final Event<EventHandler<DataExtractedEventArgs>> DataExtracted
```


Ocurre cuando los datos han sido extraídos de un documento.


### DocumentIndexed {#DocumentIndexed}
```
public final Event<EventHandler<DocumentIndexedEventArgs>> DocumentIndexed
```


Ocurre cuando un documento ha sido indexado.


### DocumentDeleted {#DocumentDeleted}
```
public final Event<EventHandler<DocumentDeletedEventArgs>> DocumentDeleted
```


Ocurre cuando un documento ha sido eliminado.


### ErrorOccurred {#ErrorOccurred}
```
public final Event<EventHandler<ErrorOccurredEventArgs>> ErrorOccurred
```


Ocurre cuando se produce un error en uno de los nodos de la red de búsqueda.


### IndexingProgressChanged {#IndexingProgressChanged}
```
public final Event<EventHandler<NetworkIndexingProgressEventArgs>> IndexingProgressChanged
```


Ocurre cuando cambia el progreso de la operación de indexación.


### OptimizationProgressChanged {#OptimizationProgressChanged}
```
public final Event<EventHandler<NetworkOptimizationProgressEventArgs>> OptimizationProgressChanged
```


Ocurre cuando cambia el progreso de la operación de optimización.


