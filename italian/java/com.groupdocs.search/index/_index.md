---
title: "Index"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Rappresenta la classe principale per l'indicizzazione dei documenti e la ricerca al loro interno."
type: docs
weight: 17
url: /it/java/com.groupdocs.search/index/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.io.Closeable
```
public class Index implements Closeable
```

Rappresenta la classe principale per l'indicizzazione dei documenti e la ricerca al loro interno.


**Learn more**

* [Creating an index](../https://docs.groupdocs.com/display/searchjava/Creating+an+index)
* [Indexing](../https://docs.groupdocs.com/display/searchjava/Indexing)
* [Searching](../https://docs.groupdocs.com/display/searchjava/Searching)


L'esempio dimostra un utilizzo tipico della classe.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // Creazione dell'indice nella cartella specificata
index.add(documentsFolder); // Indicizzazione dei documenti dalla cartella specificata
SearchResult result = index.search(query); // Ricerca nell'indice
 
```
 
````


## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [Index()](#Index--) | Inizializza una nuova istanza della classe  Index  in memoria. |
|
|  | [Index(IndexSettings settings)](#Index-com.groupdocs.search.IndexSettings-) | Inizializza una nuova istanza della classe  Index  in memoria con impostazioni dell'indice specifiche. |
|
|  | [Index(String indexFolder)](#Index-java.lang.String-) | Inizializza una nuova istanza della classe  Index  . |
|
|  | [Index(String indexFolder, IndexSettings settings)](#Index-java.lang.String-com.groupdocs.search.IndexSettings-) | Inizializza una nuova istanza di |
Index
classe.
|
|  | [Index(String indexFolder, boolean overwriteIfExists)](#Index-java.lang.String-boolean-) | Inizializza una nuova istanza di |
Index
classe.
|
|  | [Index(String indexFolder, IndexSettings settings, boolean overwriteIfExists)](#Index-java.lang.String-com.groupdocs.search.IndexSettings-boolean-) | Inizializza una nuova istanza di |
Index
classe.
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getEvents()](#getEvents--) | Ottiene il hub degli eventi per iscriversi agli eventi. |
|
|  | [getIndexInfo()](#getIndexInfo--) | Ottiene le informazioni di base sull'indice. |
|
|  | [getRepository()](#getRepository--) | Ottiene l'oggetto repository dell'indice se l'indice è contenuto in esso. |
|
|  | [getIndexSettings()](#getIndexSettings--) | Ottiene le impostazioni dell'indice. |
|
|  | [getDictionaries()](#getDictionaries--) | Ottiene il repository del dizionario. |
|
|  | [close()](#close--) | Rilascia tutte le risorse utilizzate da |
Index
.
|
|  | [add(String path)](#add-java.lang.String-) | Esegue l'operazione di indicizzazione. |
|
|  | [add(String path, IndexingOptions options)](#add-java.lang.String-com.groupdocs.search.options.IndexingOptions-) | Esegue l'operazione di indicizzazione. |
|
|  | [add(String[] paths)](#add-java.lang.String---) | Esegue l'operazione di indicizzazione. |
|
|  | [add(String[] paths, IndexingOptions options)](#add-java.lang.String---com.groupdocs.search.options.IndexingOptions-) | Esegue l'operazione di indicizzazione. |
|
|  | [add(Document[] documents, IndexingOptions options)](#add-com.groupdocs.search.Document---com.groupdocs.search.options.IndexingOptions-) | Esegue l'operazione di indicizzazione. |
|
|  | [add(ExtractedData[] data, IndexingOptions options)](#add-com.groupdocs.search.ExtractedData---com.groupdocs.search.options.IndexingOptions-) | Esegue l'operazione di indicizzazione. |
|
|  | [update()](#update--) | Reindicizza i documenti che sono stati modificati o eliminati dall'ultimo aggiornamento. |
|
|  | [update(UpdateOptions options)](#update-com.groupdocs.search.options.UpdateOptions-) | Reindicizza i documenti che sono stati modificati o eliminati dall'ultimo aggiornamento. |
|
|  | [getIndexingReports()](#getIndexingReports--) | Ottiene i report sulle operazioni di indicizzazione. |
|
|  | [getSearchReports()](#getSearchReports--) | Ottiene i report sulle operazioni di ricerca. |
|
|  | [search(String query)](#search-java.lang.String-) | Cerca nell'indice. |
|
|  | [search(String query, SearchOptions options)](#search-java.lang.String-com.groupdocs.search.options.SearchOptions-) | Cerca nell'indice. |
|
|  | [search(SearchQuery query)](#search-com.groupdocs.search.SearchQuery-) | Cerca nell'indice. |
|
|  | [search(SearchQuery query, SearchOptions options)](#search-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-) | Cerca nell'indice. |
|
|  | [search(SearchImage image, ImageSearchOptions options)](#search-com.groupdocs.search.common.SearchImage-com.groupdocs.search.options.ImageSearchOptions-) | Esegue una ricerca inversa di immagini nell'indice. |
|
|  | [searchNext(ChunkSearchToken chunkSearchToken)](#searchNext-com.groupdocs.search.common.ChunkSearchToken-) | Continua la ricerca a blocchi iniziata con il metodo Search. |
|
|  | [searchNext(ChunkSearchToken chunkSearchToken, Cancellation cancellation)](#searchNext-com.groupdocs.search.common.ChunkSearchToken-com.groupdocs.search.common.Cancellation-) | Continua la ricerca a blocchi iniziata con il metodo Search. |
|
|  | [optimize()](#optimize--) | Riduce al minimo il numero di segmenti dell'indice unendoli uno con l'altro. |
|
|  | [optimize(MergeOptions options)](#optimize-com.groupdocs.search.options.MergeOptions-) | Riduce al minimo il numero di segmenti dell'indice unendoli uno con l'altro. |
|
|  | [merge(Index index, MergeOptions options)](#merge-com.groupdocs.search.Index-com.groupdocs.search.options.MergeOptions-) | Unisce l'indice specificato nell'indice corrente. |
|
|  | [merge(IndexRepository repository, MergeOptions options)](#merge-com.groupdocs.search.IndexRepository-com.groupdocs.search.options.MergeOptions-) | Unisce gli indici dal repository di indice specificato nell'indice corrente. |
|
|  | [highlight(FoundDocument document, Highlighter highlighter)](#highlight-com.groupdocs.search.results.FoundDocument-com.groupdocs.search.highlighters.Highlighter-) | Genera testo formattato in HTML con i termini trovati evidenziati. |
|
|  | [highlight(FoundDocument document, Highlighter highlighter, HighlightOptions options)](#highlight-com.groupdocs.search.results.FoundDocument-com.groupdocs.search.highlighters.Highlighter-com.groupdocs.search.options.HighlightOptions-) | Genera testo formattato in HTML con i termini trovati evidenziati. |
|
|  | [getIndexedDocuments()](#getIndexedDocuments--) | Ottiene un array di tutti i documenti indicizzati. |
|
|  | [getIndexedDocumentItems(DocumentInfo documentInfo)](#getIndexedDocumentItems-com.groupdocs.search.results.DocumentInfo-) | Ottiene un array di elementi di documento. |
|
|  | [GetIndexedDocument(String documentKey)](#GetIndexedDocument-java.lang.String-) | Ottiene un documento indicizzato per chiave del documento. |
|
|  | [getDocumentText(DocumentInfo documentInfo, OutputAdapter adapter)](#getDocumentText-com.groupdocs.search.results.DocumentInfo-com.groupdocs.search.common.OutputAdapter-) | Genera il testo di un documento indicizzato e lo passa attraverso un adattatore di output. |
|
|  | [getDocumentText(DocumentInfo documentInfo, OutputAdapter adapter, TextOptions options)](#getDocumentText-com.groupdocs.search.results.DocumentInfo-com.groupdocs.search.common.OutputAdapter-com.groupdocs.search.options.TextOptions-) | Genera testo formattato in HTML per il documento indicizzato e lo trasferisce attraverso l'adattatore di output. |
|
|  | [getIndexedPaths()](#getIndexedPaths--) | Ottiene un array di percorsi indicizzati - documenti o cartelle. |
|
|  | [delete(String[] paths, UpdateOptions options)](#delete-java.lang.String---com.groupdocs.search.options.UpdateOptions-) | Elimina file o cartelle indicizzati dall'indice. |
|
|  | [delete(UpdateOptions options, String[] documentKeys)](#delete-com.groupdocs.search.options.UpdateOptions-java.lang.String---) | Elimina i documenti indicizzati da flussi o strutture. |
|
|  | [notifyIndex(Notification notification)](#notifyIndex-com.groupdocs.search.Notification-) | Passa l'oggetto di notifica specificato all'indice per eseguire la notifica. |
|
|  | [changeAttributes(AttributeChangeBatch batch)](#changeAttributes-com.groupdocs.search.common.AttributeChangeBatch-) | Applica il batch specificato di modifiche agli attributi ai documenti indicizzati senza reindicizzare durante l'operazione di aggiornamento. |
|
|  | [getAttributes(String path)](#getAttributes-java.lang.String-) | Ottiene tutti gli attributi associati al documento indicizzato specificato. |
|
|  | [loadIntoMemoryCompletely(String indexFolder)](#loadIntoMemoryCompletely-java.lang.String-) | Carica l'intero indice in memoria. |
|
|  | [loadIntoMemoryCompletely(String indexFolder, IndexSettings settings)](#loadIntoMemoryCompletely-java.lang.String-com.groupdocs.search.IndexSettings-) | Carica l'intero indice in memoria. |
|
### Index() {#Index--}
```
public Index()
```


Inizializza una nuova istanza della classe  Index  in memoria.


L'esempio dimostra come creare un indice in memoria senza salvare i file su disco.

````
 ```

Index index = new Index();
 
```
 
````



### Index(IndexSettings settings) {#Index-com.groupdocs.search.IndexSettings-}
```
public Index(IndexSettings settings)
```


Inizializza una nuova istanza della classe  Index  in memoria con impostazioni dell'indice specifiche.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | L'oggetto delle impostazioni dell'indice. |


L'esempio dimostra come creare un indice in memoria senza salvare i file su disco con impostazioni di indice particolari.

````
 ```

IndexSettings settings = new IndexSettings();
settings.setIndexType(IndexType.CompactIndex);
Index index = new Index(settings);
 
```
 
````

|

### Index(String indexFolder) {#Index-java.lang.String-}
```
public Index(String indexFolder)
```


Inizializza una nuova istanza della  Index  classe. Crea un nuovo indice o apre un indice esistente su disco.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | indexFolder | java.lang.String | Il percorso della cartella dell'indice. |


L'esempio dimostra come creare un indice su disco o aprire un indice esistente.

````
 ```

String indexFolder = "c:\\MyIndex\\";
Index index = new Index(indexFolder);
 
```
 
````

|

### Index(String indexFolder, IndexSettings settings) {#Index-java.lang.String-com.groupdocs.search.IndexSettings-}
```
public Index(String indexFolder, IndexSettings settings)
```


Inizializza una nuova istanza di
Index
classe.
Crea un nuovo indice con impostazioni particolari o apre un indice esistente su disco.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | indexFolder | java.lang.String | Il percorso della cartella dell'indice. |
|
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | L'oggetto delle impostazioni dell'indice. |

L'esempio dimostra come creare un indice su disco con impostazioni specifiche dell'indice.

````
 ```

String indexFolder = "c:\\MyIndex\\";
IndexSettings settings = new IndexSettings();
settings.setIndexType(IndexType.CompactIndex);
Index index = new Index(indexFolder, settings);
 
```
 
````

|

### Index(String indexFolder, boolean overwriteIfExists) {#Index-java.lang.String-boolean-}
```
public Index(String indexFolder, boolean overwriteIfExists)
```


Inizializza una nuova istanza di
Index
classe.
Carica un indice esistente dal disco se
overwriteIfExists
è
false
;
crea un nuovo indice su disco altrimenti.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | indexFolder | java.lang.String | Il percorso della cartella dell'indice. |
|
|  | overwriteIfExists | boolean | Il flag per sovrascrivere la cartella dell'indice. |

L'esempio dimostra come creare un nuovo indice in una cartella che contiene già un altro indice.

````
 ```

String indexFolder = "c:\\MyIndex\\";
Index index = new Index(indexFolder, true);
 
```
 
````

|

### Index(String indexFolder, IndexSettings settings, boolean overwriteIfExists) {#Index-java.lang.String-com.groupdocs.search.IndexSettings-boolean-}
```
public Index(String indexFolder, IndexSettings settings, boolean overwriteIfExists)
```


Inizializza una nuova istanza di
Index
classe.
Carica un indice esistente dal disco se
overwriteIfExists
è
false
;
crea un nuovo indice su disco con impostazioni specifiche dell'indice altrimenti.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | indexFolder | java.lang.String | Il percorso della cartella dell'indice. |
|
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | L'oggetto delle impostazioni dell'indice. |
|
|  | overwriteIfExists | boolean | Il flag per sovrascrivere la cartella dell'indice. |

L'esempio dimostra come creare un indice su disco con impostazioni specifiche dell'indice.

````
 ```

String indexFolder = "c:\\MyIndex\\";
IndexSettings settings = new IndexSettings();
settings.setIndexType(IndexType.CompactIndex);
Index index = new Index(indexFolder, settings, true);
 
```
 
````

|

### getEvents() {#getEvents--}
```
public final EventHub getEvents()
```


Ottiene il hub degli eventi per iscriversi agli eventi.


**Returns:**
[EventHub](../../com.groupdocs.search.events/eventhub) - The event hub for subscribing to events.

### getIndexInfo() {#getIndexInfo--}
```
public final IndexInfo getIndexInfo()
```


Ottiene le informazioni di base sull'indice.


**Returns:**
[IndexInfo](../../com.groupdocs.search.common/indexinfo) - The basic information on the index.

### getRepository() {#getRepository--}
```
public final IndexRepository getRepository()
```


Ottiene l'oggetto repository dell'indice se l'indice è contenuto in esso.


**Returns:**
[IndexRepository](../../com.groupdocs.search/indexrepository) - The index repository object.

### getIndexSettings() {#getIndexSettings--}
```
public final IndexSettings getIndexSettings()
```


Ottiene le impostazioni dell'indice.


**Returns:**
[IndexSettings](../../com.groupdocs.search/indexsettings) - The index settings.

### getDictionaries() {#getDictionaries--}
```
public final DictionaryRepository getDictionaries()
```


Ottiene il repository del dizionario.


**Returns:**
[DictionaryRepository](../../com.groupdocs.search.dictionaries/dictionaryrepository) - The dictionary repository.

### close() {#close--}
```
public final void close()
```


Rilascia tutte le risorse utilizzate da
Index
.


### add(String path) {#add-java.lang.String-}
```
public final void add(String path)
```


Esegue l'operazione di indicizzazione.
Aggiunge un file o una cartella tramite un percorso assoluto o relativo.
I documenti di tutte le sottocartelle saranno indicizzati.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | percorso | java.lang.String | Il percorso di un file o di una cartella da indicizzare. |

L'esempio dimostra come aggiungere documenti a un indice.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String folderPath = "c:\\MyDocuments\\";
String filePath = "c:\\Documents\\MyFile.txt";
Index index = new Index(indexFolder); // Creazione dell'indice nella cartella specificata
index.add(folderPath); // Indicizzazione dei documenti nella cartella specificata
index.add(filePath); // Indicizzazione del documento specificato
 
```
 
````

|

### add(String path, IndexingOptions options) {#add-java.lang.String-com.groupdocs.search.options.IndexingOptions-}
```
public final void add(String path, IndexingOptions options)
```


Esegue l'operazione di indicizzazione.
Aggiunge un file o una cartella tramite un percorso assoluto o relativo.
I documenti di tutte le sottocartelle saranno indicizzati.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | percorso | java.lang.String | Il percorso di un file o di una cartella da indicizzare. |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | Le opzioni di indicizzazione. |

L'esempio dimostra come aggiungere documenti a un indice con particolari opzioni di indicizzazione.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String folderPath = "c:\\MyDocuments\\";
String filePath = "c:\\Documents\\MyFile.txt";
Index index = new Index(indexFolder); // Creazione dell'indice nella cartella specificata
IndexingOptions options = new IndexingOptions();
options.setThreads(2); // Impostazione del numero di thread di indicizzazione
index.add(folderPath, options); // Indicizzazione dei documenti nella cartella specificata
index.add(filePath, options); // Indicizzazione del documento specificato
 
```
 
````

|

### add(String[] paths) {#add-java.lang.String---}
```
public final void add(String[] paths)
```


Esegue l'operazione di indicizzazione.
Aggiunge file o cartelle tramite un percorso assoluto o relativo.
I documenti di tutte le sottocartelle saranno indicizzati.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | paths | java.lang.String[] | I percorsi a file o cartelle da indicizzare. |

L'esempio dimostra come aggiungere documenti a un indice.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String folderPath = "c:\\MyDocuments\\";
String filePath = "c:\\Documents\\MyFile.txt";
Index index = new Index(indexFolder); // Creazione dell'indice nella cartella specificata
String[] paths = new String[] { folderPath, filePath };
index.add(paths); // Indicizzazione dei documenti nei percorsi specificati
 
```
 
````

|

### add(String[] paths, IndexingOptions options) {#add-java.lang.String---com.groupdocs.search.options.IndexingOptions-}
```
public final void add(String[] paths, IndexingOptions options)
```


Esegue l'operazione di indicizzazione.
Aggiunge file o cartelle tramite un percorso assoluto o relativo.
I documenti di tutte le sottocartelle saranno indicizzati.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | paths | java.lang.String[] | I percorsi a file o cartelle da indicizzare. |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | Le opzioni di indicizzazione. |

L'esempio dimostra come aggiungere documenti a un indice con particolari opzioni di indicizzazione.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String folderPath = "c:\\MyDocuments\\";
String filePath = "c:\\Documents\\MyFile.txt";
Index index = new Index(indexFolder); // Creazione dell'indice nella cartella specificata
IndexingOptions options = new IndexingOptions();
options.setThreads(2); // Impostazione del numero di thread di indicizzazione
String[] paths = new String[] { folderPath, filePath };
index.add(paths, options); // Indicizzazione dei documenti nei percorsi specificati
 
```
 
````

|

### add(Document[] documents, IndexingOptions options) {#add-com.groupdocs.search.Document---com.groupdocs.search.options.IndexingOptions-}
```
public final void add(Document[] documents, IndexingOptions options)
```


Esegue l'operazione di indicizzazione.
Aggiunge documenti dal file system, dallo stream o dalla struttura.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | documents | [Document\[\]](../../com.groupdocs.search/document) | I documenti dal file system, dallo stream o dalla struttura. |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | Le opzioni di indicizzazione. |
|

### add(ExtractedData[] data, IndexingOptions options) {#add-com.groupdocs.search.ExtractedData---com.groupdocs.search.options.IndexingOptions-}
```
public final void add(ExtractedData[] data, IndexingOptions options)
```


Esegue l'operazione di indicizzazione.
Aggiunge i dati estratti all'indice.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | data | [ExtractedData\[\]](../../com.groupdocs.search/extracteddata) | I dati estratti. |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | Le opzioni di indicizzazione. |
|

### update() {#update--}
```
public final void update()
```


Reindicizza i documenti che sono stati modificati o eliminati dall'ultimo aggiornamento.
Aggiunge nuovi file che sono stati aggiunti alle cartelle indicizzate.

L'esempio dimostra come aggiornare un indice.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Creazione dell'indice nella cartella specificata
index.add(documentsFolder); // Indicizzazione dei documenti dalla cartella specificata
// Elimina i documenti dalla cartella dei documenti o modificali o aggiungi nuovi documenti alla cartella
index.update(); // Aggiornamento dell'indice
 
```
 
````



### update(UpdateOptions options) {#update-com.groupdocs.search.options.UpdateOptions-}
```
public final void update(UpdateOptions options)
```


Reindicizza i documenti che sono stati modificati o eliminati dall'ultimo aggiornamento.
Aggiunge nuovi file che sono stati aggiunti alle cartelle indicizzate.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | options | [UpdateOptions](../../com.groupdocs.search.options/updateoptions) | Le opzioni di aggiornamento. |

L'esempio dimostra come aggiornare un indice con particolari opzioni di aggiornamento.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Creazione dell'indice nella cartella specificata
index.add(documentsFolder); // Indicizzazione dei documenti dalla cartella specificata
// Elimina i documenti dalla cartella dei documenti o modificali o aggiungi nuovi documenti alla cartella
UpdateOptions options = new UpdateOptions();
options.setThreads(2); // Impostazione del numero di thread di indicizzazione
index.update(options); // Aggiornamento dell'indice
 
```
 
````

|

### getIndexingReports() {#getIndexingReports--}
```
public final IndexingReport[] getIndexingReports()
```


Ottiene i report sulle operazioni di indicizzazione.


**Returns:**
com.groupdocs.search.common.IndexingReport[] - I report di indicizzazione.

L'esempio dimostra come ottenere i report di indicizzazione.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Creazione dell'indice nella cartella specificata
index.add(documentsFolder); // Indicizzazione dei documenti dalla cartella specificata
IndexingReport[] reports = index.getIndexingReports(); // Ottenimento dei report di indicizzazione
 
```
 
````


### getSearchReports() {#getSearchReports--}
```
public final SearchReport[] getSearchReports()
```


Ottiene i report sulle operazioni di ricerca.


**Returns:**
com.groupdocs.search.common.SearchReport[] - I report di ricerca.

L'esempio dimostra come ottenere i report di ricerca.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query1 = "Einstein";
String query2 = "Newton";
Index index = new Index(indexFolder); // Creazione dell'indice nella cartella specificata
index.add(documentsFolder); // Indicizzazione dei documenti dalla cartella specificata
SearchResult result1 = index.search(query1); // Ricerca
SearchResult result2 = index.search(query2);
SearchResult result3 = index.search(query1 + " & " + query2);
SearchReport[] reports = index.getSearchReports(); // Ottenere i report di ricerca
 
```
 
````


### search(String query) {#search-java.lang.String-}
```
public final SearchResult search(String query)
```


Cerca nell'indice.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | query | java.lang.String | La query di ricerca. |

Il seguente esempio dimostra come eseguire una ricerca semplice.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // Creazione dell'indice nella cartella specificata
index.add(documentsFolder); // Indicizzazione dei documenti dalla cartella specificata
SearchResult result = index.search(query); // Ricerca
 
```
 
````

Il seguente esempio dimostra come eseguire una ricerca Regex.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Creazione dell'indice nella cartella specificata
index.add(documentsFolder); // Indicizzazione dei documenti dalla cartella specificata
String query = "^[0-9]{3,}"; // Il simbolo caret all'inizio della query di ricerca indica all'indice che si tratta di una query Regex
SearchResult result = index.search(query); // Ricerca
 
```
 
````

Il seguente esempio dimostra come eseguire una ricerca a faccette.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Creazione dell'indice nella cartella specificata
index.add(documentsFolder); // Indicizzazione dei documenti dalla cartella specificata
String query = "content:Newton"; // La parola prima dei due punti nella query indica il nome del campo del documento da cercare
SearchResult result = index.search(query); // Ricerca
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(String query, SearchOptions options) {#search-java.lang.String-com.groupdocs.search.options.SearchOptions-}
```
public final SearchResult search(String query, SearchOptions options)
```


Cerca nell'indice.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | query | java.lang.String | La query di ricerca. |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | Le opzioni di ricerca. |

Il seguente esempio dimostra come eseguire una ricerca fuzzy.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Creazione dell'indice nella cartella specificata
index.add(documentsFolder); // Indicizzazione dei documenti dalla cartella specificata
SearchOptions options = new SearchOptions();
options.getFuzzySearch().setEnabled(true); // Abilitazione della ricerca fuzzy
options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(1)); // Impostazione del numero di differenze possibili per ogni parola
// Le virgolette doppie all'inizio e alla fine indicano all'indice che si tratta di una query di ricerca frase
String query = "\"The Pursuit of Happiness\"";
SearchResult result = index.search(query, options); // Ricerca
 
```
 
````

Il seguente esempio dimostra come eseguire una ricerca sinonimo.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Creazione dell'indice nella cartella specificata
index.add(documentsFolder); // Indicizzazione dei documenti dalla cartella specificata
SearchOptions options = new SearchOptions();
options.setUseSynonymSearch(true); // Abilitazione della ricerca sinonimo
String query = "cry";
SearchResult result = index.search(query, options); // Ricerca
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(SearchQuery query) {#search-com.groupdocs.search.SearchQuery-}
```
public final SearchResult search(SearchQuery query)
```


Cerca nell'indice.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | La query di ricerca. |

Il seguente esempio dimostra come eseguire una ricerca utilizzando la query in forma di oggetto.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Creazione dell'indice nella cartella specificata
index.add(documentsFolder); // Indicizzazione dei documenti dalla cartella specificata
// Creazione della sottoquery 1
SearchQuery subquery1 = SearchQuery.createWordQuery("accommodation");
subquery1.setSearchOptions(new SearchOptions()); // Impostazione delle opzioni di ricerca solo per la sottoquery 1
subquery1.getSearchOptions().getFuzzySearch().setEnabled(true); // Abilitazione della ricerca fuzzy
subquery1.getSearchOptions().getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(3)); // Impostazione del numero massimo di differenze
// Creazione della sottoquery 2
SearchQuery subquery2 = SearchQuery.createNumericRangeQuery(1, 1000000);
// Creazione della sottoquery 3
SearchQuery subquery3 = SearchQuery.createRegexQuery("(.)\\1");
// Combinazione delle sottoquery in un'unica query
SearchQuery query = SearchQuery.createPhraseSearchQuery(subquery1, subquery2, subquery3);
SearchResult result = index.search(query); // Ricerca
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(SearchQuery query, SearchOptions options) {#search-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-}
```
public final SearchResult search(SearchQuery query, SearchOptions options)
```


Cerca nell'indice.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | La query di ricerca. |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | Le opzioni di ricerca. |

Il seguente esempio dimostra come eseguire una ricerca utilizzando la query in forma di oggetto.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Creazione dell'indice nella cartella specificata
index.add(documentsFolder); // Indicizzazione dei documenti dalla cartella specificata
// Creazione di una sottoquery di ricerca per intervallo di date
SearchQuery subquery1 = SearchQuery.createDateRangeQuery(new Date(2011, 6, 17), new Date(2013, 1, 1));
// Creazione di una sottoquery wildcard con numero di parole mancanti da 0 a 2
SearchQuery subquery2 = SearchQuery.createWildcardQuery(0, 2);
// Creazione di una sottoquery di parola semplice
SearchQuery subquery3 = SearchQuery.createWordQuery("birth");
subquery3.setSearchOptions(new SearchOptions()); // Impostazione delle opzioni di ricerca solo per la sottoquery 3
subquery3.getSearchOptions().getFuzzySearch().setEnabled(true);
subquery3.getSearchOptions().getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(1));
// Combinazione delle sottoquery in un'unica query
SearchQuery query = SearchQuery.createPhraseSearchQuery(subquery1, subquery2, subquery3);
// Creazione dell'oggetto opzioni di ricerca con capacità aumentata delle occorrenze trovate
SearchOptions options = new SearchOptions(); // Opzioni di ricerca complessive
options.setMaxOccurrenceCountPerTerm(1000000);
options.setMaxTotalOccurrenceCount(10000000);
SearchResult result = index.search(query, options); // Ricerca
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(SearchImage image, ImageSearchOptions options) {#search-com.groupdocs.search.common.SearchImage-com.groupdocs.search.options.ImageSearchOptions-}
```
public final ImageSearchResult search(SearchImage image, ImageSearchOptions options)
```


Esegue una ricerca inversa di immagini nell'indice.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | image | [SearchImage](../../com.groupdocs.search.common/searchimage) | L'immagine da cercare. |
|
|  | options | [ImageSearchOptions](../../com.groupdocs.search.options/imagesearchoptions) | Le opzioni di ricerca dell'immagine. |
|

**Returns:**
[ImageSearchResult](../../com.groupdocs.search.results/imagesearchresult) - The result of a reverse image search.

### searchNext(ChunkSearchToken chunkSearchToken) {#searchNext-com.groupdocs.search.common.ChunkSearchToken-}
```
public final SearchResult searchNext(ChunkSearchToken chunkSearchToken)
```


Continua la ricerca a blocchi iniziata con il metodo Search.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | chunkSearchToken | [ChunkSearchToken](../../com.groupdocs.search.common/chunksearchtoken) | Il token di ricerca a blocchi. |

L'esempio dimostra come eseguire la ricerca a blocchi.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // Creazione dell'indice nella cartella specificata
index.add(documentsFolder); // Indicizzazione dei documenti dalla cartella specificata
SearchOptions options = new SearchOptions();
options.setChunkSearch(true); // Abilitazione della ricerca a blocchi
SearchResult result = index.search(query, options); // Avvio della ricerca a blocchi
System.out.println("Numero di documenti: " + result.getDocumentCount());
System.out.println("Numero di occorrenze: " + result.getOccurrenceCount());
while (result.getNextChunkSearchToken() != null) {
result = index.searchNext(result.getNextChunkSearchToken()); // Continuazione della ricerca a blocchi
System.out.println("Numero di documenti: " + result.getDocumentCount());
System.out.println("Numero di occorrenze: " + result.getOccurrenceCount());
}
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### searchNext(ChunkSearchToken chunkSearchToken, Cancellation cancellation) {#searchNext-com.groupdocs.search.common.ChunkSearchToken-com.groupdocs.search.common.Cancellation-}
```
public final SearchResult searchNext(ChunkSearchToken chunkSearchToken, Cancellation cancellation)
```


Continua la ricerca a blocchi iniziata con il metodo Search.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | chunkSearchToken | [ChunkSearchToken](../../com.groupdocs.search.common/chunksearchtoken) | Il token di ricerca a blocchi. |
|
|  | cancellation | [Cancellation](../../com.groupdocs.search.common/cancellation) | L'oggetto di cancellazione. |

L'esempio dimostra come eseguire la ricerca usando la query in forma di oggetto.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // Creazione dell'indice nella cartella specificata
index.add(documentsFolder); // Indicizzazione dei documenti dalla cartella specificata
Cancellation cancellation = new Cancellation(); // Questo oggetto di cancellazione interrompe tutte le continuazioni della ricerca se annullato
SearchOptions options = new SearchOptions();
options.setChunkSearch(true); // Abilitazione della ricerca a blocchi
options.setCancellation(cancellation);
SearchResult result = index.search(query, options); // Avvio della ricerca a blocchi
System.out.println("Numero di documenti: " + result.getDocumentCount());
System.out.println("Numero di occorrenze: " + result.getOccurrenceCount());
while (result.getNextChunkSearchToken() != null) {
result = index.searchNext(result.getNextChunkSearchToken(), cancellation); // Continuazione della ricerca a blocchi
System.out.println("Numero di documenti: " + result.getDocumentCount());
System.out.println("Numero di occorrenze: " + result.getOccurrenceCount());
}
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### optimize() {#optimize--}
```
public final void optimize()
```


Riduce al minimo il numero di segmenti dell'indice unendoli uno con l'altro.
Questa operazione migliora le prestazioni della ricerca.

L'esempio dimostra come unire i segmenti di un indice.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder1 = "c:\\MyDocuments1\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
String documentsFolder3 = "c:\\MyDocuments3\\";
Index index = new Index(indexFolder); // Creazione dell'indice nella cartella specificata
index.add(documentsFolder1); // Indicizzazione dei documenti dalla cartella specificata
index.add(documentsFolder2); // Ogni chiamata a AddToIndex crea almeno un nuovo segmento nell'indice
index.add(documentsFolder3);
// Unione dei segmenti dell'indice
index.optimize();
 
```
 
````



### optimize(MergeOptions options) {#optimize-com.groupdocs.search.options.MergeOptions-}
```
public final void optimize(MergeOptions options)
```


Riduce al minimo il numero di segmenti dell'indice unendoli uno con l'altro.
Questa operazione migliora le prestazioni della ricerca.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | options | [MergeOptions](../../com.groupdocs.search.options/mergeoptions) | Le opzioni di unione. |

L'esempio dimostra come unire segmenti di un indice con particolari opzioni di unione.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder1 = "c:\\MyDocuments1\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
String documentsFolder3 = "c:\\MyDocuments3\\";
Index index = new Index(indexFolder); // Creazione dell'indice nella cartella specificata
index.add(documentsFolder1); // Indicizzazione dei documenti dalla cartella specificata
index.add(documentsFolder2); // Ogni chiamata a AddToIndex crea almeno un nuovo segmento nell'indice
index.add(documentsFolder3);
MergeOptions options = new MergeOptions();
options.setAsync(true); // Operazione asincrona
options.setCancellation(new Cancellation()); // Creazione dell'oggetto di cancellazione
// Unione dei segmenti dell'indice
index.optimize(options); // Questo metodo ritornerà prima che l'operazione sia completata
options.getCancellation().cancelAfter(10000); // Impostazione della durata massima dell'operazione a 10 secondi
 
```
 
````

|

### merge(Index index, MergeOptions options) {#merge-com.groupdocs.search.Index-com.groupdocs.search.options.MergeOptions-}
```
public final void merge(Index index, MergeOptions options)
```


Unisce l'indice specificato nell'indice corrente.
Nota che l'altro indice non verrà modificato.


Se l'altro indice ha una versione precedente, deve essere aggiornato prima di unirsi a
IndexUpdater
.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | index | [Index](../../com.groupdocs.search/index) | L'indice in cui unire. |
|
|  | options | [MergeOptions](../../com.groupdocs.search.options/mergeoptions) | Le opzioni di unione. |

L'esempio dimostra come unire un indice nell'indice corrente.

````
 ```

String indexFolder1 = "c:\\MyIndex1\\";
String indexFolder2 = "c:\\MyIndex2\\";
String documentsFolder1 = "c:\\MyDocuments1\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
Index index1 = new Index(indexFolder1); // Creazione di index1
index1.add(documentsFolder1); // Indicizzazione dei documenti
Index index2 = new Index(indexFolder2); // Creazione di index2
index2.add(documentsFolder2); // Indicizzazione dei documenti
MergeOptions options = new MergeOptions();
options.setCancellation(new Cancellation()); // Creazione dell'oggetto di cancellazione
// Unione di index2 in index1. Nota che i file di index2 non saranno modificati.
index1.merge(index2, options);
 
```
 
````

|

### merge(IndexRepository repository, MergeOptions options) {#merge-com.groupdocs.search.IndexRepository-com.groupdocs.search.options.MergeOptions-}
```
public final void merge(IndexRepository repository, MergeOptions options)
```


Unisce gli indici dal repository di indice specificato nell'indice corrente.
Nota che gli indici nel repository non saranno modificati.


Se altri indici hanno una versione precedente, devono essere aggiornati prima di unire con
IndexUpdater
.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | repository | [IndexRepository](../../com.groupdocs.search/indexrepository) | Il repository di indice in cui unire. |
|
|  | options | [MergeOptions](../../com.groupdocs.search.options/mergeoptions) | Le opzioni di unione. |

L'esempio dimostra come unire un repository di indice nell'indice corrente.

````
 ```

String indexFolder1 = "c:\\MyIndex1\\";
String indexFolder2 = "c:\\MyIndex2\\";
String indexFolder3 = "c:\\MyIndex3\\";
String documentsFolder1 = "c:\\MyDocuments1\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
String documentsFolder3 = "c:\\MyDocuments3\\";
Index index1 = new Index(indexFolder1); // Creazione di index1
index1.add(documentsFolder1); // Indicizzazione dei documenti
IndexRepository repository = new IndexRepository(); // Creazione del repository di indice
Index index2 = repository.create(indexFolder2); // Creazione di index2
index2.add(documentsFolder2); // Indicizzazione dei documenti
Index index3 = repository.create(indexFolder3); // Creazione di index3
index3.add(documentsFolder3); // Indicizzazione dei documenti
MergeOptions options = new MergeOptions();
options.setCancellation(new Cancellation()); // Creazione dell'oggetto di cancellazione
// Unione di tutti gli indici nel repository di indice in index1. Nota che index2 e index3 non saranno modificati.
index1.merge(repository, options);
 
```
 
````

|

### highlight(FoundDocument document, Highlighter highlighter) {#highlight-com.groupdocs.search.results.FoundDocument-com.groupdocs.search.highlighters.Highlighter-}
```
public final void highlight(FoundDocument document, Highlighter highlighter)
```


Genera testo formattato in HTML con i termini trovati evidenziati.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | document | [FoundDocument](../../com.groupdocs.search.results/founddocument) | Il documento trovato. |
|
|  | highlighter | [Highlighter](../../com.groupdocs.search.highlighters/highlighter) | L'evidenziatore del risultato di ricerca. |

L'esempio dimostra come evidenziare le occorrenze in testo formattato HTML.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentFolder = "c:\\MyDocuments\\";
// Creazione di un indice
Index index = new Index(indexFolder);
// Indicizzazione dei documenti dalla cartella specificata
index.add(documentFolder);
// Ricerca della parola 'eternity'
SearchResult result = index.search("eternity");
// Evidenziazione delle occorrenze nel testo
if (result.getDocumentCount() > 0) {
FoundDocument document = result.getFoundDocument(0); // Ottenimento del primo documento trovato
OutputAdapter outputAdapter = new FileOutputAdapter("c:\\Highlighted.html"); // Creazione di un adattatore di output verso il file
Highlighter highlighter = new HtmlHighlighter(outputAdapter); // Creazione dell'oggetto evidenziatore
index.highlight(document, highlighter); // Generazione di testo formattato HTML con occorrenze evidenziate
}
 
```
 
````

|

### highlight(FoundDocument document, Highlighter highlighter, HighlightOptions options) {#highlight-com.groupdocs.search.results.FoundDocument-com.groupdocs.search.highlighters.Highlighter-com.groupdocs.search.options.HighlightOptions-}
```
public final void highlight(FoundDocument document, Highlighter highlighter, HighlightOptions options)
```


Genera testo formattato in HTML con i termini trovati evidenziati.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | document | [FoundDocument](../../com.groupdocs.search.results/founddocument) | Il documento trovato. |
|
|  | highlighter | [Highlighter](../../com.groupdocs.search.highlighters/highlighter) | L'evidenziatore del risultato di ricerca. |
|
|  | options | [HighlightOptions](../../com.groupdocs.search.options/highlightoptions) | Le opzioni di evidenziazione. |

L'esempio dimostra come evidenziare le occorrenze in testo formattato HTML.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentFolder = "c:\\MyDocuments\\";
// Creazione di un indice
Index index = new Index(indexFolder);
// Indicizzazione dei documenti dalla cartella specificata
index.add(documentFolder);
// Ricerca della parola 'eternity'
SearchResult result = index.search("eternity");
// Evidenziazione delle occorrenze nel testo
if (result.getDocumentCount() > 0) {
FoundDocument document = result.getFoundDocument(0); // Ottenimento del primo documento trovato
OutputAdapter outputAdapter = new FileOutputAdapter("c:\\Highlighted.html"); // Creazione di un adattatore di output verso il file
Highlighter highlighter = new HtmlHighlighter(outputAdapter); // Creazione dell'oggetto evidenziatore
HighlightOptions options = new HighlightOptions(); // Creazione dell'oggetto opzioni di evidenziazione
options.setTermsBefore(5);
options.setTermsAfter(5);
options.setTermsTotal(15);
index.highlight(document, highlighter, options); // Generazione di testo formattato HTML con occorrenze evidenziate
}
 
```
 
````

|

### getIndexedDocuments() {#getIndexedDocuments--}
```
public final DocumentInfo[] getIndexedDocuments()
```


Ottiene un array di tutti i documenti indicizzati.


**Returns:**
com.groupdocs.search.results.DocumentInfo[] - Un array di tutti i documenti indicizzati.

L'esempio dimostra come ottenere un elenco di documenti indicizzati da un indice.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Creazione di un indice nella cartella specificata
Index index = new Index(indexFolder);
// Indicizzazione dei documenti dalla cartella specificata
index.add(documentsFolder);
// Ottenere l'elenco dei documenti indicizzati
DocumentInfo[] documents = index.getIndexedDocuments();
 
```
 
````


### getIndexedDocumentItems(DocumentInfo documentInfo) {#getIndexedDocumentItems-com.groupdocs.search.results.DocumentInfo-}
```
public final DocumentInfo[] getIndexedDocumentItems(DocumentInfo documentInfo)
```


Ottiene un array di elementi di documento.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | documentInfo | [DocumentInfo](../../com.groupdocs.search.results/documentinfo) | Un'informazione sul documento. |

L'esempio dimostra come ottenere un elenco di elementi di un documento indicizzato da un indice.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Creazione di un indice nella cartella specificata
Index index = new Index(indexFolder);
// Indicizzazione dei documenti dalla cartella specificata
index.add(documentsFolder);
// Ottenere l'elenco dei documenti indicizzati
DocumentInfo[] documents = index.getIndexedDocuments();
for (int i = 0; i < documents.length; i++) {
DocumentInfo document = documents[i];
System.out.println(document.getFilePath());
DocumentInfo[] items = index.getIndexedDocumentItems(document); // Ottenere l'elenco degli elementi del documento
for (int j = 0; j < items.length; j++) {
DocumentInfo item = items[j];
System.out.println("\t" + item.getInnerPath());
}
}
 
```
 
````

|

**Returns:**
com.groupdocs.search.results.DocumentInfo[] - Un array di elementi di un documento.

### GetIndexedDocument(String documentKey) {#GetIndexedDocument-java.lang.String-}
```
public DocumentInfo GetIndexedDocument(String documentKey)
```


Ottiene un documento indicizzato per chiave del documento.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | documentKey | java.lang.String | La chiave del documento. |
|

**Returns:**
[DocumentInfo](../../com.groupdocs.search.results/documentinfo) - The indexed document.

### getDocumentText(DocumentInfo documentInfo, OutputAdapter adapter) {#getDocumentText-com.groupdocs.search.results.DocumentInfo-com.groupdocs.search.common.OutputAdapter-}
```
public final void getDocumentText(DocumentInfo documentInfo, OutputAdapter adapter)
```


Genera il testo di un documento indicizzato e lo passa attraverso un adattatore di output.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | documentInfo | [DocumentInfo](../../com.groupdocs.search.results/documentinfo) | Le informazioni del documento indicizzato. |
|
|  | adapter | [OutputAdapter](../../com.groupdocs.search.common/outputadapter) | L'adattatore di output. |

L'esempio dimostra come ottenere il testo di un documento indicizzato da un indice.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Creazione di un indice nella cartella specificata
Index index = new Index(indexFolder);
// Indicizzazione dei documenti dalla cartella specificata
index.add(documentsFolder);
// Ottenere l'elenco dei documenti indicizzati
DocumentInfo[] documents = index.getIndexedDocuments();
// Ottenere il testo di un documento
if (documents.length > 0) {
FileOutputAdapter outputAdapter = new FileOutputAdapter("C:\\Text.html");
index.getDocumentText(documents[0], outputAdapter);
}
 
```
 
````

|

### getDocumentText(DocumentInfo documentInfo, OutputAdapter adapter, TextOptions options) {#getDocumentText-com.groupdocs.search.results.DocumentInfo-com.groupdocs.search.common.OutputAdapter-com.groupdocs.search.options.TextOptions-}
```
public final void getDocumentText(DocumentInfo documentInfo, OutputAdapter adapter, TextOptions options)
```


Genera testo formattato in HTML per il documento indicizzato e lo trasferisce attraverso l'adattatore di output.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | documentInfo | [DocumentInfo](../../com.groupdocs.search.results/documentinfo) | Le informazioni del documento indicizzato. |
|
|  | adapter | [OutputAdapter](../../com.groupdocs.search.common/outputadapter) | L'adattatore di output. |
|
|  | options | [TextOptions](../../com.groupdocs.search.options/textoptions) | Le opzioni di recupero del testo. |
|

### getIndexedPaths() {#getIndexedPaths--}
```
public final String[] getIndexedPaths()
```


Ottiene un array di percorsi indicizzati - documenti o cartelle.


**Returns:**
java.lang.String[] - Un array di percorsi indicizzati.

### delete(String[] paths, UpdateOptions options) {#delete-java.lang.String---com.groupdocs.search.options.UpdateOptions-}
```
public final DeleteResult delete(String[] paths, UpdateOptions options)
```


Elimina file o cartelle indicizzate dall'indice. Quindi aggiorna l'indice senza i percorsi eliminati.
Nota che un documento individuale non può essere eliminato dall'indice se è stato aggiunto all'indice come parte di una cartella.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | paths | java.lang.String[] | I percorsi di file o cartelle da eliminare. |
|
|  | options | [UpdateOptions](../../com.groupdocs.search.options/updateoptions) | Le opzioni di aggiornamento. |

L'esempio dimostra come eliminare percorsi indicizzati da un indice.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder1 = "c:\\MyDocuments\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
// Creazione di un indice nella cartella specificata
Index index = new Index(indexFolder);
// Indicizzazione dei documenti dalle cartelle specificate
index.add(documentsFolder1);
index.add(documentsFolder2);
// Ottenere i percorsi indicizzati dall'indice
String[] indexedPaths1 = index.getIndexedPaths();
// Scrivere i percorsi indicizzati nella console
System.out.println("Percorsi indicizzati:");
for (String path : indexedPaths1) {
System.out.println("\t" + path);
}
// Eliminazione del percorso dell'indice dall'indice
DeleteResult deleteResult = index.delete(new String[] { documentsFolder1 }, new UpdateOptions());
// Ottenere i percorsi indicizzati dopo l'eliminazione
String[] indexedPaths2 = index.getIndexedPaths();
System.out.println("\nPercorsi eliminati: " + deleteResult.getSuccessCount());
System.out.println("\nIndexed paths:");
for (String path : indexedPaths2) {
System.out.println("\t" + path);
}
 
```
 
````

|

**Returns:**
[DeleteResult](../../com.groupdocs.search.results/deleteresult) - An object describing the result of deleting files or folders from the index.

### delete(UpdateOptions options, String[] documentKeys) {#delete-com.groupdocs.search.options.UpdateOptions-java.lang.String---}
```
public final DeleteResult delete(UpdateOptions options, String[] documentKeys)
```


Elimina i documenti indicizzati da flussi o strutture. Quindi aggiorna l'indice senza i documenti eliminati.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | options | [UpdateOptions](../../com.groupdocs.search.options/updateoptions) | Le opzioni di aggiornamento. |
|
|  | documentKeys | java.lang.String[] | Le chiavi dei documenti aggiunti da flussi o strutture. |
|

**Returns:**
[DeleteResult](../../com.groupdocs.search.results/deleteresult) - An object describing the result of deleting documents from the index.

### notifyIndex(Notification notification) {#notifyIndex-com.groupdocs.search.Notification-}
```
public final boolean notifyIndex(Notification notification)
```


Passa l'oggetto di notifica specificato all'indice per eseguire la notifica.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | notification | [Notification](../../com.groupdocs.search/notification) | L'oggetto di notifica. |
|

**Returns:**
boolean - Restituisce  true  se la notifica è stata eseguita con successo; altrimenti  false .

### changeAttributes(AttributeChangeBatch batch) {#changeAttributes-com.groupdocs.search.common.AttributeChangeBatch-}
```
public final void changeAttributes(AttributeChangeBatch batch)
```


Applica il batch specificato di modifiche agli attributi ai documenti indicizzati senza reindicizzare durante l'operazione di aggiornamento.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | batch | [AttributeChangeBatch](../../com.groupdocs.search.common/attributechangebatch) | Il batch di modifiche degli attributi. |
|

### getAttributes(String path) {#getAttributes-java.lang.String-}
```
public final String[] getAttributes(String path)
```


Ottiene tutti gli attributi associati al documento indicizzato specificato.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | percorso | java.lang.String | Il percorso del documento. |
|

**Returns:**
java.lang.String[] - Attributi associati al documento.

### loadIntoMemoryCompletely(String indexFolder) {#loadIntoMemoryCompletely-java.lang.String-}
```
public static Index loadIntoMemoryCompletely(String indexFolder)
```


Carica l'intero indice in memoria.
Qualsiasi modifica all'indice non viene salvata automaticamente nella cartella originale.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | indexFolder | java.lang.String | Il percorso della cartella dell'indice. |
|

**Returns:**
[Index](../../com.groupdocs.search/index) - The loaded in-memory index.

### loadIntoMemoryCompletely(String indexFolder, IndexSettings settings) {#loadIntoMemoryCompletely-java.lang.String-com.groupdocs.search.IndexSettings-}
```
public static Index loadIntoMemoryCompletely(String indexFolder, IndexSettings settings)
```


Carica l'intero indice in memoria.
Qualsiasi modifica all'indice non viene salvata automaticamente nella cartella originale.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | indexFolder | java.lang.String | Il percorso della cartella dell'indice. |
|
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | L'oggetto delle impostazioni dell'indice. |
|

**Returns:**
[Index](../../com.groupdocs.search/index) - The loaded in-memory index.

