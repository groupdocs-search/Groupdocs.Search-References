---
title: "EventHub"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Fornisce eventi dell'indice per l'iscrizione."
type: docs
weight: 12
url: /it/java/com.groupdocs.search.events/eventhub/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventHubBase](../../com.groupdocs.search.events/eventhubbase)
```
public abstract class EventHub extends EventHubBase
```

Fornisce eventi dell'indice per l'iscrizione.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)


L'esempio dimostra un utilizzo tipico della classe.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
// Creazione di un indice
Index index = new Index(indexFolder);
// Sottoscrizione all'evento
index.getEvents().ErrorOccurred.add(new EventHandler() {
public void invoke(Object sender, IndexErrorEventArgs args) {
System.out.println(args.getMessage());
}
});
// Indicizzazione dei documenti dalla cartella specificata
index.add(documentsFolder);
// Ricerca nell'indice
SearchResult result = index.search(query);
 
```
 
````


## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [EventHub()](#EventHub--) |  |
## Fields

| Field | Descrizione |
| --- | --- |
|  | [OperationFinished](#OperationFinished) | Si verifica quando un'operazione di indicizzazione è terminata. |
|
|  | [ErrorOccurred](#ErrorOccurred) | Si verifica quando si verifica un errore durante un'operazione di indicizzazione. |
|
|  | [OperationProgressChanged](#OperationProgressChanged) | Si verifica quando il progresso dell'operazione di indicizzazione o aggiornamento cambia. |
|
|  | [OptimizationProgressChanged](#OptimizationProgressChanged) | Si verifica quando il progresso dell'operazione di ottimizzazione cambia. |
|
|  | [PasswordRequired](#PasswordRequired) | Si verifica quando un documento richiede una password per l'apertura. |
|
|  | [FileIndexing](#FileIndexing) | Si verifica quando un documento sta per essere indicizzato. |
|
|  | [ImagePreparing](#ImagePreparing) | Si verifica quando un'immagine sta per essere preparata per l'indicizzazione. |
|
|  | [StatusChanged](#StatusChanged) | Si verifica quando lo stato dell'indice cambia. |
|
|  | [SearchPhaseCompleted](#SearchPhaseCompleted) | Si verifica quando la fase di ricerca è completata. |
|
### EventHub() {#EventHub--}
```
public EventHub()
```


### OperationFinished {#OperationFinished}
```
public final Event<EventHandler<OperationFinishedEventArgs>> OperationFinished
```


Si verifica quando un'operazione di indicizzazione è terminata.

L'esempio dimostra come utilizzare l'evento.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Creazione di un indice
Index index = new Index(indexFolder);
// Sottoscrizione all'evento
index.getEvents().OperationFinished.add(new EventHandler() {
public void invoke(Object sender, OperationFinishedEventArgs args) {
System.out.println("Operation finished: " + args.getOperationType());
System.out.println("Messaggio: " + args.getMessage());
System.out.println("Cartella indice: " + args.getIndexFolder());
DateFormat df = new SimpleDateFormat("MM/dd/yyyy HH:mm:ss");
System.out.println("Ora: " + df.format(args.getTime()));
}
});
// Indicizzazione dei documenti dalla cartella specificata
index.add(documentsFolder);
 
```
 
````



### ErrorOccurred {#ErrorOccurred}
```
public final Event<EventHandler<IndexErrorEventArgs>> ErrorOccurred
```


Si verifica quando si verifica un errore durante un'operazione di indicizzazione.

L'esempio dimostra come utilizzare l'evento.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
// Creazione di un indice
Index index = new Index(indexFolder);
// Sottoscrizione all'evento
index.getEvents().ErrorOccurred.add(new EventHandler() {
public void invoke(Object sender, IndexErrorEventArgs args) {
System.out.println(args.getMessage());
}
});
// Indicizzazione dei documenti dalla cartella specificata
index.add(documentsFolder);
// Ricerca nell'indice
SearchResult result = index.search(query);
 
```
 
````



### OperationProgressChanged {#OperationProgressChanged}
```
public final Event<EventHandler<OperationProgressEventArgs>> OperationProgressChanged
```


Si verifica quando il progresso dell'operazione di indicizzazione o aggiornamento cambia.

L'esempio dimostra come utilizzare l'evento.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Creazione di un indice
Index index = new Index(indexFolder);
// Sottoscrizione all'evento
index.getEvents().OperationProgressChanged.add(new EventHandler() {
public void invoke(Object sender, OperationProgressEventArgs args) {
System.out.println("Ultimo elaborato: " + args.getLastDocumentPath());
System.out.println("Risultato: " + args.getLastDocumentStatus());
System.out.println("Documenti elaborati: " + args.getTotalDocuments());
System.out.println("Percentuale di avanzamento: " + args.getProgressPercentage());
}
});
// Indicizzazione dei documenti dalla cartella specificata
index.add(documentsFolder);
 
```
 
````



### OptimizationProgressChanged {#OptimizationProgressChanged}
```
public final Event<EventHandler<OptimizationProgressEventArgs>> OptimizationProgressChanged
```


Si verifica quando il progresso dell'operazione di ottimizzazione cambia.


### PasswordRequired {#PasswordRequired}
```
public final Event<EventHandler<PasswordRequiredEventArgs>> PasswordRequired
```


Si verifica quando un documento richiede una password per l'apertura.

L'esempio dimostra come utilizzare l'evento.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Creazione di un indice
Index index = new Index(indexFolder);
// Sottoscrizione all'evento
index.getEvents().PasswordRequired.add(new EventHandler() {
public void invoke(Object sender, PasswordRequiredEventArgs args) {
if (args.getDocumentFullPath().endsWith("ProtectedDocument.pdf")) {
args.setPassword("123456");
}
}
});
// Indicizzazione dei documenti dalla cartella specificata
index.add(documentsFolder);
 
```
 
````



### FileIndexing {#FileIndexing}
```
public final Event<EventHandler<FileIndexingEventArgs>> FileIndexing
```


Si verifica quando un documento sta per essere indicizzato.

L'esempio dimostra come utilizzare l'evento.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Creazione di un indice
Index index = new Index(indexFolder);
// Sottoscrizione all'evento
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
// Indicizzazione dei documenti dalla cartella specificata
index.add(documentsFolder);
 
```
 
````



### ImagePreparing {#ImagePreparing}
```
public final Event<EventHandler<ImagePreparingEventArgs>> ImagePreparing
```


Si verifica quando un'immagine sta per essere preparata per l'indicizzazione.


### StatusChanged {#StatusChanged}
```
public final Event<EventHandler<BaseIndexEventArgs>> StatusChanged
```


Si verifica quando lo stato dell'indice cambia.

L'esempio dimostra come utilizzare l'evento.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Creazione di un indice
Index index = new Index(indexFolder);
// Sottoscrizione all'evento
index.getEvents().StatusChanged.add(new EventHandler() {
public void invoke(Object sender, BaseIndexEventArgs args) {
if (args.getStatus() != IndexStatus.InProgress) {
// Una notifica del completamento dell'operazione dovrebbe trovarsi qui
}
}
});
// Impostazione del flag per l'indicizzazione asincrona
IndexingOptions options = new IndexingOptions();
options.setAsync(true);
// Indicizzazione asincrona dei documenti dalla cartella specificata
// Il metodo termina prima che l'operazione sia completata
index.add(documentsFolder, options);
 
```
 
````



### SearchPhaseCompleted {#SearchPhaseCompleted}
```
public final Event<EventHandler<SearchPhaseEventArgs>> SearchPhaseCompleted
```


Si verifica quando la fase di ricerca è completata.

L'esempio dimostra come utilizzare l'evento.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Creazione di un indice
Index index = new Index(indexFolder);
// Indicizzazione dei documenti dalla cartella specificata
index.add(documentsFolder);
// Sottoscrizione all'evento
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



