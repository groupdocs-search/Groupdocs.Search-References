---
title: "NodeEventHub"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Stellt Knotenereignisse zum Abonnieren bereit."
type: docs
weight: 16
url: /de/java/com.groupdocs.search.scaling.events/nodeeventhub/
---
**Inheritance:**
java.lang.Object
```
public abstract class NodeEventHub
```

Stellt Knotenereignisse zum Abonnieren bereit.

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [NodeEventHub()](#NodeEventHub--) |  |
## Felder

| Feld | Beschreibung |
| --- | --- |
|  | [ConfigurationCompleted](#ConfigurationCompleted) | Tritt auf, wenn der Konfigurationsprozess des Suchnetzwerks abgeschlossen ist. |
|
|  | [IndexingCompleted](#IndexingCompleted) | Tritt auf, wenn die Indizierung aller eingereichten Dokumente abgeschlossen ist. |
|
|  | [DeletionCompleted](#DeletionCompleted) | Tritt auf, wenn alle eingereichten Löschungen von Dokumenten abgeschlossen sind. |
|
|  | [OptimizationCompleted](#OptimizationCompleted) | Tritt auf, wenn die Optimierung aller Knoten abgeschlossen ist. |
|
|  | [SynchronizationCompleted](#SynchronizationCompleted) | Tritt auf, wenn die Synchronisation mit allen Knoten abgeschlossen ist. |
|
|  | [AttributeChangesCompleted](#AttributeChangesCompleted) | Tritt auf, wenn alle eingereichten Attributänderungen abgeschlossen sind. |
|
|  | [StatusChanged](#StatusChanged) | Tritt auf, wenn sich der Status des Suchnetzwerks ändert. |
|
|  | [DataExtracted](#DataExtracted) | Tritt auf, wenn die Daten aus einem Dokument extrahiert wurden. |
|
|  | [DocumentIndexed](#DocumentIndexed) | Tritt auf, wenn ein Dokument indiziert wurde. |
|
|  | [DocumentDeleted](#DocumentDeleted) | Tritt auf, wenn ein Dokument gelöscht wurde. |
|
|  | [ErrorOccurred](#ErrorOccurred) | Tritt auf, wenn in einem der Knoten des Suchnetzwerks ein Fehler auftritt. |
|
|  | [IndexingProgressChanged](#IndexingProgressChanged) | Tritt auf, wenn sich der Fortschritt des Indizierungsvorgangs geändert hat. |
|
|  | [OptimizationProgressChanged](#OptimizationProgressChanged) | Tritt auf, wenn sich der Fortschritt des Optimierungsvorgangs geändert hat. |
|
### NodeEventHub() {#NodeEventHub--}
```
public NodeEventHub()
```


### ConfigurationCompleted {#ConfigurationCompleted}
```
public final Event<EventHandler> ConfigurationCompleted
```


Tritt auf, wenn der Konfigurationsprozess des Suchnetzwerks abgeschlossen ist.


### IndexingCompleted {#IndexingCompleted}
```
public final Event<EventHandler> IndexingCompleted
```


Tritt auf, wenn die Indizierung aller eingereichten Dokumente abgeschlossen ist.


### DeletionCompleted {#DeletionCompleted}
```
public final Event<EventHandler> DeletionCompleted
```


Tritt auf, wenn alle eingereichten Löschungen von Dokumenten abgeschlossen sind.


### OptimizationCompleted {#OptimizationCompleted}
```
public final Event<EventHandler> OptimizationCompleted
```


Tritt auf, wenn die Optimierung aller Knoten abgeschlossen ist.


### SynchronizationCompleted {#SynchronizationCompleted}
```
public final Event<EventHandler> SynchronizationCompleted
```


Tritt auf, wenn die Synchronisation mit allen Knoten abgeschlossen ist.


### AttributeChangesCompleted {#AttributeChangesCompleted}
```
public final Event<EventHandler> AttributeChangesCompleted
```


Tritt auf, wenn alle eingereichten Attributänderungen abgeschlossen sind.


### StatusChanged {#StatusChanged}
```
public final Event<EventHandler<StatusChangedEventArgs>> StatusChanged
```


Tritt auf, wenn sich der Status des Suchnetzwerks ändert.


### DataExtracted {#DataExtracted}
```
public final Event<EventHandler<DataExtractedEventArgs>> DataExtracted
```


Tritt auf, wenn die Daten aus einem Dokument extrahiert wurden.


### DocumentIndexed {#DocumentIndexed}
```
public final Event<EventHandler<DocumentIndexedEventArgs>> DocumentIndexed
```


Tritt auf, wenn ein Dokument indiziert wurde.


### DocumentDeleted {#DocumentDeleted}
```
public final Event<EventHandler<DocumentDeletedEventArgs>> DocumentDeleted
```


Tritt auf, wenn ein Dokument gelöscht wurde.


### ErrorOccurred {#ErrorOccurred}
```
public final Event<EventHandler<ErrorOccurredEventArgs>> ErrorOccurred
```


Tritt auf, wenn in einem der Knoten des Suchnetzwerks ein Fehler auftritt.


### IndexingProgressChanged {#IndexingProgressChanged}
```
public final Event<EventHandler<NetworkIndexingProgressEventArgs>> IndexingProgressChanged
```


Tritt auf, wenn sich der Fortschritt des Indizierungsvorgangs geändert hat.


### OptimizationProgressChanged {#OptimizationProgressChanged}
```
public final Event<EventHandler<NetworkOptimizationProgressEventArgs>> OptimizationProgressChanged
```


Tritt auf, wenn sich der Fortschritt des Optimierungsvorgangs geändert hat.


