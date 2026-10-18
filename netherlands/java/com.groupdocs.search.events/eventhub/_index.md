---
title: "EventHub"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Biedt indexgebeurtenissen om op te abonneren."
type: docs
weight: 12
url: /nl/java/com.groupdocs.search.events/eventhub/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventHubBase](../../com.groupdocs.search.events/eventhubbase)
```
public abstract class EventHub extends EventHubBase
```

Biedt indexgebeurtenissen om op te abonneren.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)


Het voorbeeld toont een typisch gebruik van de klasse.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
// Een index maken
Index index = new Index(indexFolder);
// Abonneren op het evenement
index.getEvents().ErrorOccurred.add(new EventHandler() {
public void invoke(Object sender, IndexErrorEventArgs args) {
System.out.println(args.getMessage());
}
});
// Documenten indexeren vanuit de opgegeven map
index.add(documentsFolder);
// Zoeken in de index
SearchResult result = index.search(query);
 
```
 
````


## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [EventHub()](#EventHub--) |  |
## Velden

| Veld | Beschrijving |
| --- | --- |
|  | [OperationFinished](#OperationFinished) | Vindt plaats wanneer een indexbewerking is voltooid. |
|
|  | [ErrorOccurred](#ErrorOccurred) | Vindt plaats wanneer er een fout optreedt tijdens een indexbewerking. |
|
|  | [OperationProgressChanged](#OperationProgressChanged) | Vindt plaats wanneer de voortgang van de indexerings- of updatebewerking verandert. |
|
|  | [OptimizationProgressChanged](#OptimizationProgressChanged) | Vindt plaats wanneer de voortgang van de optimalisatiebewerking verandert. |
|
|  | [PasswordRequired](#PasswordRequired) | Treedt op wanneer een document een wachtwoord vereist om te openen. |
|
|  | [FileIndexing](#FileIndexing) | Vindt plaats wanneer een document zal worden geïndexeerd. |
|
|  | [ImagePreparing](#ImagePreparing) | Treedt op wanneer een afbeelding wordt voorbereid voor indexering. |
|
|  | [StatusChanged](#StatusChanged) | Vindt plaats wanneer de status van de index verandert. |
|
|  | [SearchPhaseCompleted](#SearchPhaseCompleted) | Vindt plaats wanneer de zoekfase is voltooid. |
|
### EventHub() {#EventHub--}
```
public EventHub()
```


### OperationFinished {#OperationFinished}
```
public final Event<EventHandler<OperationFinishedEventArgs>> OperationFinished
```


Vindt plaats wanneer een indexbewerking is voltooid.

Het voorbeeld toont hoe het evenement gebruikt kan worden.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Een index maken
Index index = new Index(indexFolder);
// Abonneren op het evenement
index.getEvents().OperationFinished.add(new EventHandler() {
public void invoke(Object sender, OperationFinishedEventArgs args) {
System.out.println("Operation finished: " + args.getOperationType());
System.out.println("Bericht: " + args.getMessage());
System.out.println("Indexmap: " + args.getIndexFolder());
DateFormat df = new SimpleDateFormat("MM/dd/yyyy HH:mm:ss");
System.out.println("Tijd: " + df.format(args.getTime()));
}
});
// Documenten indexeren vanuit de opgegeven map
index.add(documentsFolder);
 
```
 
````



### ErrorOccurred {#ErrorOccurred}
```
public final Event<EventHandler<IndexErrorEventArgs>> ErrorOccurred
```


Vindt plaats wanneer er een fout optreedt tijdens een indexbewerking.

Het voorbeeld toont hoe het evenement gebruikt kan worden.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
// Een index maken
Index index = new Index(indexFolder);
// Abonneren op het evenement
index.getEvents().ErrorOccurred.add(new EventHandler() {
public void invoke(Object sender, IndexErrorEventArgs args) {
System.out.println(args.getMessage());
}
});
// Documenten indexeren vanuit de opgegeven map
index.add(documentsFolder);
// Zoeken in de index
SearchResult result = index.search(query);
 
```
 
````



### OperationProgressChanged {#OperationProgressChanged}
```
public final Event<EventHandler<OperationProgressEventArgs>> OperationProgressChanged
```


Vindt plaats wanneer de voortgang van de indexerings- of updatebewerking verandert.

Het voorbeeld toont hoe het evenement gebruikt kan worden.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Een index maken
Index index = new Index(indexFolder);
// Abonneren op het evenement
index.getEvents().OperationProgressChanged.add(new EventHandler() {
public void invoke(Object sender, OperationProgressEventArgs args) {
System.out.println("Laatst verwerkt: " + args.getLastDocumentPath());
System.out.println("Resultaat: " + args.getLastDocumentStatus());
System.out.println("Verwerkte documenten: " + args.getTotalDocuments());
System.out.println("Voortgangspercentage: " + args.getProgressPercentage());
}
});
// Documenten indexeren vanuit de opgegeven map
index.add(documentsFolder);
 
```
 
````



### OptimizationProgressChanged {#OptimizationProgressChanged}
```
public final Event<EventHandler<OptimizationProgressEventArgs>> OptimizationProgressChanged
```


Vindt plaats wanneer de voortgang van de optimalisatiebewerking verandert.


### PasswordRequired {#PasswordRequired}
```
public final Event<EventHandler<PasswordRequiredEventArgs>> PasswordRequired
```


Treedt op wanneer een document een wachtwoord vereist om te openen.

Het voorbeeld toont hoe het evenement gebruikt kan worden.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Een index maken
Index index = new Index(indexFolder);
// Abonneren op het evenement
index.getEvents().PasswordRequired.add(new EventHandler() {
public void invoke(Object sender, PasswordRequiredEventArgs args) {
if (args.getDocumentFullPath().endsWith("ProtectedDocument.pdf")) {
args.setPassword("123456");
}
}
});
// Documenten indexeren vanuit de opgegeven map
index.add(documentsFolder);
 
```
 
````



### FileIndexing {#FileIndexing}
```
public final Event<EventHandler<FileIndexingEventArgs>> FileIndexing
```


Vindt plaats wanneer een document zal worden geïndexeerd.

Het voorbeeld toont hoe het evenement gebruikt kan worden.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Een index maken
Index index = new Index(indexFolder);
// Abonneren op het evenement
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
// Documenten indexeren vanuit de opgegeven map
index.add(documentsFolder);
 
```
 
````



### ImagePreparing {#ImagePreparing}
```
public final Event<EventHandler<ImagePreparingEventArgs>> ImagePreparing
```


Treedt op wanneer een afbeelding wordt voorbereid voor indexering.


### StatusChanged {#StatusChanged}
```
public final Event<EventHandler<BaseIndexEventArgs>> StatusChanged
```


Vindt plaats wanneer de status van de index verandert.

Het voorbeeld toont hoe het evenement gebruikt kan worden.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Een index maken
Index index = new Index(indexFolder);
// Abonneren op het evenement
index.getEvents().StatusChanged.add(new EventHandler() {
public void invoke(Object sender, BaseIndexEventArgs args) {
if (args.getStatus() != IndexStatus.InProgress) {
// Een melding van de voltooiing van de bewerking moet hier staan
}
}
});
// Instellen van de vlag voor asynchrone indexering
IndexingOptions options = new IndexingOptions();
options.setAsync(true);
// Asynchrone indexering van documenten uit de opgegeven map
// De methode beëindigt voordat de bewerking voltooid is
index.add(documentsFolder, options);
 
```
 
````



### SearchPhaseCompleted {#SearchPhaseCompleted}
```
public final Event<EventHandler<SearchPhaseEventArgs>> SearchPhaseCompleted
```


Vindt plaats wanneer de zoekfase is voltooid.

Het voorbeeld toont hoe het evenement gebruikt kan worden.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Een index maken
Index index = new Index(indexFolder);
// Documenten indexeren vanuit de opgegeven map
index.add(documentsFolder);
// Abonneren op het evenement
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
 
````



