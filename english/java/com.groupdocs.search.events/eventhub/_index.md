---
title: EventHub
second_title: GroupDocs.Search for Java API Reference
description: Provides index events for subscribing.
type: docs
weight: 13
url: /java/com.groupdocs.search.events/eventhub/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventHubBase](../../com.groupdocs.search.events/eventhubbase)
```
public abstract class EventHub extends EventHubBase
```

Provides index events for subscribing.

**Learn more**

 *  [Search index events][]

The example demonstrates a typical usage of the class.

```

 String indexFolder = "c:\\MyIndex\\";
 String documentsFolder = "c:\\MyDocuments\\";
 String query = "Einstein";
 // Creating an index
 Index index = new Index(indexFolder);
 // Subscribing to the event
 index.getEvents().ErrorOccurred.add(new EventHandler() {
     public void invoke(Object sender, IndexErrorEventArgs args) {
         System.out.println(args.getMessage());
     }
 });
 // Indexing documents from the specified folder
 index.add(documentsFolder);
 // Searching in the index
 SearchResult result = index.search(query);
 
```


[Search index events]: https://docs.groupdocs.com/display/searchjava/Search+index+events
## Constructors

| Constructor | Description |
| --- | --- |
| [EventHub()](#EventHub--) |  |
## Fields

| Field | Description |
| --- | --- |
| [OperationFinished](#OperationFinished) | Occurs when an index operation is finished. |
| [ErrorOccurred](#ErrorOccurred) | Occurs when an error happens during an index operation. |
| [OperationProgressChanged](#OperationProgressChanged) | Occurs when the progress of the indexing or update operation changes. |
| [OptimizationProgressChanged](#OptimizationProgressChanged) | Occurs when the progress of the optimization operation changes. |
| [PasswordRequired](#PasswordRequired) | Occurs when a document requires password for opening. |
| [FileIndexing](#FileIndexing) | Occurs when a document is going to be indexed. |
| [ImagePreparing](#ImagePreparing) | Occurs when an image is going to be prepared for indexing. |
| [StatusChanged](#StatusChanged) | Occurs when the index status changes. |
| [SearchPhaseCompleted](#SearchPhaseCompleted) | Occurs when the search phase is completed. |
### EventHub() {#EventHub--}
```
public EventHub()
```


### OperationFinished {#OperationFinished}
```
public final Event<EventHandler<OperationFinishedEventArgs>> OperationFinished
```


Occurs when an index operation is finished.

The example demonstrates how to use the event.

```

 String indexFolder = "c:\\MyIndex\\";
 String documentsFolder = "c:\\MyDocuments\\";
 // Creating an index
 Index index = new Index(indexFolder);
 // Subscribing to the event
 index.getEvents().OperationFinished.add(new EventHandler() {
     public void invoke(Object sender, OperationFinishedEventArgs args) {
         System.out.println("Operation finished: " + args.getOperationType());
         System.out.println("Message: " + args.getMessage());
         System.out.println("Index folder: " + args.getIndexFolder());
         DateFormat df = new SimpleDateFormat("MM/dd/yyyy HH:mm:ss");
         System.out.println("Time: " + df.format(args.getTime()));
     }
 });
 // Indexing documents from the specified folder
 index.add(documentsFolder);
 
```

### ErrorOccurred {#ErrorOccurred}
```
public final Event<EventHandler<IndexErrorEventArgs>> ErrorOccurred
```


Occurs when an error happens during an index operation.

The example demonstrates how to use the event.

```

 String indexFolder = "c:\\MyIndex\\";
 String documentsFolder = "c:\\MyDocuments\\";
 String query = "Einstein";
 // Creating an index
 Index index = new Index(indexFolder);
 // Subscribing to the event
 index.getEvents().ErrorOccurred.add(new EventHandler() {
     public void invoke(Object sender, IndexErrorEventArgs args) {
         System.out.println(args.getMessage());
     }
 });
 // Indexing documents from the specified folder
 index.add(documentsFolder);
 // Searching in the index
 SearchResult result = index.search(query);
 
```

### OperationProgressChanged {#OperationProgressChanged}
```
public final Event<EventHandler<OperationProgressEventArgs>> OperationProgressChanged
```


Occurs when the progress of the indexing or update operation changes.

The example demonstrates how to use the event.

```

 String indexFolder = "c:\\MyIndex\\";
 String documentsFolder = "c:\\MyDocuments\\";
 // Creating an index
 Index index = new Index(indexFolder);
 // Subscribing to the event
 index.getEvents().OperationProgressChanged.add(new EventHandler() {
     public void invoke(Object sender, OperationProgressEventArgs args) {
         System.out.println("Last processed: " + args.getLastDocumentPath());
         System.out.println("Result: " + args.getLastDocumentStatus());
         System.out.println("Processed documents: " + args.getTotalDocuments());
         System.out.println("Progress percentage: " + args.getProgressPercentage());
     }
 });
 // Indexing documents from the specified folder
 index.add(documentsFolder);
 
```

### OptimizationProgressChanged {#OptimizationProgressChanged}
```
public final Event<EventHandler<OptimizationProgressEventArgs>> OptimizationProgressChanged
```


Occurs when the progress of the optimization operation changes.

### PasswordRequired {#PasswordRequired}
```
public final Event<EventHandler<PasswordRequiredEventArgs>> PasswordRequired
```


Occurs when a document requires password for opening.

The example demonstrates how to use the event.

```

 String indexFolder = "c:\\MyIndex\\";
 String documentsFolder = "c:\\MyDocuments\\";
 // Creating an index
 Index index = new Index(indexFolder);
 // Subscribing to the event
 index.getEvents().PasswordRequired.add(new EventHandler() {
     public void invoke(Object sender, PasswordRequiredEventArgs args) {
         if (args.getDocumentFullPath().endsWith("ProtectedDocument.pdf")) {
             args.setPassword("123456");
         }
     }
 });
 // Indexing documents from the specified folder
 index.add(documentsFolder);
 
```

### FileIndexing {#FileIndexing}
```
public final Event<EventHandler<FileIndexingEventArgs>> FileIndexing
```


Occurs when a document is going to be indexed.

The example demonstrates how to use the event.

```

 String indexFolder = "c:\\MyIndex\\";
 String documentsFolder = "c:\\MyDocuments\\";
 // Creating an index
 Index index = new Index(indexFolder);
 // Subscribing to the event
 index.getEvents().FileIndexing.add(new EventHandler() {
     public void invoke(Object sender, FileIndexingEventArgs args) {
         if (args.getDocumentFullPath().endsWith("Protected.pdf")) {
             args.setAdditionalFields(new DocumentField[] {
                 new DocumentField("Tags", "Protected")
             });
         }
         if (!args.getDocumentFullPath().toLowerCase().contains("important")) {
             args.setSkipIndexing(true);
         }
     }
 });
 // Indexing documents from the specified folder
 index.add(documentsFolder);
 
```

### ImagePreparing {#ImagePreparing}
```
public final Event<EventHandler<ImagePreparingEventArgs>> ImagePreparing
```


Occurs when an image is going to be prepared for indexing.

### StatusChanged {#StatusChanged}
```
public final Event<EventHandler<BaseIndexEventArgs>> StatusChanged
```


Occurs when the index status changes.

The example demonstrates how to use the event.

```

 String indexFolder = "c:\\MyIndex\\";
 String documentsFolder = "c:\\MyDocuments\\";
 // Creating an index
 Index index = new Index(indexFolder);
 // Subscribing to the event
 index.getEvents().StatusChanged.add(new EventHandler() {
     public void invoke(Object sender, BaseIndexEventArgs args) {
         if (args.getStatus() != IndexStatus.InProgress) {
             // A notification of the operation completion should be here
         }
     }
 });
 // Setting the flag for asynchronous indexing
 IndexingOptions options = new IndexingOptions();
 options.setAsync(true);
 // Asynchronous indexing documents from the specified folder
 // The method terminates before the operation completes
 index.add(documentsFolder, options);
 
```

### SearchPhaseCompleted {#SearchPhaseCompleted}
```
public final Event<EventHandler<SearchPhaseEventArgs>> SearchPhaseCompleted
```


Occurs when the search phase is completed.

The example demonstrates how to use the event.

```

 String indexFolder = "c:\\MyIndex\\";
 String documentsFolder = "c:\\MyDocuments\\";
 // Creating an index
 Index index = new Index(indexFolder);
 // Indexing documents from the specified folder
 index.add(documentsFolder);
 // Subscribing to the event
 index.getEvents().SearchPhaseCompleted.add(new EventHandler() {
     public void invoke(Object sender, SearchPhaseEventArgs args) {
         System.out.println("Search phase: " + args.getSearchPhase());
         System.out.println("Words: " + args.getWords().length);
     }
 });
 SearchOptions options = new SearchOptions();
 options.setUseSynonymSearch(true);
 options.setUseWordFormsSearch(true);
 options.getFuzzySearch().setEnabled(true);
 options.setUseHomophoneSearch(true);
 SearchResult result = index.search("Einstein", options);
 
```

