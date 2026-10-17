---
title: "EventHub"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Fournit des événements d'index pour l'abonnement."
type: docs
weight: 12
url: /fr/java/com.groupdocs.search.events/eventhub/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventHubBase](../../com.groupdocs.search.events/eventhubbase)
```
public abstract class EventHub extends EventHubBase
```

Fournit des événements d'index pour l'abonnement.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)


L'exemple montre une utilisation typique de la classe.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
// Création d'un index
Index index = new Index(indexFolder);
// Souscription à l'événement
index.getEvents().ErrorOccurred.add(new EventHandler() {
public void invoke(Object sender, IndexErrorEventArgs args) {
System.out.println(args.getMessage());
}
});
// Indexation des documents du dossier spécifié
index.add(documentsFolder);
// Recherche dans l'index
SearchResult result = index.search(query);
 
```
 
````


## Constructeurs

| Constructeur | Description |
| --- | --- |
| [EventHub()](#EventHub--) |  |
## Fields

| Field | Description |
| --- | --- |
|  | [OperationFinished](#OperationFinished) | Se produit lorsqu'une opération d'indexation est terminée. |
|
|  | [ErrorOccurred](#ErrorOccurred) | Se produit lorsqu'une erreur survient lors d'une opération d'indexation. |
|
|  | [OperationProgressChanged](#OperationProgressChanged) | Se produit lorsque la progression de l'opération d'indexation ou de mise à jour change. |
|
|  | [OptimizationProgressChanged](#OptimizationProgressChanged) | Se produit lorsque la progression de l'opération d'optimisation change. |
|
|  | [PasswordRequired](#PasswordRequired) | Se produit lorsqu'un document nécessite un mot de passe pour être ouvert. |
|
|  | [FileIndexing](#FileIndexing) | Se produit lorsqu'un document va être indexé. |
|
|  | [ImagePreparing](#ImagePreparing) | Se produit lorsqu'une image doit être préparée pour l'indexation. |
|
|  | [StatusChanged](#StatusChanged) | Se produit lorsque l'état de l'index change. |
|
|  | [SearchPhaseCompleted](#SearchPhaseCompleted) | Se produit lorsque la phase de recherche est terminée. |
|
### EventHub() {#EventHub--}
```
public EventHub()
```


### OperationFinished {#OperationFinished}
```
public final Event<EventHandler<OperationFinishedEventArgs>> OperationFinished
```


Se produit lorsqu'une opération d'indexation est terminée.

L'exemple montre comment utiliser l'événement.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Création d'un index
Index index = new Index(indexFolder);
// Souscription à l'événement
index.getEvents().OperationFinished.add(new EventHandler() {
public void invoke(Object sender, OperationFinishedEventArgs args) {
System.out.println("Operation finished: " + args.getOperationType());
System.out.println("Message : " + args.getMessage());
System.out.println("Dossier d'index : " + args.getIndexFolder());
DateFormat df = new SimpleDateFormat("MM/dd/yyyy HH:mm:ss");
System.out.println("Heure : " + df.format(args.getTime()));
}
});
// Indexation des documents du dossier spécifié
index.add(documentsFolder);
 
```
 
````



### ErrorOccurred {#ErrorOccurred}
```
public final Event<EventHandler<IndexErrorEventArgs>> ErrorOccurred
```


Se produit lorsqu'une erreur survient lors d'une opération d'indexation.

L'exemple montre comment utiliser l'événement.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
// Création d'un index
Index index = new Index(indexFolder);
// Souscription à l'événement
index.getEvents().ErrorOccurred.add(new EventHandler() {
public void invoke(Object sender, IndexErrorEventArgs args) {
System.out.println(args.getMessage());
}
});
// Indexation des documents du dossier spécifié
index.add(documentsFolder);
// Recherche dans l'index
SearchResult result = index.search(query);
 
```
 
````



### OperationProgressChanged {#OperationProgressChanged}
```
public final Event<EventHandler<OperationProgressEventArgs>> OperationProgressChanged
```


Se produit lorsque la progression de l'opération d'indexation ou de mise à jour change.

L'exemple montre comment utiliser l'événement.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Création d'un index
Index index = new Index(indexFolder);
// Souscription à l'événement
index.getEvents().OperationProgressChanged.add(new EventHandler() {
public void invoke(Object sender, OperationProgressEventArgs args) {
System.out.println("Dernier traité : " + args.getLastDocumentPath());
System.out.println("Résultat : " + args.getLastDocumentStatus());
System.out.println("Documents traités : " + args.getTotalDocuments());
System.out.println("Pourcentage de progression : " + args.getProgressPercentage());
}
});
// Indexation des documents du dossier spécifié
index.add(documentsFolder);
 
```
 
````



### OptimizationProgressChanged {#OptimizationProgressChanged}
```
public final Event<EventHandler<OptimizationProgressEventArgs>> OptimizationProgressChanged
```


Se produit lorsque la progression de l'opération d'optimisation change.


### PasswordRequired {#PasswordRequired}
```
public final Event<EventHandler<PasswordRequiredEventArgs>> PasswordRequired
```


Se produit lorsqu'un document nécessite un mot de passe pour être ouvert.

L'exemple montre comment utiliser l'événement.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Création d'un index
Index index = new Index(indexFolder);
// Souscription à l'événement
index.getEvents().PasswordRequired.add(new EventHandler() {
public void invoke(Object sender, PasswordRequiredEventArgs args) {
if (args.getDocumentFullPath().endsWith("ProtectedDocument.pdf")) {
args.setPassword("123456");
}
}
});
// Indexation des documents du dossier spécifié
index.add(documentsFolder);
 
```
 
````



### FileIndexing {#FileIndexing}
```
public final Event<EventHandler<FileIndexingEventArgs>> FileIndexing
```


Se produit lorsqu'un document va être indexé.

L'exemple montre comment utiliser l'événement.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Création d'un index
Index index = new Index(indexFolder);
// Souscription à l'événement
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
// Indexation des documents du dossier spécifié
index.add(documentsFolder);
 
```
 
````



### ImagePreparing {#ImagePreparing}
```
public final Event<EventHandler<ImagePreparingEventArgs>> ImagePreparing
```


Se produit lorsqu'une image doit être préparée pour l'indexation.


### StatusChanged {#StatusChanged}
```
public final Event<EventHandler<BaseIndexEventArgs>> StatusChanged
```


Se produit lorsque l'état de l'index change.

L'exemple montre comment utiliser l'événement.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Création d'un index
Index index = new Index(indexFolder);
// Souscription à l'événement
index.getEvents().StatusChanged.add(new EventHandler() {
public void invoke(Object sender, BaseIndexEventArgs args) {
if (args.getStatus() != IndexStatus.InProgress) {
// Une notification de la fin de l'opération devrait être ici
}
}
});
// Définition du drapeau pour l'indexation asynchrone
IndexingOptions options = new IndexingOptions();
options.setAsync(true);
// Indexation asynchrone des documents depuis le dossier spécifié
// La méthode se termine avant que l'opération ne soit terminée
index.add(documentsFolder, options);
 
```
 
````



### SearchPhaseCompleted {#SearchPhaseCompleted}
```
public final Event<EventHandler<SearchPhaseEventArgs>> SearchPhaseCompleted
```


Se produit lorsque la phase de recherche est terminée.

L'exemple montre comment utiliser l'événement.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Création d'un index
Index index = new Index(indexFolder);
// Indexation des documents du dossier spécifié
index.add(documentsFolder);
// Souscription à l'événement
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



