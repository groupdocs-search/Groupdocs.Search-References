---
title: "NodeEventHub"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Biedt knooppunteenementen om op te abonneren."
type: docs
weight: 16
url: /nl/java/com.groupdocs.search.scaling.events/nodeeventhub/
---
**Inheritance:**
java.lang.Object
```
public abstract class NodeEventHub
```

Biedt knooppunteenementen om op te abonneren.

## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [NodeEventHub()](#NodeEventHub--) |  |
## Velden

| Veld | Beschrijving |
| --- | --- |
|  | [ConfigurationCompleted](#ConfigurationCompleted) | Vindt plaats wanneer het configuratieproces van het zoeknetwerk is voltooid. |
|
|  | [IndexingCompleted](#IndexingCompleted) | Vindt plaats wanneer het indexeren van alle in de wachtrij geplaatste documenten is voltooid. |
|
|  | [DeletionCompleted](#DeletionCompleted) | Vindt plaats wanneer alle in de wachtrij geplaatste verwijderingen van documenten zijn voltooid. |
|
|  | [OptimizationCompleted](#OptimizationCompleted) | Vindt plaats wanneer de optimalisatie van alle knooppunten is voltooid. |
|
|  | [SynchronizationCompleted](#SynchronizationCompleted) | Vindt plaats wanneer de synchronisatie met alle knooppunten is voltooid. |
|
|  | [AttributeChangesCompleted](#AttributeChangesCompleted) | Vindt plaats wanneer alle in de wachtrij geplaatste attribuutwijzigingen zijn voltooid. |
|
|  | [StatusChanged](#StatusChanged) | Vindt plaats wanneer de status van het zoeknetwerk verandert. |
|
|  | [DataExtracted](#DataExtracted) | Vindt plaats wanneer de gegevens uit een document zijn geëxtraheerd. |
|
|  | [DocumentIndexed](#DocumentIndexed) | Vindt plaats wanneer een document is geïndexeerd. |
|
|  | [DocumentDeleted](#DocumentDeleted) | Vindt plaats wanneer een document is verwijderd. |
|
|  | [ErrorOccurred](#ErrorOccurred) | Vindt plaats wanneer er een fout optreedt in een van de knooppunten van het zoeknetwerk. |
|
|  | [IndexingProgressChanged](#IndexingProgressChanged) | Vindt plaats wanneer de voortgang van de indexeringsbewerking is gewijzigd. |
|
|  | [OptimizationProgressChanged](#OptimizationProgressChanged) | Vindt plaats wanneer de voortgang van de optimalisatiebewerking is gewijzigd. |
|
### NodeEventHub() {#NodeEventHub--}
```
public NodeEventHub()
```


### ConfigurationCompleted {#ConfigurationCompleted}
```
public final Event<EventHandler> ConfigurationCompleted
```


Vindt plaats wanneer het configuratieproces van het zoeknetwerk is voltooid.


### IndexingCompleted {#IndexingCompleted}
```
public final Event<EventHandler> IndexingCompleted
```


Vindt plaats wanneer het indexeren van alle in de wachtrij geplaatste documenten is voltooid.


### DeletionCompleted {#DeletionCompleted}
```
public final Event<EventHandler> DeletionCompleted
```


Vindt plaats wanneer alle in de wachtrij geplaatste verwijderingen van documenten zijn voltooid.


### OptimizationCompleted {#OptimizationCompleted}
```
public final Event<EventHandler> OptimizationCompleted
```


Vindt plaats wanneer de optimalisatie van alle knooppunten is voltooid.


### SynchronizationCompleted {#SynchronizationCompleted}
```
public final Event<EventHandler> SynchronizationCompleted
```


Vindt plaats wanneer de synchronisatie met alle knooppunten is voltooid.


### AttributeChangesCompleted {#AttributeChangesCompleted}
```
public final Event<EventHandler> AttributeChangesCompleted
```


Vindt plaats wanneer alle in de wachtrij geplaatste attribuutwijzigingen zijn voltooid.


### StatusChanged {#StatusChanged}
```
public final Event<EventHandler<StatusChangedEventArgs>> StatusChanged
```


Vindt plaats wanneer de status van het zoeknetwerk verandert.


### DataExtracted {#DataExtracted}
```
public final Event<EventHandler<DataExtractedEventArgs>> DataExtracted
```


Vindt plaats wanneer de gegevens uit een document zijn geëxtraheerd.


### DocumentIndexed {#DocumentIndexed}
```
public final Event<EventHandler<DocumentIndexedEventArgs>> DocumentIndexed
```


Vindt plaats wanneer een document is geïndexeerd.


### DocumentDeleted {#DocumentDeleted}
```
public final Event<EventHandler<DocumentDeletedEventArgs>> DocumentDeleted
```


Vindt plaats wanneer een document is verwijderd.


### ErrorOccurred {#ErrorOccurred}
```
public final Event<EventHandler<ErrorOccurredEventArgs>> ErrorOccurred
```


Vindt plaats wanneer er een fout optreedt in een van de knooppunten van het zoeknetwerk.


### IndexingProgressChanged {#IndexingProgressChanged}
```
public final Event<EventHandler<NetworkIndexingProgressEventArgs>> IndexingProgressChanged
```


Vindt plaats wanneer de voortgang van de indexeringsbewerking is gewijzigd.


### OptimizationProgressChanged {#OptimizationProgressChanged}
```
public final Event<EventHandler<NetworkOptimizationProgressEventArgs>> OptimizationProgressChanged
```


Vindt plaats wanneer de voortgang van de optimalisatiebewerking is gewijzigd.


