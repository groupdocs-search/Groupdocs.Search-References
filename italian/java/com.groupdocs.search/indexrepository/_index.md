---
title: "IndexRepository"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Rappresenta un contenitore per combinare più indici ed eseguire operazioni comuni su di essi."
type: docs
weight: 18
url: /it/java/com.groupdocs.search/indexrepository/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.io.Closeable
```
public class IndexRepository implements Closeable
```

Rappresenta un contenitore per combinare più indici ed eseguire operazioni comuni su di essi.


**Learn more**

* [Search index repository](../https://docs.groupdocs.com/display/searchjava/Search+index+repository)


L'esempio dimostra un utilizzo tipico della classe.

````
 ```

String indexFolder1 = "c:\\MyIndex\\";
String indexFolder2 = "c:\\MyIndex\\";
String query = "Einstein";
IndexRepository repository = new IndexRepository();
repository.addToRepository(indexFolder1); // Caricamento di un indice esistente
repository.addToRepository(indexFolder2); // Caricamento di un altro indice esistente
SearchResult result = repository.search(query); // Ricerca negli indici del repository
 
```
 
````


## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [IndexRepository()](#IndexRepository--) | Inizializza una nuova istanza di |
IndexRepository
classe.
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getEvents()](#getEvents--) | Ottiene il hub degli eventi per iscriversi agli eventi. |
|
|  | [getIndexes()](#getIndexes--) | Ottiene gli indici contenuti in questo |
IndexRepository
.
|
|  | [close()](#close--) | Rilascia tutte le risorse utilizzate da |
IndexRepository
.
|
|  | [create()](#create--) | Crea un nuovo indice in memoria. |
|
|  | [create(IndexSettings settings)](#create-com.groupdocs.search.IndexSettings-) | Crea un nuovo indice in memoria. |
|
|  | [create(String indexFolder)](#create-java.lang.String-) | Crea un nuovo indice su disco. |
|
|  | [create(String indexFolder, IndexSettings settings)](#create-java.lang.String-com.groupdocs.search.IndexSettings-) | Crea un nuovo indice su disco. |
|
|  | [addToRepository(Index index)](#addToRepository-com.groupdocs.search.Index-) | Aggiunge un indice al repository degli indici. |
|
|  | [addToRepository(String indexFolder)](#addToRepository-java.lang.String-) | Apre e aggiunge un indice al repository degli indici. |
|
|  | [update()](#update--) | Aggiorna tutti gli indici nel repository. |
|
|  | [update(UpdateOptions options)](#update-com.groupdocs.search.options.UpdateOptions-) | Aggiorna tutti gli indici nel repository. |
|
|  | [search(String query)](#search-java.lang.String-) | Cerca in tutti gli indici del repository. |
|
|  | [search(String query, SearchOptions options)](#search-java.lang.String-com.groupdocs.search.options.SearchOptions-) | Cerca in tutti gli indici del repository. |
|
|  | [search(SearchQuery query)](#search-com.groupdocs.search.SearchQuery-) | Cerca in tutti gli indici del repository. |
|
|  | [search(SearchQuery query, SearchOptions options)](#search-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-) | Cerca in tutti gli indici del repository. |
|
### IndexRepository() {#IndexRepository--}
```
public IndexRepository()
```


Inizializza una nuova istanza di
IndexRepository
classe.


### getEvents() {#getEvents--}
```
public final EventHub getEvents()
```


Ottiene il hub degli eventi per iscriversi agli eventi.


**Returns:**
[EventHub](../../com.groupdocs.search.events/eventhub) - The event hub for subscribing to events.

### getIndexes() {#getIndexes--}
```
public final Index[] getIndexes()
```


Ottiene gli indici contenuti in questo
IndexRepository
.


**Returns:**
com.groupdocs.search.Index[] - Gli indici.

### close() {#close--}
```
public final void close()
```


Rilascia tutte le risorse utilizzate da
IndexRepository
.


### create() {#create--}
```
public final Index create()
```


Crea un nuovo indice in memoria.


**Returns:**
[Index](../../com.groupdocs.search/index) - The created index.

L'esempio dimostra come creare un indice in memoria tramite il repository degli indici.

````
 ```

IndexRepository indexRepository = new IndexRepository();
Index index = indexRepository.create();
 
```
 
````


### create(IndexSettings settings) {#create-com.groupdocs.search.IndexSettings-}
```
public final Index create(IndexSettings settings)
```


Crea un nuovo indice in memoria.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | Le impostazioni dell'indice. |

L'esempio dimostra come creare un indice in memoria tramite il repository degli indici.

````
 ```

IndexRepository indexRepository = new IndexRepository();
IndexSettings settings = new IndexSettings();
settings.setUseStopWords(false); // Disabilita l'uso di parole stop durante l'indicizzazione
Index index = indexRepository.create(settings);
 
```
 
````

|

**Returns:**
[Index](../../com.groupdocs.search/index) - The created index.

### create(String indexFolder) {#create-java.lang.String-}
```
public final Index create(String indexFolder)
```


Crea un nuovo indice su disco.
La cartella dell'indice verrà pulita prima della creazione dell'indice.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | indexFolder | java.lang.String | La cartella dell'indice. |

L'esempio dimostra come creare un indice su disco tramite il repository degli indici.

````
 ```

String indexFolder = "c:\\MyIndex\\";
IndexRepository indexRepository = new IndexRepository();
Index index = indexRepository.create(indexFolder);
 
```
 
````

|

**Returns:**
[Index](../../com.groupdocs.search/index) - The created index.

### create(String indexFolder, IndexSettings settings) {#create-java.lang.String-com.groupdocs.search.IndexSettings-}
```
public final Index create(String indexFolder, IndexSettings settings)
```


Crea un nuovo indice su disco.
La cartella dell'indice verrà pulita prima della creazione dell'indice.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | indexFolder | java.lang.String | La cartella dell'indice. |
|
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | Le impostazioni dell'indice. |

L'esempio dimostra come creare un indice su disco tramite il repository degli indici.

````
 ```

String indexFolder = "c:\\MyIndex\\";
IndexRepository indexRepository = new IndexRepository();
IndexSettings settings = new IndexSettings();
settings.setUseStopWords(false); // Disabilita l'uso di parole stop durante l'indicizzazione
Index index = indexRepository.create(indexFolder, settings);
 
```
 
````

|

**Returns:**
[Index](../../com.groupdocs.search/index) - The created index.

### addToRepository(Index index) {#addToRepository-com.groupdocs.search.Index-}
```
public final void addToRepository(Index index)
```


Aggiunge un indice al repository degli indici.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | index | [Index](../../com.groupdocs.search/index) | L'indice da aggiungere. |

L'esempio dimostra come aggiungere un indice al repository degli indici.

````
 ```

Index index = new Index();
IndexRepository indexRepository = new IndexRepository();
indexRepository.addToRepository(index);
 
```
 
````

|

### addToRepository(String indexFolder) {#addToRepository-java.lang.String-}
```
public final void addToRepository(String indexFolder)
```


Apre e aggiunge un indice al repository degli indici.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | indexFolder | java.lang.String | La cartella dell'indice. |

L'esempio dimostra come aggiungere un indice al repository degli indici.

````
 ```

String indexFolder = "c:\\MyIndex\\";
IndexRepository indexRepository = new IndexRepository();
indexRepository.addToRepository(indexFolder);
 
```
 
````

|

### update() {#update--}
```
public final void update()
```


Aggiorna tutti gli indici nel repository.

L'esempio dimostra come aggiornare gli indici nel repository.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // Creazione dell'indice
index.add(documentsFolder); // Indicizzazione dei documenti
// Elimina i documenti dalla cartella dei documenti o modificali o aggiungi nuovi documenti alla cartella
repository.update();
 
```
 
````



### update(UpdateOptions options) {#update-com.groupdocs.search.options.UpdateOptions-}
```
public final void update(UpdateOptions options)
```


Aggiorna tutti gli indici nel repository.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | options | [UpdateOptions](../../com.groupdocs.search.options/updateoptions) | Le opzioni di aggiornamento. |

L'esempio dimostra come aggiornare gli indici nel repository.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // Creazione dell'indice
index.add(documentsFolder); // Indicizzazione dei documenti
// Elimina i documenti dalla cartella dei documenti o modificali o aggiungi nuovi documenti alla cartella
UpdateOptions options = new UpdateOptions();
options.setThreads(2); // Impostazione del numero di thread di indicizzazione
repository.update(options);
 
```
 
````

|

### search(String query) {#search-java.lang.String-}
```
public final SearchResult search(String query)
```


Cerca in tutti gli indici del repository.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | query | java.lang.String | La query di ricerca. |

L'esempio dimostra come eseguire la ricerca nel repository di indici.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // Creazione dell'indice
index.add(documentsFolder); // Indicizzazione dei documenti
SearchResult result = repository.search(query); // Ricerca
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(String query, SearchOptions options) {#search-java.lang.String-com.groupdocs.search.options.SearchOptions-}
```
public final SearchResult search(String query, SearchOptions options)
```


Cerca in tutti gli indici del repository.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | query | java.lang.String | La query di ricerca. |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | Le opzioni di ricerca. |

L'esempio dimostra come eseguire la ricerca nel repository di indici.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // Creazione dell'indice
index.add(documentsFolder); // Indicizzazione dei documenti
SearchOptions options = new SearchOptions();
options.setUseCaseSensitiveSearch(true); // Impostazione del flag di ricerca sensibile al maiuscolo/minuscolo
SearchResult result = repository.search(query, options); // Ricerca
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(SearchQuery query) {#search-com.groupdocs.search.SearchQuery-}
```
public final SearchResult search(SearchQuery query)
```


Cerca in tutti gli indici del repository.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | La query di ricerca. |

L'esempio dimostra come eseguire la ricerca nel repository di indici.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // Creazione dell'indice
index.add(documentsFolder); // Indicizzazione dei documenti
SearchQuery query = SearchQuery.createWordQuery("Einstein"); // Creazione della query di ricerca in forma di oggetto
SearchResult result = repository.search(query); // Ricerca
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(SearchQuery query, SearchOptions options) {#search-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-}
```
public final SearchResult search(SearchQuery query, SearchOptions options)
```


Cerca in tutti gli indici del repository.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | La query di ricerca. |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | Le opzioni di ricerca. |

L'esempio dimostra come eseguire la ricerca nel repository di indici.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // Creazione dell'indice
index.add(documentsFolder); // Indicizzazione dei documenti
SearchOptions options = new SearchOptions();
options.setUseCaseSensitiveSearch(true); // Impostazione del flag di ricerca sensibile al maiuscolo/minuscolo
SearchQuery query = SearchQuery.createWordQuery("Einstein"); // Creazione della query di ricerca in forma di oggetto
SearchResult result = repository.search(query, options); // Ricerca
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

