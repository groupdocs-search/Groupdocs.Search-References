---
title: "IndexRepository"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Stelt een container voor het combineren van meerdere indexen en het uitvoeren van gemeenschappelijke bewerkingen daarop voor."
type: docs
weight: 18
url: /nl/java/com.groupdocs.search/indexrepository/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.io.Closeable
```
public class IndexRepository implements Closeable
```

Stelt een container voor het combineren van meerdere indexen en het uitvoeren van gemeenschappelijke bewerkingen daarop voor.


**Learn more**

* [Search index repository](../https://docs.groupdocs.com/display/searchjava/Search+index+repository)


Het voorbeeld toont een typisch gebruik van de klasse.

````
 ```

String indexFolder1 = "c:\\MyIndex\\";
String indexFolder2 = "c:\\MyIndex\\";
String query = "Einstein";
IndexRepository repository = new IndexRepository();
repository.addToRepository(indexFolder1); // Laden van een bestaande index
repository.addToRepository(indexFolder2); // Laden van een andere bestaande index
SearchResult result = repository.search(query); // Zoeken in indexen van de repository
 
```
 
````


## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [IndexRepository()](#IndexRepository--) | Initialiseert een nieuw exemplaar van de |
IndexRepository
klasse.
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getEvents()](#getEvents--) | Haalt de event-hub op voor het abonneren op gebeurtenissen. |
|
|  | [getIndexes()](#getIndexes--) | Haalt de indexen op die hierin zijn opgenomen |
IndexRepository
.
|
|  | [close()](#close--) | Geeft alle bronnen vrij die door de |
IndexRepository
.
|
|  | [create()](#create--) | Maakt een nieuwe index in het geheugen aan. |
|
|  | [create(IndexSettings settings)](#create-com.groupdocs.search.IndexSettings-) | Maakt een nieuwe index in het geheugen aan. |
|
|  | [create(String indexFolder)](#create-java.lang.String-) | Maakt een nieuwe index op schijf aan. |
|
|  | [create(String indexFolder, IndexSettings settings)](#create-java.lang.String-com.groupdocs.search.IndexSettings-) | Maakt een nieuwe index op schijf aan. |
|
|  | [addToRepository(Index index)](#addToRepository-com.groupdocs.search.Index-) | Voegt een index toe aan de indexrepository. |
|
|  | [addToRepository(String indexFolder)](#addToRepository-java.lang.String-) | Opent en voegt een index toe aan de indexrepository. |
|
|  | [update()](#update--) | Werkt alle indexen in de repository bij. |
|
|  | [update(UpdateOptions options)](#update-com.groupdocs.search.options.UpdateOptions-) | Werkt alle indexen in de repository bij. |
|
|  | [search(String query)](#search-java.lang.String-) | Zoekt in alle indexen van de repository. |
|
|  | [search(String query, SearchOptions options)](#search-java.lang.String-com.groupdocs.search.options.SearchOptions-) | Zoekt in alle indexen van de repository. |
|
|  | [search(SearchQuery query)](#search-com.groupdocs.search.SearchQuery-) | Zoekt in alle indexen van de repository. |
|
|  | [search(SearchQuery query, SearchOptions options)](#search-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-) | Zoekt in alle indexen van de repository. |
|
### IndexRepository() {#IndexRepository--}
```
public IndexRepository()
```


Initialiseert een nieuw exemplaar van de
IndexRepository
klasse.


### getEvents() {#getEvents--}
```
public final EventHub getEvents()
```


Haalt de event-hub op voor het abonneren op gebeurtenissen.


**Returns:**
[EventHub](../../com.groupdocs.search.events/eventhub) - The event hub for subscribing to events.

### getIndexes() {#getIndexes--}
```
public final Index[] getIndexes()
```


Haalt de indexen op die hierin zijn opgenomen
IndexRepository
.


**Returns:**
com.groupdocs.search.Index[] - De indexen.

### close() {#close--}
```
public final void close()
```


Geeft alle bronnen vrij die door de
IndexRepository
.


### create() {#create--}
```
public final Index create()
```


Maakt een nieuwe index in het geheugen aan.


**Returns:**
[Index](../../com.groupdocs.search/index) - The created index.

Het voorbeeld laat zien hoe je een index in het geheugen maakt via de indexrepository.

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


Maakt een nieuwe index in het geheugen aan.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | De indexinstellingen. |

Het voorbeeld laat zien hoe je een index in het geheugen maakt via de indexrepository.

````
 ```

IndexRepository indexRepository = new IndexRepository();
IndexSettings settings = new IndexSettings();
settings.setUseStopWords(false); // Het uitschakelen van het gebruik van stopwoorden tijdens het indexeren
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


Maakt een nieuwe index op schijf aan.
De indexmap wordt opgeschoond vóór de creatie van de index.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | indexFolder | java.lang.String | De indexmap. |

Het voorbeeld laat zien hoe je een index op schijf maakt via de indexrepository.

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


Maakt een nieuwe index op schijf aan.
De indexmap wordt opgeschoond vóór de creatie van de index.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | indexFolder | java.lang.String | De indexmap. |
|
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | De indexinstellingen. |

Het voorbeeld laat zien hoe je een index op schijf maakt via de indexrepository.

````
 ```

String indexFolder = "c:\\MyIndex\\";
IndexRepository indexRepository = new IndexRepository();
IndexSettings settings = new IndexSettings();
settings.setUseStopWords(false); // Het uitschakelen van het gebruik van stopwoorden tijdens het indexeren
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


Voegt een index toe aan de indexrepository.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | index | [Index](../../com.groupdocs.search/index) | De toe te voegen index. |

Het voorbeeld laat zien hoe je een index toevoegt aan de indexrepository.

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


Opent en voegt een index toe aan de indexrepository.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | indexFolder | java.lang.String | De indexmap. |

Het voorbeeld laat zien hoe je een index toevoegt aan de indexrepository.

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


Werkt alle indexen in de repository bij.

Het voorbeeld laat zien hoe indexen in de repository worden bijgewerkt.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // Index aanmaken
index.add(documentsFolder); // Documenten indexeren
// Verwijder documenten uit de documentmap of wijzig ze of voeg nieuwe documenten toe aan de map
repository.update();
 
```
 
````



### update(UpdateOptions options) {#update-com.groupdocs.search.options.UpdateOptions-}
```
public final void update(UpdateOptions options)
```


Werkt alle indexen in de repository bij.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | options | [UpdateOptions](../../com.groupdocs.search.options/updateoptions) | De update‑opties. |

Het voorbeeld laat zien hoe indexen in de repository worden bijgewerkt.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // Index aanmaken
index.add(documentsFolder); // Documenten indexeren
// Verwijder documenten uit de documentmap of wijzig ze of voeg nieuwe documenten toe aan de map
UpdateOptions options = new UpdateOptions();
options.setThreads(2); // Instellen van het aantal indexeer‑threads
repository.update(options);
 
```
 
````

|

### search(String query) {#search-java.lang.String-}
```
public final SearchResult search(String query)
```


Zoekt in alle indexen van de repository.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | query | java.lang.String | De zoekopdracht. |

Het voorbeeld laat zien hoe zoeken in de indexrepository wordt uitgevoerd.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // Index aanmaken
index.add(documentsFolder); // Documenten indexeren
SearchResult result = repository.search(query); // Zoeken
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(String query, SearchOptions options) {#search-java.lang.String-com.groupdocs.search.options.SearchOptions-}
```
public final SearchResult search(String query, SearchOptions options)
```


Zoekt in alle indexen van de repository.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | query | java.lang.String | De zoekopdracht. |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | De zoekopties. |

Het voorbeeld laat zien hoe zoeken in de indexrepository wordt uitgevoerd.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // Index aanmaken
index.add(documentsFolder); // Documenten indexeren
SearchOptions options = new SearchOptions();
options.setUseCaseSensitiveSearch(true); // Instellen van de vlag voor hoofdlettergevoelig zoeken
SearchResult result = repository.search(query, options); // Zoeken
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(SearchQuery query) {#search-com.groupdocs.search.SearchQuery-}
```
public final SearchResult search(SearchQuery query)
```


Zoekt in alle indexen van de repository.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | De zoekopdracht. |

Het voorbeeld laat zien hoe zoeken in de indexrepository wordt uitgevoerd.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // Index aanmaken
index.add(documentsFolder); // Documenten indexeren
SearchQuery query = SearchQuery.createWordQuery("Einstein"); // Zoekopdracht maken in objectvorm
SearchResult result = repository.search(query); // Zoeken
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(SearchQuery query, SearchOptions options) {#search-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-}
```
public final SearchResult search(SearchQuery query, SearchOptions options)
```


Zoekt in alle indexen van de repository.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | De zoekopdracht. |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | De zoekopties. |

Het voorbeeld laat zien hoe zoeken in de indexrepository wordt uitgevoerd.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // Index aanmaken
index.add(documentsFolder); // Documenten indexeren
SearchOptions options = new SearchOptions();
options.setUseCaseSensitiveSearch(true); // Instellen van de vlag voor hoofdlettergevoelig zoeken
SearchQuery query = SearchQuery.createWordQuery("Einstein"); // Zoekopdracht maken in objectvorm
SearchResult result = repository.search(query, options); // Zoeken
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

