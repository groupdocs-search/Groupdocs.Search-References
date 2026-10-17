---
title: "IndexRepository"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Représente un conteneur permettant de combiner plusieurs index et d'exécuter des opérations communes sur ceux-ci."
type: docs
weight: 18
url: /fr/java/com.groupdocs.search/indexrepository/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.io.Closeable
```
public class IndexRepository implements Closeable
```

Représente un conteneur permettant de combiner plusieurs index et d'exécuter des opérations communes sur ceux-ci.


**Learn more**

* [Search index repository](../https://docs.groupdocs.com/display/searchjava/Search+index+repository)


L'exemple montre une utilisation typique de la classe.

````
 ```

String indexFolder1 = "c:\\MyIndex\\";
String indexFolder2 = "c:\\MyIndex\\";
String query = "Einstein";
IndexRepository repository = new IndexRepository();
repository.addToRepository(indexFolder1); // Chargement d'un index existant
repository.addToRepository(indexFolder2); // Chargement d'un autre index existant
SearchResult result = repository.search(query); // Recherche dans les index du référentiel
 
```
 
````


## Constructeurs

| Constructeur | Description |
| --- | --- |
|  | [IndexRepository()](#IndexRepository--) | Initialise une nouvelle instance de la |
IndexRepository
classe.
|
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getEvents()](#getEvents--) | Obtient le hub d'événements pour s'abonner aux événements. |
|
|  | [getIndexes()](#getIndexes--) | Obtient les index contenus dans cet objet |
IndexRepository
.
|
|  | [close()](#close--) | Libère toutes les ressources utilisées par le |
IndexRepository
.
|
|  | [create()](#create--) | Crée un nouvel index en mémoire. |
|
|  | [create(IndexSettings settings)](#create-com.groupdocs.search.IndexSettings-) | Crée un nouvel index en mémoire. |
|
|  | [create(String indexFolder)](#create-java.lang.String-) | Crée un nouvel index sur le disque. |
|
|  | [create(String indexFolder, IndexSettings settings)](#create-java.lang.String-com.groupdocs.search.IndexSettings-) | Crée un nouvel index sur le disque. |
|
|  | [addToRepository(Index index)](#addToRepository-com.groupdocs.search.Index-) | Ajoute un index au référentiel d'index. |
|
|  | [addToRepository(String indexFolder)](#addToRepository-java.lang.String-) | Ouvre et ajoute un index au référentiel d'index. |
|
|  | [update()](#update--) | Met à jour tous les index du référentiel. |
|
|  | [update(UpdateOptions options)](#update-com.groupdocs.search.options.UpdateOptions-) | Met à jour tous les index du référentiel. |
|
|  | [search(String query)](#search-java.lang.String-) | Recherche dans tous les index du référentiel. |
|
|  | [search(String query, SearchOptions options)](#search-java.lang.String-com.groupdocs.search.options.SearchOptions-) | Recherche dans tous les index du référentiel. |
|
|  | [search(SearchQuery query)](#search-com.groupdocs.search.SearchQuery-) | Recherche dans tous les index du référentiel. |
|
|  | [search(SearchQuery query, SearchOptions options)](#search-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-) | Recherche dans tous les index du référentiel. |
|
### IndexRepository() {#IndexRepository--}
```
public IndexRepository()
```


Initialise une nouvelle instance de la
IndexRepository
classe.


### getEvents() {#getEvents--}
```
public final EventHub getEvents()
```


Obtient le hub d'événements pour s'abonner aux événements.


**Returns:**
[EventHub](../../com.groupdocs.search.events/eventhub) - The event hub for subscribing to events.

### getIndexes() {#getIndexes--}
```
public final Index[] getIndexes()
```


Obtient les index contenus dans cet objet
IndexRepository
.


**Returns:**
com.groupdocs.search.Index[] - Les index.

### close() {#close--}
```
public final void close()
```


Libère toutes les ressources utilisées par le
IndexRepository
.


### create() {#create--}
```
public final Index create()
```


Crée un nouvel index en mémoire.


**Returns:**
[Index](../../com.groupdocs.search/index) - The created index.

L'exemple montre comment créer un index en mémoire via le référentiel d'index.

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


Crée un nouvel index en mémoire.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | Les paramètres de l'index. |

L'exemple montre comment créer un index en mémoire via le référentiel d'index.

````
 ```

IndexRepository indexRepository = new IndexRepository();
IndexSettings settings = new IndexSettings();
settings.setUseStopWords(false); // Désactivation de l'utilisation des mots vides lors de l'indexation
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


Crée un nouvel index sur le disque.
Le dossier d'index sera nettoyé avant la création de l'index.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | indexFolder | java.lang.String | Le dossier d'index. |

L'exemple montre comment créer un index sur le disque via le référentiel d'index.

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


Crée un nouvel index sur le disque.
Le dossier d'index sera nettoyé avant la création de l'index.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | indexFolder | java.lang.String | Le dossier d'index. |
|
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | Les paramètres de l'index. |

L'exemple montre comment créer un index sur le disque via le référentiel d'index.

````
 ```

String indexFolder = "c:\\MyIndex\\";
IndexRepository indexRepository = new IndexRepository();
IndexSettings settings = new IndexSettings();
settings.setUseStopWords(false); // Désactivation de l'utilisation des mots vides lors de l'indexation
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


Ajoute un index au référentiel d'index.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | index | [Index](../../com.groupdocs.search/index) | L'index à ajouter. |

L'exemple montre comment ajouter un index au référentiel d'index.

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


Ouvre et ajoute un index au référentiel d'index.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | indexFolder | java.lang.String | Le dossier d'index. |

L'exemple montre comment ajouter un index au référentiel d'index.

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


Met à jour tous les index du référentiel.

L'exemple montre comment mettre à jour les index dans le référentiel.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // Création de l'index
index.add(documentsFolder); // Indexation des documents
// Supprimer les documents du dossier de documents ou les modifier ou ajouter de nouveaux documents au dossier
repository.update();
 
```
 
````



### update(UpdateOptions options) {#update-com.groupdocs.search.options.UpdateOptions-}
```
public final void update(UpdateOptions options)
```


Met à jour tous les index du référentiel.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | options | [UpdateOptions](../../com.groupdocs.search.options/updateoptions) | Les options de mise à jour. |

L'exemple montre comment mettre à jour les index dans le référentiel.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // Création de l'index
index.add(documentsFolder); // Indexation des documents
// Supprimer les documents du dossier de documents ou les modifier ou ajouter de nouveaux documents au dossier
UpdateOptions options = new UpdateOptions();
options.setThreads(2); // Définition du nombre de threads d'indexation
repository.update(options);
 
```
 
````

|

### search(String query) {#search-java.lang.String-}
```
public final SearchResult search(String query)
```


Recherche dans tous les index du référentiel.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | query | java.lang.String | La requête de recherche. |

L'exemple montre comment effectuer une recherche dans le référentiel d'index.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // Création de l'index
index.add(documentsFolder); // Indexation des documents
SearchResult result = repository.search(query); // Recherche
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(String query, SearchOptions options) {#search-java.lang.String-com.groupdocs.search.options.SearchOptions-}
```
public final SearchResult search(String query, SearchOptions options)
```


Recherche dans tous les index du référentiel.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | query | java.lang.String | La requête de recherche. |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | Les options de recherche. |

L'exemple montre comment effectuer une recherche dans le référentiel d'index.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // Création de l'index
index.add(documentsFolder); // Indexation des documents
SearchOptions options = new SearchOptions();
options.setUseCaseSensitiveSearch(true); // Définition du drapeau de recherche sensible à la casse
SearchResult result = repository.search(query, options); // Recherche
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(SearchQuery query) {#search-com.groupdocs.search.SearchQuery-}
```
public final SearchResult search(SearchQuery query)
```


Recherche dans tous les index du référentiel.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | La requête de recherche. |

L'exemple montre comment effectuer une recherche dans le référentiel d'index.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // Création de l'index
index.add(documentsFolder); // Indexation des documents
SearchQuery query = SearchQuery.createWordQuery("Einstein"); // Création de la requête de recherche sous forme d'objet
SearchResult result = repository.search(query); // Recherche
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(SearchQuery query, SearchOptions options) {#search-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-}
```
public final SearchResult search(SearchQuery query, SearchOptions options)
```


Recherche dans tous les index du référentiel.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | La requête de recherche. |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | Les options de recherche. |

L'exemple montre comment effectuer une recherche dans le référentiel d'index.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // Création de l'index
index.add(documentsFolder); // Indexation des documents
SearchOptions options = new SearchOptions();
options.setUseCaseSensitiveSearch(true); // Définition du drapeau de recherche sensible à la casse
SearchQuery query = SearchQuery.createWordQuery("Einstein"); // Création de la requête de recherche sous forme d'objet
SearchResult result = repository.search(query, options); // Recherche
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

