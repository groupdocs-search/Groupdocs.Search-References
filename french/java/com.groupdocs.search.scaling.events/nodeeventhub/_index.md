---
title: "NodeEventHub"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Fournit des événements de nœud pour l'abonnement."
type: docs
weight: 16
url: /fr/java/com.groupdocs.search.scaling.events/nodeeventhub/
---
**Inheritance:**
java.lang.Object
```
public abstract class NodeEventHub
```

Fournit des événements de nœud pour l'abonnement.

## Constructeurs

| Constructeur | Description |
| --- | --- |
| [NodeEventHub()](#NodeEventHub--) |  |
## Fields

| Field | Description |
| --- | --- |
|  | [ConfigurationCompleted](#ConfigurationCompleted) | Se produit lorsque le processus de configuration du réseau de recherche est terminé. |
|
|  | [IndexingCompleted](#IndexingCompleted) | Se produit lorsque l'indexation de tous les documents en file d'attente est terminée. |
|
|  | [DeletionCompleted](#DeletionCompleted) | Se produit lorsque toutes les suppressions en file d'attente de documents sont terminées. |
|
|  | [OptimizationCompleted](#OptimizationCompleted) | Se produit lorsque l'optimisation de tous les nœuds est terminée. |
|
|  | [SynchronizationCompleted](#SynchronizationCompleted) | Se produit lorsque la synchronisation avec tous les nœuds est terminée. |
|
|  | [AttributeChangesCompleted](#AttributeChangesCompleted) | Se produit lorsque tous les changements d'attributs en file d'attente sont terminés. |
|
|  | [StatusChanged](#StatusChanged) | Se produit lorsque l'état du réseau de recherche change. |
|
|  | [DataExtracted](#DataExtracted) | Se produit lorsque les données ont été extraites d'un document. |
|
|  | [DocumentIndexed](#DocumentIndexed) | Se produit lorsqu'un document a été indexé. |
|
|  | [DocumentDeleted](#DocumentDeleted) | Se produit lorsqu'un document a été supprimé. |
|
|  | [ErrorOccurred](#ErrorOccurred) | Se produit lorsqu'une erreur survient dans l'un des nœuds du réseau de recherche. |
|
|  | [IndexingProgressChanged](#IndexingProgressChanged) | Se produit lorsque la progression de l'opération d'indexation a changé. |
|
|  | [OptimizationProgressChanged](#OptimizationProgressChanged) | Se produit lorsque la progression de l'opération d'optimisation a changé. |
|
### NodeEventHub() {#NodeEventHub--}
```
public NodeEventHub()
```


### ConfigurationCompleted {#ConfigurationCompleted}
```
public final Event<EventHandler> ConfigurationCompleted
```


Se produit lorsque le processus de configuration du réseau de recherche est terminé.


### IndexingCompleted {#IndexingCompleted}
```
public final Event<EventHandler> IndexingCompleted
```


Se produit lorsque l'indexation de tous les documents en file d'attente est terminée.


### DeletionCompleted {#DeletionCompleted}
```
public final Event<EventHandler> DeletionCompleted
```


Se produit lorsque toutes les suppressions en file d'attente de documents sont terminées.


### OptimizationCompleted {#OptimizationCompleted}
```
public final Event<EventHandler> OptimizationCompleted
```


Se produit lorsque l'optimisation de tous les nœuds est terminée.


### SynchronizationCompleted {#SynchronizationCompleted}
```
public final Event<EventHandler> SynchronizationCompleted
```


Se produit lorsque la synchronisation avec tous les nœuds est terminée.


### AttributeChangesCompleted {#AttributeChangesCompleted}
```
public final Event<EventHandler> AttributeChangesCompleted
```


Se produit lorsque tous les changements d'attributs en file d'attente sont terminés.


### StatusChanged {#StatusChanged}
```
public final Event<EventHandler<StatusChangedEventArgs>> StatusChanged
```


Se produit lorsque l'état du réseau de recherche change.


### DataExtracted {#DataExtracted}
```
public final Event<EventHandler<DataExtractedEventArgs>> DataExtracted
```


Se produit lorsque les données ont été extraites d'un document.


### DocumentIndexed {#DocumentIndexed}
```
public final Event<EventHandler<DocumentIndexedEventArgs>> DocumentIndexed
```


Se produit lorsqu'un document a été indexé.


### DocumentDeleted {#DocumentDeleted}
```
public final Event<EventHandler<DocumentDeletedEventArgs>> DocumentDeleted
```


Se produit lorsqu'un document a été supprimé.


### ErrorOccurred {#ErrorOccurred}
```
public final Event<EventHandler<ErrorOccurredEventArgs>> ErrorOccurred
```


Se produit lorsqu'une erreur survient dans l'un des nœuds du réseau de recherche.


### IndexingProgressChanged {#IndexingProgressChanged}
```
public final Event<EventHandler<NetworkIndexingProgressEventArgs>> IndexingProgressChanged
```


Se produit lorsque la progression de l'opération d'indexation a changé.


### OptimizationProgressChanged {#OptimizationProgressChanged}
```
public final Event<EventHandler<NetworkOptimizationProgressEventArgs>> OptimizationProgressChanged
```


Se produit lorsque la progression de l'opération d'optimisation a changé.


