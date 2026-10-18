---
title: "NodeEventHub"
second_title: "GroupDocs.Search για Java API Reference"
description: "Παρέχει γεγονότα κόμβου για εγγραφή."
type: docs
weight: 16
url: /el/java/com.groupdocs.search.scaling.events/nodeeventhub/
---
**Inheritance:**
java.lang.Object
```
public abstract class NodeEventHub
```

Παρέχει γεγονότα κόμβου για εγγραφή.

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [NodeEventHub()](#NodeEventHub--) |  |
## Πεδία

| Πεδίο | Περιγραφή |
| --- | --- |
|  | [ConfigurationCompleted](#ConfigurationCompleted) | Συμβαίνει όταν ολοκληρωθεί η διαδικασία διαμόρφωσης του δικτύου αναζήτησης. |
|
|  | [IndexingCompleted](#IndexingCompleted) | Συμβαίνει όταν ολοκληρωθεί η ευρετηρίαση όλων των εγγεγραμμένων εγγράφων. |
|
|  | [DeletionCompleted](#DeletionCompleted) | Συμβαίνει όταν ολοκληρωθούν όλες οι εγγεγραμμένες διαγραφές εγγράφων. |
|
|  | [OptimizationCompleted](#OptimizationCompleted) | Συμβαίνει όταν ολοκληρωθεί η βελτιστοποίηση όλων των κόμβων. |
|
|  | [SynchronizationCompleted](#SynchronizationCompleted) | Συμβαίνει όταν ολοκληρωθεί ο συγχρονισμός με όλους τους κόμβους. |
|
|  | [AttributeChangesCompleted](#AttributeChangesCompleted) | Συμβαίνει όταν ολοκληρωθούν όλες οι εγγεγραμμένες αλλαγές ιδιοτήτων. |
|
|  | [StatusChanged](#StatusChanged) | Συμβαίνει όταν αλλάξει η κατάσταση του δικτύου αναζήτησης. |
|
|  | [DataExtracted](#DataExtracted) | Συμβαίνει όταν τα δεδομένα έχουν εξαχθεί από ένα έγγραφο. |
|
|  | [DocumentIndexed](#DocumentIndexed) | Συμβαίνει όταν ένα έγγραφο έχει ευρετηριαστεί. |
|
|  | [DocumentDeleted](#DocumentDeleted) | Συμβαίνει όταν ένα έγγραφο έχει διαγραφεί. |
|
|  | [ErrorOccurred](#ErrorOccurred) | Συμβαίνει όταν προκύψει σφάλμα σε έναν από τους κόμβους του δικτύου αναζήτησης. |
|
|  | [IndexingProgressChanged](#IndexingProgressChanged) | Συμβαίνει όταν αλλάξει η πρόοδος της λειτουργίας ευρετηρίασης. |
|
|  | [OptimizationProgressChanged](#OptimizationProgressChanged) | Συμβαίνει όταν αλλάξει η πρόοδος της λειτουργίας βελτιστοποίησης. |
|
### NodeEventHub() {#NodeEventHub--}
```
public NodeEventHub()
```


### ConfigurationCompleted {#ConfigurationCompleted}
```
public final Event<EventHandler> ConfigurationCompleted
```


Συμβαίνει όταν ολοκληρωθεί η διαδικασία διαμόρφωσης του δικτύου αναζήτησης.


### IndexingCompleted {#IndexingCompleted}
```
public final Event<EventHandler> IndexingCompleted
```


Συμβαίνει όταν ολοκληρωθεί η ευρετηρίαση όλων των εγγεγραμμένων εγγράφων.


### DeletionCompleted {#DeletionCompleted}
```
public final Event<EventHandler> DeletionCompleted
```


Συμβαίνει όταν ολοκληρωθούν όλες οι εγγεγραμμένες διαγραφές εγγράφων.


### OptimizationCompleted {#OptimizationCompleted}
```
public final Event<EventHandler> OptimizationCompleted
```


Συμβαίνει όταν ολοκληρωθεί η βελτιστοποίηση όλων των κόμβων.


### SynchronizationCompleted {#SynchronizationCompleted}
```
public final Event<EventHandler> SynchronizationCompleted
```


Συμβαίνει όταν ολοκληρωθεί ο συγχρονισμός με όλους τους κόμβους.


### AttributeChangesCompleted {#AttributeChangesCompleted}
```
public final Event<EventHandler> AttributeChangesCompleted
```


Συμβαίνει όταν ολοκληρωθούν όλες οι εγγεγραμμένες αλλαγές ιδιοτήτων.


### StatusChanged {#StatusChanged}
```
public final Event<EventHandler<StatusChangedEventArgs>> StatusChanged
```


Συμβαίνει όταν αλλάξει η κατάσταση του δικτύου αναζήτησης.


### DataExtracted {#DataExtracted}
```
public final Event<EventHandler<DataExtractedEventArgs>> DataExtracted
```


Συμβαίνει όταν τα δεδομένα έχουν εξαχθεί από ένα έγγραφο.


### DocumentIndexed {#DocumentIndexed}
```
public final Event<EventHandler<DocumentIndexedEventArgs>> DocumentIndexed
```


Συμβαίνει όταν ένα έγγραφο έχει ευρετηριαστεί.


### DocumentDeleted {#DocumentDeleted}
```
public final Event<EventHandler<DocumentDeletedEventArgs>> DocumentDeleted
```


Συμβαίνει όταν ένα έγγραφο έχει διαγραφεί.


### ErrorOccurred {#ErrorOccurred}
```
public final Event<EventHandler<ErrorOccurredEventArgs>> ErrorOccurred
```


Συμβαίνει όταν προκύψει σφάλμα σε έναν από τους κόμβους του δικτύου αναζήτησης.


### IndexingProgressChanged {#IndexingProgressChanged}
```
public final Event<EventHandler<NetworkIndexingProgressEventArgs>> IndexingProgressChanged
```


Συμβαίνει όταν αλλάξει η πρόοδος της λειτουργίας ευρετηρίασης.


### OptimizationProgressChanged {#OptimizationProgressChanged}
```
public final Event<EventHandler<NetworkOptimizationProgressEventArgs>> OptimizationProgressChanged
```


Συμβαίνει όταν αλλάξει η πρόοδος της λειτουργίας βελτιστοποίησης.


