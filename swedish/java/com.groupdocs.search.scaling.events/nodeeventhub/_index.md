---
title: "NodeEventHub"
second_title: "GroupDocs.Search för Java API-referens"
description: "Tillhandahåller nodhändelser för prenumeration."
type: docs
weight: 16
url: /sv/java/com.groupdocs.search.scaling.events/nodeeventhub/
---
**Inheritance:**
java.lang.Object
```
public abstract class NodeEventHub
```

Tillhandahåller nodhändelser för prenumeration.

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [NodeEventHub()](#NodeEventHub--) |  |
## Fält

| Fält | Beskrivning |
| --- | --- |
|  | [ConfigurationCompleted](#ConfigurationCompleted) | Uppstår när konfigurationsprocessen för söknätverket är klar. |
|
|  | [IndexingCompleted](#IndexingCompleted) | Uppstår när indexeringen av alla köade dokument är klar. |
|
|  | [DeletionCompleted](#DeletionCompleted) | Uppstår när alla köade borttagningar av dokument är klara. |
|
|  | [OptimizationCompleted](#OptimizationCompleted) | Uppstår när optimeringen av alla noder är klar. |
|
|  | [SynchronizationCompleted](#SynchronizationCompleted) | Uppstår när synkroniseringen med alla noder är klar. |
|
|  | [AttributeChangesCompleted](#AttributeChangesCompleted) | Uppstår när alla köade attributändringar är klara. |
|
|  | [StatusChanged](#StatusChanged) | Uppstår när statusen för söknätverket ändras. |
|
|  | [DataExtracted](#DataExtracted) | Uppstår när data har extraherats från ett dokument. |
|
|  | [DocumentIndexed](#DocumentIndexed) | Uppstår när ett dokument har indexerats. |
|
|  | [DocumentDeleted](#DocumentDeleted) | Uppstår när ett dokument har raderats. |
|
|  | [ErrorOccurred](#ErrorOccurred) | Uppstår när ett fel inträffar i en av noderna i söknätverket. |
|
|  | [IndexingProgressChanged](#IndexingProgressChanged) | Uppstår när framstegen för indexeringsoperationen har ändrats. |
|
|  | [OptimizationProgressChanged](#OptimizationProgressChanged) | Uppstår när framstegen för optimeringsoperationen har ändrats. |
|
### NodeEventHub() {#NodeEventHub--}
```
public NodeEventHub()
```


### ConfigurationCompleted {#ConfigurationCompleted}
```
public final Event<EventHandler> ConfigurationCompleted
```


Uppstår när konfigurationsprocessen för söknätverket är klar.


### IndexingCompleted {#IndexingCompleted}
```
public final Event<EventHandler> IndexingCompleted
```


Uppstår när indexeringen av alla köade dokument är klar.


### DeletionCompleted {#DeletionCompleted}
```
public final Event<EventHandler> DeletionCompleted
```


Uppstår när alla köade borttagningar av dokument är klara.


### OptimizationCompleted {#OptimizationCompleted}
```
public final Event<EventHandler> OptimizationCompleted
```


Uppstår när optimeringen av alla noder är klar.


### SynchronizationCompleted {#SynchronizationCompleted}
```
public final Event<EventHandler> SynchronizationCompleted
```


Uppstår när synkroniseringen med alla noder är klar.


### AttributeChangesCompleted {#AttributeChangesCompleted}
```
public final Event<EventHandler> AttributeChangesCompleted
```


Uppstår när alla köade attributändringar är klara.


### StatusChanged {#StatusChanged}
```
public final Event<EventHandler<StatusChangedEventArgs>> StatusChanged
```


Uppstår när statusen för söknätverket ändras.


### DataExtracted {#DataExtracted}
```
public final Event<EventHandler<DataExtractedEventArgs>> DataExtracted
```


Uppstår när data har extraherats från ett dokument.


### DocumentIndexed {#DocumentIndexed}
```
public final Event<EventHandler<DocumentIndexedEventArgs>> DocumentIndexed
```


Uppstår när ett dokument har indexerats.


### DocumentDeleted {#DocumentDeleted}
```
public final Event<EventHandler<DocumentDeletedEventArgs>> DocumentDeleted
```


Uppstår när ett dokument har raderats.


### ErrorOccurred {#ErrorOccurred}
```
public final Event<EventHandler<ErrorOccurredEventArgs>> ErrorOccurred
```


Uppstår när ett fel inträffar i en av noderna i söknätverket.


### IndexingProgressChanged {#IndexingProgressChanged}
```
public final Event<EventHandler<NetworkIndexingProgressEventArgs>> IndexingProgressChanged
```


Uppstår när framstegen för indexeringsoperationen har ändrats.


### OptimizationProgressChanged {#OptimizationProgressChanged}
```
public final Event<EventHandler<NetworkOptimizationProgressEventArgs>> OptimizationProgressChanged
```


Uppstår när framstegen för optimeringsoperationen har ändrats.


