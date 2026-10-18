---
title: "EventHub"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Stellt Indexereignisse zum Abonnieren bereit."
type: docs
weight: 12
url: /de/java/com.groupdocs.search.events/eventhub/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventHubBase](../../com.groupdocs.search.events/eventhubbase)
```
public abstract class EventHub extends EventHubBase
```

Stellt Indexereignisse zum Abonnieren bereit.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)


Das Beispiel demonstriert eine typische Verwendung der Klasse.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
// Erstellen eines Index
Index index = new Index(indexFolder);
// Abonnieren des Ereignisses
index.getEvents().ErrorOccurred.add(new EventHandler() {
public void invoke(Object sender, IndexErrorEventArgs args) {
System.out.println(args.getMessage());
}
});
// Indizieren von Dokumenten aus dem angegebenen Ordner
index.add(documentsFolder);
// Durchsuchen des Indexes
SearchResult result = index.search(query);
 
```
 
````


## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [EventHub()](#EventHub--) |  |
## Felder

| Feld | Beschreibung |
| --- | --- |
|  | [OperationFinished](#OperationFinished) | Tritt auf, wenn ein Indexvorgang abgeschlossen ist. |
|
|  | [ErrorOccurred](#ErrorOccurred) | Tritt auf, wenn während eines Indexvorgangs ein Fehler auftritt. |
|
|  | [OperationProgressChanged](#OperationProgressChanged) | Tritt auf, wenn sich der Fortschritt des Indexierungs- oder Aktualisierungsvorgangs ändert. |
|
|  | [OptimizationProgressChanged](#OptimizationProgressChanged) | Tritt auf, wenn sich der Fortschritt des Optimierungsvorgangs ändert. |
|
|  | [PasswordRequired](#PasswordRequired) | Tritt auf, wenn ein Dokument ein Passwort zum Öffnen benötigt. |
|
|  | [FileIndexing](#FileIndexing) | Tritt auf, wenn ein Dokument indiziert werden soll. |
|
|  | [ImagePreparing](#ImagePreparing) | Tritt auf, wenn ein Bild für die Indizierung vorbereitet wird. |
|
|  | [StatusChanged](#StatusChanged) | Tritt auf, wenn sich der Indexstatus ändert. |
|
|  | [SearchPhaseCompleted](#SearchPhaseCompleted) | Tritt auf, wenn die Suchphase abgeschlossen ist. |
|
### EventHub() {#EventHub--}
```
public EventHub()
```


### OperationFinished {#OperationFinished}
```
public final Event<EventHandler<OperationFinishedEventArgs>> OperationFinished
```


Tritt auf, wenn ein Indexvorgang abgeschlossen ist.

Das Beispiel zeigt, wie das Ereignis verwendet wird.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Erstellen eines Index
Index index = new Index(indexFolder);
// Abonnieren des Ereignisses
index.getEvents().OperationFinished.add(new EventHandler() {
public void invoke(Object sender, OperationFinishedEventArgs args) {
System.out.println("Operation finished: " + args.getOperationType());
System.out.println("Nachricht: " + args.getMessage());
System.out.println("Indexordner: " + args.getIndexFolder());
DateFormat df = new SimpleDateFormat("MM/dd/yyyy HH:mm:ss");
System.out.println("Zeit: " + df.format(args.getTime()));
}
});
// Indizieren von Dokumenten aus dem angegebenen Ordner
index.add(documentsFolder);
 
```
 
````



### ErrorOccurred {#ErrorOccurred}
```
public final Event<EventHandler<IndexErrorEventArgs>> ErrorOccurred
```


Tritt auf, wenn während eines Indexvorgangs ein Fehler auftritt.

Das Beispiel zeigt, wie das Ereignis verwendet wird.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
// Erstellen eines Index
Index index = new Index(indexFolder);
// Abonnieren des Ereignisses
index.getEvents().ErrorOccurred.add(new EventHandler() {
public void invoke(Object sender, IndexErrorEventArgs args) {
System.out.println(args.getMessage());
}
});
// Indizieren von Dokumenten aus dem angegebenen Ordner
index.add(documentsFolder);
// Durchsuchen des Indexes
SearchResult result = index.search(query);
 
```
 
````



### OperationProgressChanged {#OperationProgressChanged}
```
public final Event<EventHandler<OperationProgressEventArgs>> OperationProgressChanged
```


Tritt auf, wenn sich der Fortschritt des Indexierungs- oder Aktualisierungsvorgangs ändert.

Das Beispiel zeigt, wie das Ereignis verwendet wird.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Erstellen eines Index
Index index = new Index(indexFolder);
// Abonnieren des Ereignisses
index.getEvents().OperationProgressChanged.add(new EventHandler() {
public void invoke(Object sender, OperationProgressEventArgs args) {
System.out.println("Zuletzt verarbeitet: " + args.getLastDocumentPath());
System.out.println("Ergebnis: " + args.getLastDocumentStatus());
System.out.println("Verarbeitete Dokumente: " + args.getTotalDocuments());
System.out.println("Fortschritt in Prozent: " + args.getProgressPercentage());
}
});
// Indizieren von Dokumenten aus dem angegebenen Ordner
index.add(documentsFolder);
 
```
 
````



### OptimizationProgressChanged {#OptimizationProgressChanged}
```
public final Event<EventHandler<OptimizationProgressEventArgs>> OptimizationProgressChanged
```


Tritt auf, wenn sich der Fortschritt des Optimierungsvorgangs ändert.


### PasswordRequired {#PasswordRequired}
```
public final Event<EventHandler<PasswordRequiredEventArgs>> PasswordRequired
```


Tritt auf, wenn ein Dokument ein Passwort zum Öffnen benötigt.

Das Beispiel zeigt, wie das Ereignis verwendet wird.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Erstellen eines Index
Index index = new Index(indexFolder);
// Abonnieren des Ereignisses
index.getEvents().PasswordRequired.add(new EventHandler() {
public void invoke(Object sender, PasswordRequiredEventArgs args) {
if (args.getDocumentFullPath().endsWith("ProtectedDocument.pdf")) {
args.setPassword("123456");
}
}
});
// Indizieren von Dokumenten aus dem angegebenen Ordner
index.add(documentsFolder);
 
```
 
````



### FileIndexing {#FileIndexing}
```
public final Event<EventHandler<FileIndexingEventArgs>> FileIndexing
```


Tritt auf, wenn ein Dokument indiziert werden soll.

Das Beispiel zeigt, wie das Ereignis verwendet wird.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Erstellen eines Index
Index index = new Index(indexFolder);
// Abonnieren des Ereignisses
index.getEvents().FileIndexing.add(new EventHandler() {
public void invoke(Object sender, FileIndexingEventArgs args) {
if (args.getDocumentFullPath().endsWith("Protected.pdf")) {
args.setAdditionalFields(new DocumentField[] {
new DocumentField("Schlagwörter", "Geschützt")
});
}
if (!args.getDocumentFullPath().toLowerCase().contains("wichtig")) {
args.setSkipIndexing(true);
}
}
});
// Indizieren von Dokumenten aus dem angegebenen Ordner
index.add(documentsFolder);
 
```
 
````



### ImagePreparing {#ImagePreparing}
```
public final Event<EventHandler<ImagePreparingEventArgs>> ImagePreparing
```


Tritt auf, wenn ein Bild für die Indizierung vorbereitet wird.


### StatusChanged {#StatusChanged}
```
public final Event<EventHandler<BaseIndexEventArgs>> StatusChanged
```


Tritt auf, wenn sich der Indexstatus ändert.

Das Beispiel zeigt, wie das Ereignis verwendet wird.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Erstellen eines Index
Index index = new Index(indexFolder);
// Abonnieren des Ereignisses
index.getEvents().StatusChanged.add(new EventHandler() {
public void invoke(Object sender, BaseIndexEventArgs args) {
if (args.getStatus() != IndexStatus.InProgress) {
// Eine Benachrichtigung über den Abschluss der Operation sollte hier stehen
}
}
});
// Festlegen des Flags für asynchrones Indexieren
IndexingOptions options = new IndexingOptions();
options.setAsync(true);
// Asynchrones Indexieren von Dokumenten aus dem angegebenen Ordner
// Die Methode beendet sich, bevor der Vorgang abgeschlossen ist
index.add(documentsFolder, options);
 
```
 
````



### SearchPhaseCompleted {#SearchPhaseCompleted}
```
public final Event<EventHandler<SearchPhaseEventArgs>> SearchPhaseCompleted
```


Tritt auf, wenn die Suchphase abgeschlossen ist.

Das Beispiel zeigt, wie das Ereignis verwendet wird.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Erstellen eines Index
Index index = new Index(indexFolder);
// Indizieren von Dokumenten aus dem angegebenen Ordner
index.add(documentsFolder);
// Abonnieren des Ereignisses
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
SearchResult result = index.search(\"Einstein\", options);
 
```
 
````



