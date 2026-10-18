---
title: "IndexRepository"
second_title: "GroupDocs.Search för Java API-referens"
description: "Representerar en behållare för att kombinera flera index och utföra vanliga operationer på dem."
type: docs
weight: 18
url: /sv/java/com.groupdocs.search/indexrepository/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.io.Closeable
```
public class IndexRepository implements Closeable
```

Representerar en behållare för att kombinera flera index och utföra vanliga operationer på dem.


**Learn more**

* [Search index repository](../https://docs.groupdocs.com/display/searchjava/Search+index+repository)


Exemplet demonstrerar ett typiskt användningssätt av klassen.

````
 ```

String indexFolder1 = "c:\\MyIndex\\";
String indexFolder2 = "c:\\MyIndex\\";
String query = "Einstein";
IndexRepository repository = new IndexRepository();
repository.addToRepository(indexFolder1); // Laddar ett befintligt index
repository.addToRepository(indexFolder2); // Laddar ett annat befintligt index
SearchResult result = repository.search(query); // Söker i indexen i lagret
 
```
 
````


## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [IndexRepository()](#IndexRepository--) | Initierar en ny instans av |
IndexRepository
klassen.
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getEvents()](#getEvents--) | Hämtar händelsehubben för att prenumerera på händelser. |
|
|  | [getIndexes()](#getIndexes--) | Hämtar indexen som finns i detta |
IndexRepository
.
|
|  | [close()](#close--) | Frigör alla resurser som används av |
IndexRepository
.
|
|  | [create()](#create--) | Skapar ett nytt index i minnet. |
|
|  | [create(IndexSettings settings)](#create-com.groupdocs.search.IndexSettings-) | Skapar ett nytt index i minnet. |
|
|  | [create(String indexFolder)](#create-java.lang.String-) | Skapar ett nytt index på disk. |
|
|  | [create(String indexFolder, IndexSettings settings)](#create-java.lang.String-com.groupdocs.search.IndexSettings-) | Skapar ett nytt index på disk. |
|
|  | [addToRepository(Index index)](#addToRepository-com.groupdocs.search.Index-) | Lägger till ett index i indexförrådet. |
|
|  | [addToRepository(String indexFolder)](#addToRepository-java.lang.String-) | Öppnar och lägger till ett index i indexförrådet. |
|
|  | [update()](#update--) | Uppdaterar alla index i förrådet. |
|
|  | [update(UpdateOptions options)](#update-com.groupdocs.search.options.UpdateOptions-) | Uppdaterar alla index i förrådet. |
|
|  | [search(String query)](#search-java.lang.String-) | Söker i alla index i förrådet. |
|
|  | [search(String query, SearchOptions options)](#search-java.lang.String-com.groupdocs.search.options.SearchOptions-) | Söker i alla index i förrådet. |
|
|  | [search(SearchQuery query)](#search-com.groupdocs.search.SearchQuery-) | Söker i alla index i förrådet. |
|
|  | [search(SearchQuery query, SearchOptions options)](#search-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-) | Söker i alla index i förrådet. |
|
### IndexRepository() {#IndexRepository--}
```
public IndexRepository()
```


Initierar en ny instans av
IndexRepository
klassen.


### getEvents() {#getEvents--}
```
public final EventHub getEvents()
```


Hämtar händelsehubben för att prenumerera på händelser.


**Returns:**
[EventHub](../../com.groupdocs.search.events/eventhub) - The event hub for subscribing to events.

### getIndexes() {#getIndexes--}
```
public final Index[] getIndexes()
```


Hämtar indexen som finns i detta
IndexRepository
.


**Returns:**
com.groupdocs.search.Index[] - Indexen.

### close() {#close--}
```
public final void close()
```


Frigör alla resurser som används av
IndexRepository
.


### create() {#create--}
```
public final Index create()
```


Skapar ett nytt index i minnet.


**Returns:**
[Index](../../com.groupdocs.search/index) - The created index.

Exemplet visar hur man skapar ett index i minnet via indexförrådet.

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


Skapar ett nytt index i minnet.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | Indexinställningarna. |

Exemplet visar hur man skapar ett index i minnet via indexförrådet.

````
 ```

IndexRepository indexRepository = new IndexRepository();
IndexSettings settings = new IndexSettings();
settings.setUseStopWords(false); // Inaktiverar användning av stoppord under indexering
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


Skapar ett nytt index på disk.
Indexmappen kommer att rensas innan indexet skapas.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | indexFolder | java.lang.String | Indexmappen. |

Exemplet visar hur man skapar ett index på disk via indexförrådet.

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


Skapar ett nytt index på disk.
Indexmappen kommer att rensas innan indexet skapas.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | indexFolder | java.lang.String | Indexmappen. |
|
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | Indexinställningarna. |

Exemplet visar hur man skapar ett index på disk via indexförrådet.

````
 ```

String indexFolder = "c:\\MyIndex\\";
IndexRepository indexRepository = new IndexRepository();
IndexSettings settings = new IndexSettings();
settings.setUseStopWords(false); // Inaktiverar användning av stoppord under indexering
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


Lägger till ett index i indexförrådet.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | index | [Index](../../com.groupdocs.search/index) | Indexet att lägga till. |

Exemplet visar hur man lägger till ett index i indexförrådet.

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


Öppnar och lägger till ett index i indexförrådet.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | indexFolder | java.lang.String | Indexmappen. |

Exemplet visar hur man lägger till ett index i indexförrådet.

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


Uppdaterar alla index i förrådet.

Exemplet visar hur man uppdaterar index i lagret.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // Skapar index
index.add(documentsFolder); // Indexerar dokument
// Radera dokument från dokumentmappen eller ändra dem eller lägg till nya dokument i mappen
repository.update();
 
```
 
````



### update(UpdateOptions options) {#update-com.groupdocs.search.options.UpdateOptions-}
```
public final void update(UpdateOptions options)
```


Uppdaterar alla index i förrådet.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | options | [UpdateOptions](../../com.groupdocs.search.options/updateoptions) | Uppdateringsalternativen. |

Exemplet visar hur man uppdaterar index i lagret.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // Skapar index
index.add(documentsFolder); // Indexerar dokument
// Radera dokument från dokumentmappen eller ändra dem eller lägg till nya dokument i mappen
UpdateOptions options = new UpdateOptions();
options.setThreads(2); // Ställer in antalet indexeringstrådar
repository.update(options);
 
```
 
````

|

### search(String query) {#search-java.lang.String-}
```
public final SearchResult search(String query)
```


Söker i alla index i förrådet.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | query | java.lang.String | Sökfrågan. |

Exemplet visar hur man utför sökning i indexlagret.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // Skapar index
index.add(documentsFolder); // Indexerar dokument
SearchResult result = repository.search(query); // Söker
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(String query, SearchOptions options) {#search-java.lang.String-com.groupdocs.search.options.SearchOptions-}
```
public final SearchResult search(String query, SearchOptions options)
```


Söker i alla index i förrådet.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | query | java.lang.String | Sökfrågan. |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | Sökalternativen. |

Exemplet visar hur man utför sökning i indexlagret.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // Skapar index
index.add(documentsFolder); // Indexerar dokument
SearchOptions options = new SearchOptions();
options.setUseCaseSensitiveSearch(true); // Ställer in flaggan för skiftlägeskänslig sökning
SearchResult result = repository.search(query, options); // Söker
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(SearchQuery query) {#search-com.groupdocs.search.SearchQuery-}
```
public final SearchResult search(SearchQuery query)
```


Söker i alla index i förrådet.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | Sökfrågan. |

Exemplet visar hur man utför sökning i indexlagret.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // Skapar index
index.add(documentsFolder); // Indexerar dokument
SearchQuery query = SearchQuery.createWordQuery("Einstein"); // Skapar sökfråga i objektform
SearchResult result = repository.search(query); // Söker
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(SearchQuery query, SearchOptions options) {#search-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-}
```
public final SearchResult search(SearchQuery query, SearchOptions options)
```


Söker i alla index i förrådet.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | Sökfrågan. |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | Sökalternativen. |

Exemplet visar hur man utför sökning i indexlagret.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // Skapar index
index.add(documentsFolder); // Indexerar dokument
SearchOptions options = new SearchOptions();
options.setUseCaseSensitiveSearch(true); // Ställer in flaggan för skiftlägeskänslig sökning
SearchQuery query = SearchQuery.createWordQuery("Einstein"); // Skapar sökfråga i objektform
SearchResult result = repository.search(query, options); // Söker
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

