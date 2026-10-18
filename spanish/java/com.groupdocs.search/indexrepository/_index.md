---
title: "IndexRepository"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Representa un contenedor para combinar múltiples índices y realizar operaciones comunes sobre ellos."
type: docs
weight: 18
url: /es/java/com.groupdocs.search/indexrepository/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.io.Closeable
```
public class IndexRepository implements Closeable
```

Representa un contenedor para combinar múltiples índices y realizar operaciones comunes sobre ellos.


**Learn more**

* [Search index repository](../https://docs.groupdocs.com/display/searchjava/Search+index+repository)


El ejemplo muestra un uso típico de la clase.

````
 ```

String indexFolder1 = "c:\\MyIndex\\";
String indexFolder2 = "c:\\MyIndex\\";
String query = "Einstein";
IndexRepository repository = new IndexRepository();
repository.addToRepository(indexFolder1); // Cargando un índice existente
repository.addToRepository(indexFolder2); // Cargando otro índice existente
SearchResult result = repository.search(query); // Buscando en los índices del repositorio
 
```
 
````


## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [IndexRepository()](#IndexRepository--) | Inicializa una nueva instancia de la |
IndexRepository
clase.
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getEvents()](#getEvents--) | Obtiene el hub de eventos para suscribirse a eventos. |
|
|  | [getIndexes()](#getIndexes--) | Obtiene los índices contenidos en este |
IndexRepository
.
|
|  | [close()](#close--) | Libera todos los recursos utilizados por el |
IndexRepository
.
|
|  | [create()](#create--) | Crea un nuevo índice en memoria. |
|
|  | [create(IndexSettings settings)](#create-com.groupdocs.search.IndexSettings-) | Crea un nuevo índice en memoria. |
|
|  | [create(String indexFolder)](#create-java.lang.String-) | Crea un nuevo índice en disco. |
|
|  | [create(String indexFolder, IndexSettings settings)](#create-java.lang.String-com.groupdocs.search.IndexSettings-) | Crea un nuevo índice en disco. |
|
|  | [addToRepository(Index index)](#addToRepository-com.groupdocs.search.Index-) | Agrega un índice al repositorio de índices. |
|
|  | [addToRepository(String indexFolder)](#addToRepository-java.lang.String-) | Abre y agrega un índice al repositorio de índices. |
|
|  | [update()](#update--) | Actualiza todos los índices en el repositorio. |
|
|  | [update(UpdateOptions options)](#update-com.groupdocs.search.options.UpdateOptions-) | Actualiza todos los índices en el repositorio. |
|
|  | [search(String query)](#search-java.lang.String-) | Busca en todos los índices del repositorio. |
|
|  | [search(String query, SearchOptions options)](#search-java.lang.String-com.groupdocs.search.options.SearchOptions-) | Busca en todos los índices del repositorio. |
|
|  | [search(SearchQuery query)](#search-com.groupdocs.search.SearchQuery-) | Busca en todos los índices del repositorio. |
|
|  | [search(SearchQuery query, SearchOptions options)](#search-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-) | Busca en todos los índices del repositorio. |
|
### IndexRepository() {#IndexRepository--}
```
public IndexRepository()
```


Inicializa una nueva instancia de la
IndexRepository
clase.


### getEvents() {#getEvents--}
```
public final EventHub getEvents()
```


Obtiene el hub de eventos para suscribirse a eventos.


**Returns:**
[EventHub](../../com.groupdocs.search.events/eventhub) - The event hub for subscribing to events.

### getIndexes() {#getIndexes--}
```
public final Index[] getIndexes()
```


Obtiene los índices contenidos en este
IndexRepository
.


**Returns:**
com.groupdocs.search.Index[] - Los índices.

### close() {#close--}
```
public final void close()
```


Libera todos los recursos utilizados por el
IndexRepository
.


### create() {#create--}
```
public final Index create()
```


Crea un nuevo índice en memoria.


**Returns:**
[Index](../../com.groupdocs.search/index) - The created index.

El ejemplo muestra cómo crear un índice en memoria a través del repositorio de índices.

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


Crea un nuevo índice en memoria.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | La configuración del índice. |

El ejemplo muestra cómo crear un índice en memoria a través del repositorio de índices.

````
 ```

IndexRepository indexRepository = new IndexRepository();
IndexSettings settings = new IndexSettings();
settings.setUseStopWords(false); // Desactivando el uso de palabras vacías durante la indexación
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


Crea un nuevo índice en disco.
La carpeta del índice se limpiará antes de crear el índice.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | indexFolder | java.lang.String | La carpeta del índice. |

El ejemplo muestra cómo crear un índice en disco a través del repositorio de índices.

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


Crea un nuevo índice en disco.
La carpeta del índice se limpiará antes de crear el índice.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | indexFolder | java.lang.String | La carpeta del índice. |
|
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | La configuración del índice. |

El ejemplo muestra cómo crear un índice en disco a través del repositorio de índices.

````
 ```

String indexFolder = "c:\\MyIndex\\";
IndexRepository indexRepository = new IndexRepository();
IndexSettings settings = new IndexSettings();
settings.setUseStopWords(false); // Desactivando el uso de palabras vacías durante la indexación
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


Agrega un índice al repositorio de índices.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | index | [Index](../../com.groupdocs.search/index) | El índice a agregar. |

El ejemplo muestra cómo agregar un índice al repositorio de índices.

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


Abre y agrega un índice al repositorio de índices.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | indexFolder | java.lang.String | La carpeta del índice. |

El ejemplo muestra cómo agregar un índice al repositorio de índices.

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


Actualiza todos los índices en el repositorio.

El ejemplo demuestra cómo actualizar índices en el repositorio.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // Creando índice
index.add(documentsFolder); // Indexando documentos
// Eliminar documentos de la carpeta de documentos o modificarlos o agregar nuevos documentos a la carpeta
repository.update();
 
```
 
````



### update(UpdateOptions options) {#update-com.groupdocs.search.options.UpdateOptions-}
```
public final void update(UpdateOptions options)
```


Actualiza todos los índices en el repositorio.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | options | [UpdateOptions](../../com.groupdocs.search.options/updateoptions) | Las opciones de actualización. |

El ejemplo demuestra cómo actualizar índices en el repositorio.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // Creando índice
index.add(documentsFolder); // Indexando documentos
// Eliminar documentos de la carpeta de documentos o modificarlos o agregar nuevos documentos a la carpeta
UpdateOptions options = new UpdateOptions();
options.setThreads(2); // Estableciendo el número de hilos de indexación
repository.update(options);
 
```
 
````

|

### search(String query) {#search-java.lang.String-}
```
public final SearchResult search(String query)
```


Busca en todos los índices del repositorio.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | query | java.lang.String | La consulta de búsqueda. |

El ejemplo demuestra cómo realizar búsquedas en el repositorio de índices.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // Creando índice
index.add(documentsFolder); // Indexando documentos
SearchResult result = repository.search(query); // Buscando
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(String query, SearchOptions options) {#search-java.lang.String-com.groupdocs.search.options.SearchOptions-}
```
public final SearchResult search(String query, SearchOptions options)
```


Busca en todos los índices del repositorio.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | query | java.lang.String | La consulta de búsqueda. |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | Las opciones de búsqueda. |

El ejemplo demuestra cómo realizar búsquedas en el repositorio de índices.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // Creando índice
index.add(documentsFolder); // Indexando documentos
SearchOptions options = new SearchOptions();
options.setUseCaseSensitiveSearch(true); // Estableciendo la bandera de búsqueda sensible a mayúsculas
SearchResult result = repository.search(query, options); // Buscando
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(SearchQuery query) {#search-com.groupdocs.search.SearchQuery-}
```
public final SearchResult search(SearchQuery query)
```


Busca en todos los índices del repositorio.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | La consulta de búsqueda. |

El ejemplo demuestra cómo realizar búsquedas en el repositorio de índices.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // Creando índice
index.add(documentsFolder); // Indexando documentos
SearchQuery query = SearchQuery.createWordQuery("Einstein"); // Creando consulta de búsqueda en forma de objeto
SearchResult result = repository.search(query); // Buscando
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(SearchQuery query, SearchOptions options) {#search-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-}
```
public final SearchResult search(SearchQuery query, SearchOptions options)
```


Busca en todos los índices del repositorio.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | La consulta de búsqueda. |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | Las opciones de búsqueda. |

El ejemplo demuestra cómo realizar búsquedas en el repositorio de índices.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // Creando índice
index.add(documentsFolder); // Indexando documentos
SearchOptions options = new SearchOptions();
options.setUseCaseSensitiveSearch(true); // Estableciendo la bandera de búsqueda sensible a mayúsculas
SearchQuery query = SearchQuery.createWordQuery("Einstein"); // Creando consulta de búsqueda en forma de objeto
SearchResult result = repository.search(query, options); // Buscando
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

