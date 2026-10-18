---
title: "IndexRepository"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Stellt einen Container dar, der mehrere Indizes kombiniert und gemeinsame Operationen darauf ausführt."
type: docs
weight: 18
url: /de/java/com.groupdocs.search/indexrepository/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.io.Closeable
```
public class IndexRepository implements Closeable
```

Stellt einen Container dar, der mehrere Indizes kombiniert und gemeinsame Operationen darauf ausführt.


**Learn more**

* [Search index repository](../https://docs.groupdocs.com/display/searchjava/Search+index+repository)


Das Beispiel demonstriert eine typische Verwendung der Klasse.

````
 ```

String indexFolder1 = "c:\\MyIndex\\";
String indexFolder2 = "c:\\MyIndex\\";
String query = "Einstein";
IndexRepository repository = new IndexRepository();
repository.addToRepository(indexFolder1); // Laden eines vorhandenen Index
repository.addToRepository(indexFolder2); // Laden eines weiteren vorhandenen Index
SearchResult result = repository.search(query); // Durchsuchen der Indizes des Repositorys
 
```
 
````


## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [IndexRepository()](#IndexRepository--) | Initialisiert eine neue Instanz von |
IndexRepository
Klasse.
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getEvents()](#getEvents--) | Ermittelt den Ereignis‑Hub zum Abonnieren von Ereignissen. |
|
|  | [getIndexes()](#getIndexes--) | Ruft die in diesem enthaltenen Indizes ab |
IndexRepository
.
|
|  | [close()](#close--) | Gibt alle vom System genutzten Ressourcen frei |
IndexRepository
.
|
|  | [create()](#create--) | Erstellt einen neuen Index im Speicher. |
|
|  | [create(IndexSettings settings)](#create-com.groupdocs.search.IndexSettings-) | Erstellt einen neuen Index im Speicher. |
|
|  | [create(String indexFolder)](#create-java.lang.String-) | Erstellt einen neuen Index auf der Festplatte. |
|
|  | [create(String indexFolder, IndexSettings settings)](#create-java.lang.String-com.groupdocs.search.IndexSettings-) | Erstellt einen neuen Index auf der Festplatte. |
|
|  | [addToRepository(Index index)](#addToRepository-com.groupdocs.search.Index-) | Fügt einen Index zum Index-Repository hinzu. |
|
|  | [addToRepository(String indexFolder)](#addToRepository-java.lang.String-) | Öffnet und fügt einen Index zum Index-Repository hinzu. |
|
|  | [update()](#update--) | Aktualisiert alle Indexe im Repository. |
|
|  | [update(UpdateOptions options)](#update-com.groupdocs.search.options.UpdateOptions-) | Aktualisiert alle Indexe im Repository. |
|
|  | [search(String query)](#search-java.lang.String-) | Durchsucht alle Indexe des Repositorys. |
|
|  | [search(String query, SearchOptions options)](#search-java.lang.String-com.groupdocs.search.options.SearchOptions-) | Durchsucht alle Indexe des Repositorys. |
|
|  | [search(SearchQuery query)](#search-com.groupdocs.search.SearchQuery-) | Durchsucht alle Indexe des Repositorys. |
|
|  | [search(SearchQuery query, SearchOptions options)](#search-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-) | Durchsucht alle Indexe des Repositorys. |
|
### IndexRepository() {#IndexRepository--}
```
public IndexRepository()
```


Initialisiert eine neue Instanz von
IndexRepository
Klasse.


### getEvents() {#getEvents--}
```
public final EventHub getEvents()
```


Ermittelt den Ereignis‑Hub zum Abonnieren von Ereignissen.


**Returns:**
[EventHub](../../com.groupdocs.search.events/eventhub) - The event hub for subscribing to events.

### getIndexes() {#getIndexes--}
```
public final Index[] getIndexes()
```


Ruft die in diesem enthaltenen Indizes ab
IndexRepository
.


**Returns:**
com.groupdocs.search.Index[] - Die Indexe.

### close() {#close--}
```
public final void close()
```


Gibt alle vom System genutzten Ressourcen frei
IndexRepository
.


### create() {#create--}
```
public final Index create()
```


Erstellt einen neuen Index im Speicher.


**Returns:**
[Index](../../com.groupdocs.search/index) - The created index.

Das Beispiel zeigt, wie man über das Index-Repository einen Index im Speicher erstellt.

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


Erstellt einen neuen Index im Speicher.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | Die Indexeinstellungen. |

Das Beispiel zeigt, wie man über das Index-Repository einen Index im Speicher erstellt.

````
 ```

IndexRepository indexRepository = new IndexRepository();
IndexSettings settings = new IndexSettings();
settings.setUseStopWords(false); // Deaktiviert die Verwendung von Stoppwörtern beim Indexieren
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


Erstellt einen neuen Index auf der Festplatte.
Der Indexordner wird vor der Indexerstellung bereinigt.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | indexFolder | java.lang.String | Der Indexordner. |

Das Beispiel zeigt, wie man über das Index-Repository einen Index auf der Festplatte erstellt.

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


Erstellt einen neuen Index auf der Festplatte.
Der Indexordner wird vor der Indexerstellung bereinigt.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | indexFolder | java.lang.String | Der Indexordner. |
|
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | Die Indexeinstellungen. |

Das Beispiel zeigt, wie man über das Index-Repository einen Index auf der Festplatte erstellt.

````
 ```

String indexFolder = "c:\\MyIndex\\";
IndexRepository indexRepository = new IndexRepository();
IndexSettings settings = new IndexSettings();
settings.setUseStopWords(false); // Deaktiviert die Verwendung von Stoppwörtern beim Indexieren
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


Fügt einen Index zum Index-Repository hinzu.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | index | [Index](../../com.groupdocs.search/index) | Der hinzuzufügende Index. |

Das Beispiel zeigt, wie man einen Index zum Index-Repository hinzufügt.

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


Öffnet und fügt einen Index zum Index-Repository hinzu.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | indexFolder | java.lang.String | Der Indexordner. |

Das Beispiel zeigt, wie man einen Index zum Index-Repository hinzufügt.

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


Aktualisiert alle Indexe im Repository.

Das Beispiel zeigt, wie man Indizes im Repository aktualisiert.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // Index erstellen
index.add(documentsFolder); // Dokumente indizieren
// Dokumente aus dem Dokumentenordner löschen oder sie ändern oder neue Dokumente zum Ordner hinzufügen
repository.update();
 
```
 
````



### update(UpdateOptions options) {#update-com.groupdocs.search.options.UpdateOptions-}
```
public final void update(UpdateOptions options)
```


Aktualisiert alle Indexe im Repository.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | options | [UpdateOptions](../../com.groupdocs.search.options/updateoptions) | Die Aktualisierungsoptionen. |

Das Beispiel zeigt, wie man Indizes im Repository aktualisiert.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // Index erstellen
index.add(documentsFolder); // Dokumente indizieren
// Dokumente aus dem Dokumentenordner löschen oder sie ändern oder neue Dokumente zum Ordner hinzufügen
UpdateOptions options = new UpdateOptions();
options.setThreads(2); // Festlegen der Anzahl von Indexierungs-Threads
repository.update(options);
 
```
 
````

|

### search(String query) {#search-java.lang.String-}
```
public final SearchResult search(String query)
```


Durchsucht alle Indexe des Repositorys.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | query | java.lang.String | Die Suchanfrage. |

Das Beispiel zeigt, wie man eine Suche im Index-Repository durchführt.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // Index erstellen
index.add(documentsFolder); // Dokumente indizieren
SearchResult result = repository.search(query); // Suche
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(String query, SearchOptions options) {#search-java.lang.String-com.groupdocs.search.options.SearchOptions-}
```
public final SearchResult search(String query, SearchOptions options)
```


Durchsucht alle Indexe des Repositorys.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | query | java.lang.String | Die Suchanfrage. |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | Die Suchoptionen. |

Das Beispiel zeigt, wie man eine Suche im Index-Repository durchführt.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // Index erstellen
index.add(documentsFolder); // Dokumente indizieren
SearchOptions options = new SearchOptions();
options.setUseCaseSensitiveSearch(true); // Festlegen des Flags für die Groß-/Kleinschreibung
SearchResult result = repository.search(query, options); // Suche
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(SearchQuery query) {#search-com.groupdocs.search.SearchQuery-}
```
public final SearchResult search(SearchQuery query)
```


Durchsucht alle Indexe des Repositorys.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | Die Suchanfrage. |

Das Beispiel zeigt, wie man eine Suche im Index-Repository durchführt.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // Index erstellen
index.add(documentsFolder); // Dokumente indizieren
SearchQuery query = SearchQuery.createWordQuery("Einstein"); // Erstellen einer Suchanfrage in Objektform
SearchResult result = repository.search(query); // Suche
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(SearchQuery query, SearchOptions options) {#search-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-}
```
public final SearchResult search(SearchQuery query, SearchOptions options)
```


Durchsucht alle Indexe des Repositorys.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | Die Suchanfrage. |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | Die Suchoptionen. |

Das Beispiel zeigt, wie man eine Suche im Index-Repository durchführt.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // Index erstellen
index.add(documentsFolder); // Dokumente indizieren
SearchOptions options = new SearchOptions();
options.setUseCaseSensitiveSearch(true); // Festlegen des Flags für die Groß-/Kleinschreibung
SearchQuery query = SearchQuery.createWordQuery("Einstein"); // Erstellen einer Suchanfrage in Objektform
SearchResult result = repository.search(query, options); // Suche
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

