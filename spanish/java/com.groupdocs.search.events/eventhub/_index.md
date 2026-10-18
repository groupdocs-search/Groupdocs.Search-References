---
title: "EventHub"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Proporciona eventos de índice para suscribirse."
type: docs
weight: 12
url: /es/java/com.groupdocs.search.events/eventhub/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventHubBase](../../com.groupdocs.search.events/eventhubbase)
```
public abstract class EventHub extends EventHubBase
```

Proporciona eventos de índice para suscribirse.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)


El ejemplo muestra un uso típico de la clase.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
// Creando un índice
Index index = new Index(indexFolder);
// Suscribiéndose al evento
index.getEvents().ErrorOccurred.add(new EventHandler() {
public void invoke(Object sender, IndexErrorEventArgs args) {
System.out.println(args.getMessage());
}
});
// Indexando documentos de la carpeta especificada
index.add(documentsFolder);
// Buscando en el índice
SearchResult result = index.search(query);
 
```
 
````


## Constructores

| Constructor | Descripción |
| --- | --- |
| [EventHub()](#EventHub--) |  |
## Campos

| Campo | Descripción |
| --- | --- |
|  | [OperationFinished](#OperationFinished) | Ocurre cuando se finaliza una operación de índice. |
|
|  | [ErrorOccurred](#ErrorOccurred) | Ocurre cuando se produce un error durante una operación de índice. |
|
|  | [OperationProgressChanged](#OperationProgressChanged) | Ocurre cuando cambia el progreso de la operación de indexación o actualización. |
|
|  | [OptimizationProgressChanged](#OptimizationProgressChanged) | Ocurre cuando cambia el progreso de la operación de optimización. |
|
|  | [PasswordRequired](#PasswordRequired) | Ocurre cuando un documento requiere contraseña para abrirse. |
|
|  | [FileIndexing](#FileIndexing) | Ocurre cuando un documento va a ser indexado. |
|
|  | [ImagePreparing](#ImagePreparing) | Ocurre cuando una imagen está a punto de prepararse para indexarse. |
|
|  | [StatusChanged](#StatusChanged) | Ocurre cuando el estado del índice cambia. |
|
|  | [SearchPhaseCompleted](#SearchPhaseCompleted) | Ocurre cuando se completa la fase de búsqueda. |
|
### EventHub() {#EventHub--}
```
public EventHub()
```


### OperationFinished {#OperationFinished}
```
public final Event<EventHandler<OperationFinishedEventArgs>> OperationFinished
```


Ocurre cuando se finaliza una operación de índice.

El ejemplo muestra cómo usar el evento.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Creando un índice
Index index = new Index(indexFolder);
// Suscribiéndose al evento
index.getEvents().OperationFinished.add(new EventHandler() {
public void invoke(Object sender, OperationFinishedEventArgs args) {
System.out.println("Operation finished: " + args.getOperationType());
System.out.println("Mensaje: " + args.getMessage());
System.out.println("Carpeta de índice: " + args.getIndexFolder());
DateFormat df = new SimpleDateFormat("MM/dd/yyyy HH:mm:ss");
System.out.println("Hora: " + df.format(args.getTime()));
}
});
// Indexando documentos de la carpeta especificada
index.add(documentsFolder);
 
```
 
````



### ErrorOccurred {#ErrorOccurred}
```
public final Event<EventHandler<IndexErrorEventArgs>> ErrorOccurred
```


Ocurre cuando se produce un error durante una operación de índice.

El ejemplo muestra cómo usar el evento.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
// Creando un índice
Index index = new Index(indexFolder);
// Suscribiéndose al evento
index.getEvents().ErrorOccurred.add(new EventHandler() {
public void invoke(Object sender, IndexErrorEventArgs args) {
System.out.println(args.getMessage());
}
});
// Indexando documentos de la carpeta especificada
index.add(documentsFolder);
// Buscando en el índice
SearchResult result = index.search(query);
 
```
 
````



### OperationProgressChanged {#OperationProgressChanged}
```
public final Event<EventHandler<OperationProgressEventArgs>> OperationProgressChanged
```


Ocurre cuando cambia el progreso de la operación de indexación o actualización.

El ejemplo muestra cómo usar el evento.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Creando un índice
Index index = new Index(indexFolder);
// Suscribiéndose al evento
index.getEvents().OperationProgressChanged.add(new EventHandler() {
public void invoke(Object sender, OperationProgressEventArgs args) {
System.out.println("Último procesado: " + args.getLastDocumentPath());
System.out.println("Resultado: " + args.getLastDocumentStatus());
System.out.println("Documentos procesados: " + args.getTotalDocuments());
System.out.println("Porcentaje de progreso: " + args.getProgressPercentage());
}
});
// Indexando documentos de la carpeta especificada
index.add(documentsFolder);
 
```
 
````



### OptimizationProgressChanged {#OptimizationProgressChanged}
```
public final Event<EventHandler<OptimizationProgressEventArgs>> OptimizationProgressChanged
```


Ocurre cuando cambia el progreso de la operación de optimización.


### PasswordRequired {#PasswordRequired}
```
public final Event<EventHandler<PasswordRequiredEventArgs>> PasswordRequired
```


Ocurre cuando un documento requiere contraseña para abrirse.

El ejemplo muestra cómo usar el evento.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Creando un índice
Index index = new Index(indexFolder);
// Suscribiéndose al evento
index.getEvents().PasswordRequired.add(new EventHandler() {
public void invoke(Object sender, PasswordRequiredEventArgs args) {
if (args.getDocumentFullPath().endsWith("ProtectedDocument.pdf")) {
args.setPassword("123456");
}
}
});
// Indexando documentos de la carpeta especificada
index.add(documentsFolder);
 
```
 
````



### FileIndexing {#FileIndexing}
```
public final Event<EventHandler<FileIndexingEventArgs>> FileIndexing
```


Ocurre cuando un documento va a ser indexado.

El ejemplo muestra cómo usar el evento.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Creando un índice
Index index = new Index(indexFolder);
// Suscribiéndose al evento
index.getEvents().FileIndexing.add(new EventHandler() {
public void invoke(Object sender, FileIndexingEventArgs args) {
if (args.getDocumentFullPath().endsWith("Protected.pdf")) {
args.setAdditionalFields(new DocumentField[] {
new DocumentField("Etiquetas", "Protegido")
});
}
if (!args.getDocumentFullPath().toLowerCase().contains("importante")) {
args.setSkipIndexing(true);
}
}
});
// Indexando documentos de la carpeta especificada
index.add(documentsFolder);
 
```
 
````



### ImagePreparing {#ImagePreparing}
```
public final Event<EventHandler<ImagePreparingEventArgs>> ImagePreparing
```


Ocurre cuando una imagen está a punto de prepararse para indexarse.


### StatusChanged {#StatusChanged}
```
public final Event<EventHandler<BaseIndexEventArgs>> StatusChanged
```


Ocurre cuando el estado del índice cambia.

El ejemplo muestra cómo usar el evento.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Creando un índice
Index index = new Index(indexFolder);
// Suscribiéndose al evento
index.getEvents().StatusChanged.add(new EventHandler() {
public void invoke(Object sender, BaseIndexEventArgs args) {
if (args.getStatus() != IndexStatus.InProgress) {
// Se debería colocar una notificación de la finalización de la operación aquí
}
}
});
// Configurando la bandera para la indexación asíncrona
IndexingOptions options = new IndexingOptions();
options.setAsync(true);
// Indexación asíncrona de documentos desde la carpeta especificada
// El método termina antes de que la operación se complete
index.add(documentsFolder, options);
 
```
 
````



### SearchPhaseCompleted {#SearchPhaseCompleted}
```
public final Event<EventHandler<SearchPhaseEventArgs>> SearchPhaseCompleted
```


Ocurre cuando se completa la fase de búsqueda.

El ejemplo muestra cómo usar el evento.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Creando un índice
Index index = new Index(indexFolder);
// Indexando documentos de la carpeta especificada
index.add(documentsFolder);
// Suscribiéndose al evento
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



