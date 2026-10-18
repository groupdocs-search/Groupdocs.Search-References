---
title: "EventHub"
second_title: "GroupDocs.Search för Java API-referens"
description: "Tillhandahåller indexhändelser för prenumeration."
type: docs
weight: 12
url: /sv/java/com.groupdocs.search.events/eventhub/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventHubBase](../../com.groupdocs.search.events/eventhubbase)
```
public abstract class EventHub extends EventHubBase
```

Tillhandahåller indexhändelser för prenumeration.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)


Exemplet demonstrerar ett typiskt användningssätt av klassen.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
// Skapar ett index
Index index = new Index(indexFolder);
// Prenumererar på händelsen
index.getEvents().ErrorOccurred.add(new EventHandler() {
public void invoke(Object sender, IndexErrorEventArgs args) {
System.out.println(args.getMessage());
}
});
// Indexerar dokument från den angivna mappen
index.add(documentsFolder);
// Söker i indexet
SearchResult result = index.search(query);
 
```
 
````


## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [EventHub()](#EventHub--) |  |
## Fält

| Fält | Beskrivning |
| --- | --- |
|  | [OperationFinished](#OperationFinished) | Inträffar när en indexoperation är klar. |
|
|  | [ErrorOccurred](#ErrorOccurred) | Inträffar när ett fel uppstår under en indexoperation. |
|
|  | [OperationProgressChanged](#OperationProgressChanged) | Inträffar när framstegen för indexering eller uppdateringsoperationen ändras. |
|
|  | [OptimizationProgressChanged](#OptimizationProgressChanged) | Inträffar när framstegen för optimeringsoperationen ändras. |
|
|  | [PasswordRequired](#PasswordRequired) | Uppstår när ett dokument kräver lösenord för att öppnas. |
|
|  | [FileIndexing](#FileIndexing) | Inträffar när ett dokument ska indexeras. |
|
|  | [ImagePreparing](#ImagePreparing) | Uppstår när en bild ska förberedas för indexering. |
|
|  | [StatusChanged](#StatusChanged) | Inträffar när indexstatusen ändras. |
|
|  | [SearchPhaseCompleted](#SearchPhaseCompleted) | Inträffar när sökfasen är slutförd. |
|
### EventHub() {#EventHub--}
```
public EventHub()
```


### OperationFinished {#OperationFinished}
```
public final Event<EventHandler<OperationFinishedEventArgs>> OperationFinished
```


Inträffar när en indexoperation är klar.

Exemplet visar hur man använder händelsen.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Skapar ett index
Index index = new Index(indexFolder);
// Prenumererar på händelsen
index.getEvents().OperationFinished.add(new EventHandler() {
public void invoke(Object sender, OperationFinishedEventArgs args) {
System.out.println("Operation finished: " + args.getOperationType());
System.out.println("Meddelande: " + args.getMessage());
System.out.println("Indexmapp: " + args.getIndexFolder());
DateFormat df = new SimpleDateFormat("MM/dd/yyyy HH:mm:ss");
System.out.println("Tid: " + df.format(args.getTime()));
}
});
// Indexerar dokument från den angivna mappen
index.add(documentsFolder);
 
```
 
````



### ErrorOccurred {#ErrorOccurred}
```
public final Event<EventHandler<IndexErrorEventArgs>> ErrorOccurred
```


Inträffar när ett fel uppstår under en indexoperation.

Exemplet visar hur man använder händelsen.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
// Skapar ett index
Index index = new Index(indexFolder);
// Prenumererar på händelsen
index.getEvents().ErrorOccurred.add(new EventHandler() {
public void invoke(Object sender, IndexErrorEventArgs args) {
System.out.println(args.getMessage());
}
});
// Indexerar dokument från den angivna mappen
index.add(documentsFolder);
// Söker i indexet
SearchResult result = index.search(query);
 
```
 
````



### OperationProgressChanged {#OperationProgressChanged}
```
public final Event<EventHandler<OperationProgressEventArgs>> OperationProgressChanged
```


Inträffar när framstegen för indexering eller uppdateringsoperationen ändras.

Exemplet visar hur man använder händelsen.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Skapar ett index
Index index = new Index(indexFolder);
// Prenumererar på händelsen
index.getEvents().OperationProgressChanged.add(new EventHandler() {
public void invoke(Object sender, OperationProgressEventArgs args) {
System.out.println("Senast bearbetad: " + args.getLastDocumentPath());
System.out.println("Resultat: " + args.getLastDocumentStatus());
System.out.println("Bearbetade dokument: " + args.getTotalDocuments());
System.out.println("Framsteg i procent: " + args.getProgressPercentage());
}
});
// Indexerar dokument från den angivna mappen
index.add(documentsFolder);
 
```
 
````



### OptimizationProgressChanged {#OptimizationProgressChanged}
```
public final Event<EventHandler<OptimizationProgressEventArgs>> OptimizationProgressChanged
```


Inträffar när framstegen för optimeringsoperationen ändras.


### PasswordRequired {#PasswordRequired}
```
public final Event<EventHandler<PasswordRequiredEventArgs>> PasswordRequired
```


Uppstår när ett dokument kräver lösenord för att öppnas.

Exemplet visar hur man använder händelsen.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Skapar ett index
Index index = new Index(indexFolder);
// Prenumererar på händelsen
index.getEvents().PasswordRequired.add(new EventHandler() {
public void invoke(Object sender, PasswordRequiredEventArgs args) {
if (args.getDocumentFullPath().endsWith("ProtectedDocument.pdf")) {
args.setPassword("123456");
}
}
});
// Indexerar dokument från den angivna mappen
index.add(documentsFolder);
 
```
 
````



### FileIndexing {#FileIndexing}
```
public final Event<EventHandler<FileIndexingEventArgs>> FileIndexing
```


Inträffar när ett dokument ska indexeras.

Exemplet visar hur man använder händelsen.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Skapar ett index
Index index = new Index(indexFolder);
// Prenumererar på händelsen
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
// Indexerar dokument från den angivna mappen
index.add(documentsFolder);
 
```
 
````



### ImagePreparing {#ImagePreparing}
```
public final Event<EventHandler<ImagePreparingEventArgs>> ImagePreparing
```


Uppstår när en bild ska förberedas för indexering.


### StatusChanged {#StatusChanged}
```
public final Event<EventHandler<BaseIndexEventArgs>> StatusChanged
```


Inträffar när indexstatusen ändras.

Exemplet visar hur man använder händelsen.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Skapar ett index
Index index = new Index(indexFolder);
// Prenumererar på händelsen
index.getEvents().StatusChanged.add(new EventHandler() {
public void invoke(Object sender, BaseIndexEventArgs args) {
if (args.getStatus() != IndexStatus.InProgress) {
// En notifikation om operationens slutförande bör vara här
}
}
});
// Ställer in flaggan för asynkron indexering
IndexingOptions options = new IndexingOptions();
options.setAsync(true);
// Asynkron indexering av dokument från den angivna mappen
// Metoden avslutas innan operationen slutförs
index.add(documentsFolder, options);
 
```
 
````



### SearchPhaseCompleted {#SearchPhaseCompleted}
```
public final Event<EventHandler<SearchPhaseEventArgs>> SearchPhaseCompleted
```


Inträffar när sökfasen är slutförd.

Exemplet visar hur man använder händelsen.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Skapar ett index
Index index = new Index(indexFolder);
// Indexerar dokument från den angivna mappen
index.add(documentsFolder);
// Prenumererar på händelsen
index.getEvents().SearchPhaseCompleted.add(new EventHandler() {
public void invoke(Object sender, SearchPhaseEventArgs args) {
System.out.println("Sökfas: " + args.getSearchPhase());
System.out.println("Ord: " + args.getWords().length);
}
});
SearchOptions options = new SearchOptions();
options.setUseSynonymSearch(true);
options.setUseWordFormsSearch(true);
options.getFuzzySearch().setEnabled(true);
options.setUseHomophoneSearch(true);
SearchResult result = index.search("Einstein", options);
 
```
 
````



