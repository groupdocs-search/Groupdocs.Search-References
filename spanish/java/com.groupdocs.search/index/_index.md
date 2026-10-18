---
title: "Índice"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Representa la clase principal para indexar documentos y buscar a través de ellos."
type: docs
weight: 17
url: /es/java/com.groupdocs.search/index/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.io.Closeable
```
public class Index implements Closeable
```

Representa la clase principal para indexar documentos y buscar a través de ellos.


**Learn more**

* [Creating an index](../https://docs.groupdocs.com/display/searchjava/Creating+an+index)
* [Indexing](../https://docs.groupdocs.com/display/searchjava/Indexing)
* [Searching](../https://docs.groupdocs.com/display/searchjava/Searching)


El ejemplo muestra un uso típico de la clase.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // Creando índice en la carpeta especificada
index.add(documentsFolder); // Indexando documentos de la carpeta especificada
SearchResult result = index.search(query); // Buscando en el índice
 
```
 
````


## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [Index()](#Index--) | Inicializa una nueva instancia de la  Index  clase en memoria. |
|
|  | [Index(IndexSettings settings)](#Index-com.groupdocs.search.IndexSettings-) | Inicializa una nueva instancia de la  Index  clase en memoria con configuraciones de índice particulares. |
|
|  | [Index(String indexFolder)](#Index-java.lang.String-) | Inicializa una nueva instancia de la  Index  clase. |
|
|  | [Index(String indexFolder, IndexSettings settings)](#Index-java.lang.String-com.groupdocs.search.IndexSettings-) | Inicializa una nueva instancia de la |
Índice
clase.
|
|  | [Index(String indexFolder, boolean overwriteIfExists)](#Index-java.lang.String-boolean-) | Inicializa una nueva instancia de la |
Índice
clase.
|
|  | [Index(String indexFolder, IndexSettings settings, boolean overwriteIfExists)](#Index-java.lang.String-com.groupdocs.search.IndexSettings-boolean-) | Inicializa una nueva instancia de la |
Índice
clase.
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getEvents()](#getEvents--) | Obtiene el hub de eventos para suscribirse a eventos. |
|
|  | [getIndexInfo()](#getIndexInfo--) | Obtiene la información básica del índice. |
|
|  | [getRepository()](#getRepository--) | Obtiene el objeto del repositorio de índices si el índice está contenido en él. |
|
|  | [getIndexSettings()](#getIndexSettings--) | Obtiene la configuración del índice. |
|
|  | [getDictionaries()](#getDictionaries--) | Obtiene el repositorio del diccionario. |
|
|  | [close()](#close--) | Libera todos los recursos utilizados por el |
Índice
.
|
|  | [add(String path)](#add-java.lang.String-) | Realiza la operación de indexación. |
|
|  | [add(String path, IndexingOptions options)](#add-java.lang.String-com.groupdocs.search.options.IndexingOptions-) | Realiza la operación de indexación. |
|
|  | [add(String[] paths)](#add-java.lang.String---) | Realiza la operación de indexación. |
|
|  | [add(String[] paths, IndexingOptions options)](#add-java.lang.String---com.groupdocs.search.options.IndexingOptions-) | Realiza la operación de indexación. |
|
|  | [add(Document[] documents, IndexingOptions options)](#add-com.groupdocs.search.Document---com.groupdocs.search.options.IndexingOptions-) | Realiza la operación de indexación. |
|
|  | [add(ExtractedData[] data, IndexingOptions options)](#add-com.groupdocs.search.ExtractedData---com.groupdocs.search.options.IndexingOptions-) | Realiza la operación de indexación. |
|
|  | [update()](#update--) | Re-indexa documentos que han sido modificados o eliminados desde la última actualización. |
|
|  | [update(UpdateOptions options)](#update-com.groupdocs.search.options.UpdateOptions-) | Re-indexa documentos que han sido modificados o eliminados desde la última actualización. |
|
|  | [getIndexingReports()](#getIndexingReports--) | Obtiene los informes sobre operaciones de indexación. |
|
|  | [getSearchReports()](#getSearchReports--) | Obtiene los informes sobre operaciones de búsqueda. |
|
|  | [search(String query)](#search-java.lang.String-) | Busca en el índice. |
|
|  | [search(String query, SearchOptions options)](#search-java.lang.String-com.groupdocs.search.options.SearchOptions-) | Busca en el índice. |
|
|  | [search(SearchQuery query)](#search-com.groupdocs.search.SearchQuery-) | Busca en el índice. |
|
|  | [search(SearchQuery query, SearchOptions options)](#search-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-) | Busca en el índice. |
|
|  | [search(SearchImage image, ImageSearchOptions options)](#search-com.groupdocs.search.common.SearchImage-com.groupdocs.search.options.ImageSearchOptions-) | Realiza una búsqueda inversa de imágenes en el índice. |
|
|  | [searchNext(ChunkSearchToken chunkSearchToken)](#searchNext-com.groupdocs.search.common.ChunkSearchToken-) | Continúa la búsqueda por fragmentos iniciada con el método Search. |
|
|  | [searchNext(ChunkSearchToken chunkSearchToken, Cancellation cancellation)](#searchNext-com.groupdocs.search.common.ChunkSearchToken-com.groupdocs.search.common.Cancellation-) | Continúa la búsqueda por fragmentos iniciada con el método Search. |
|
|  | [optimize()](#optimize--) | Minimiza el número de segmentos del índice fusionándolos uno con otro. |
|
|  | [optimize(MergeOptions options)](#optimize-com.groupdocs.search.options.MergeOptions-) | Minimiza el número de segmentos del índice fusionándolos uno con otro. |
|
|  | [merge(Index index, MergeOptions options)](#merge-com.groupdocs.search.Index-com.groupdocs.search.options.MergeOptions-) | Fusiona el índice especificado en el índice actual. |
|
|  | [merge(IndexRepository repository, MergeOptions options)](#merge-com.groupdocs.search.IndexRepository-com.groupdocs.search.options.MergeOptions-) | Fusiona índices del repositorio de índices especificado en el índice actual. |
|
|  | [highlight(FoundDocument document, Highlighter highlighter)](#highlight-com.groupdocs.search.results.FoundDocument-com.groupdocs.search.highlighters.Highlighter-) | Genera texto con formato HTML con los términos encontrados resaltados. |
|
|  | [highlight(FoundDocument document, Highlighter highlighter, HighlightOptions options)](#highlight-com.groupdocs.search.results.FoundDocument-com.groupdocs.search.highlighters.Highlighter-com.groupdocs.search.options.HighlightOptions-) | Genera texto con formato HTML con los términos encontrados resaltados. |
|
|  | [getIndexedDocuments()](#getIndexedDocuments--) | Obtiene una matriz de todos los documentos indexados. |
|
|  | [getIndexedDocumentItems(DocumentInfo documentInfo)](#getIndexedDocumentItems-com.groupdocs.search.results.DocumentInfo-) | Obtiene una matriz de elementos de documento. |
|
|  | [GetIndexedDocument(String documentKey)](#GetIndexedDocument-java.lang.String-) | Obtiene un documento indexado por clave de documento. |
|
|  | [getDocumentText(DocumentInfo documentInfo, OutputAdapter adapter)](#getDocumentText-com.groupdocs.search.results.DocumentInfo-com.groupdocs.search.common.OutputAdapter-) | Genera el texto de un documento indexado y lo pasa a través de un adaptador de salida. |
|
|  | [getDocumentText(DocumentInfo documentInfo, OutputAdapter adapter, TextOptions options)](#getDocumentText-com.groupdocs.search.results.DocumentInfo-com.groupdocs.search.common.OutputAdapter-com.groupdocs.search.options.TextOptions-) | Genera texto con formato HTML para el documento indexado y lo transfiere a través del adaptador de salida. |
|
|  | [getIndexedPaths()](#getIndexedPaths--) | Obtiene una matriz de rutas indexadas: documentos o carpetas. |
|
|  | [delete(String[] paths, UpdateOptions options)](#delete-java.lang.String---com.groupdocs.search.options.UpdateOptions-) | Elimina archivos o carpetas indexados del índice. |
|
|  | [delete(UpdateOptions options, String[] documentKeys)](#delete-com.groupdocs.search.options.UpdateOptions-java.lang.String---) | Elimina documentos indexados de flujos o estructuras. |
|
|  | [notifyIndex(Notification notification)](#notifyIndex-com.groupdocs.search.Notification-) | Pasa el objeto de notificación especificado al índice para realizar la notificación. |
|
|  | [changeAttributes(AttributeChangeBatch batch)](#changeAttributes-com.groupdocs.search.common.AttributeChangeBatch-) | Aplica el lote especificado de cambios de atributos a documentos indexados sin reindexar durante la operación de actualización. |
|
|  | [getAttributes(String path)](#getAttributes-java.lang.String-) | Obtiene todos los atributos asociados con el documento indexado especificado. |
|
|  | [loadIntoMemoryCompletely(String indexFolder)](#loadIntoMemoryCompletely-java.lang.String-) | Carga todo el índice en la memoria. |
|
|  | [loadIntoMemoryCompletely(String indexFolder, IndexSettings settings)](#loadIntoMemoryCompletely-java.lang.String-com.groupdocs.search.IndexSettings-) | Carga todo el índice en la memoria. |
|
### Index() {#Index--}
```
public Index()
```


Inicializa una nueva instancia de la  Index  clase en memoria.


El ejemplo muestra cómo crear un índice en memoria sin guardar archivos en disco.

````
 ```

Index index = new Index();
 
```
 
````



### Index(IndexSettings settings) {#Index-com.groupdocs.search.IndexSettings-}
```
public Index(IndexSettings settings)
```


Inicializa una nueva instancia de la  Index  clase en memoria con configuraciones de índice particulares.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | El objeto de configuración del índice. |


El ejemplo muestra cómo crear un índice en memoria sin guardar archivos en disco con configuraciones de índice particulares.

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


Inicializa una nueva instancia de la clase  Index . Crea una nueva o abre un índice existente en disco.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | indexFolder | java.lang.String | La ruta de la carpeta del índice. |


El ejemplo muestra cómo crear un índice en un disco o abrir un índice existente.

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


Inicializa una nueva instancia de la
Índice
clase.
Crea un nuevo índice con configuraciones particulares o abre un índice existente en disco.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | indexFolder | java.lang.String | La ruta de la carpeta del índice. |
|
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | El objeto de configuración del índice. |

El ejemplo muestra cómo crear un índice en un disco con configuraciones de índice particulares.

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


Inicializa una nueva instancia de la
Índice
clase.
Carga un índice existente desde el disco si
overwriteIfExists
is
false
;
crea un nuevo índice en el disco de lo contrario.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | indexFolder | java.lang.String | La ruta de la carpeta del índice. |
|
|  | overwriteIfExists | boolean | La bandera de sobrescribir la carpeta del índice. |

El ejemplo muestra cómo crear un nuevo índice en una carpeta que ya contiene otro índice.

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


Inicializa una nueva instancia de la
Índice
clase.
Carga un índice existente desde el disco si
overwriteIfExists
is
false
;
crea un nuevo índice en el disco con configuraciones de índice particulares de lo contrario.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | indexFolder | java.lang.String | La ruta de la carpeta del índice. |
|
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | El objeto de configuración del índice. |
|
|  | overwriteIfExists | boolean | La bandera de sobrescribir la carpeta del índice. |

El ejemplo muestra cómo crear un índice en un disco con configuraciones de índice particulares.

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


Obtiene el hub de eventos para suscribirse a eventos.


**Returns:**
[EventHub](../../com.groupdocs.search.events/eventhub) - The event hub for subscribing to events.

### getIndexInfo() {#getIndexInfo--}
```
public final IndexInfo getIndexInfo()
```


Obtiene la información básica del índice.


**Returns:**
[IndexInfo](../../com.groupdocs.search.common/indexinfo) - The basic information on the index.

### getRepository() {#getRepository--}
```
public final IndexRepository getRepository()
```


Obtiene el objeto del repositorio de índices si el índice está contenido en él.


**Returns:**
[IndexRepository](../../com.groupdocs.search/indexrepository) - The index repository object.

### getIndexSettings() {#getIndexSettings--}
```
public final IndexSettings getIndexSettings()
```


Obtiene la configuración del índice.


**Returns:**
[IndexSettings](../../com.groupdocs.search/indexsettings) - The index settings.

### getDictionaries() {#getDictionaries--}
```
public final DictionaryRepository getDictionaries()
```


Obtiene el repositorio del diccionario.


**Returns:**
[DictionaryRepository](../../com.groupdocs.search.dictionaries/dictionaryrepository) - The dictionary repository.

### close() {#close--}
```
public final void close()
```


Libera todos los recursos utilizados por el
Índice
.


### add(String path) {#add-java.lang.String-}
```
public final void add(String path)
```


Realiza la operación de indexación.
Agrega un archivo o carpeta mediante una ruta absoluta o relativa.
Los documentos de todas las subcarpetas serán indexados.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | path | java.lang.String | La ruta a un archivo o carpeta que será indexado. |

El ejemplo muestra cómo agregar documentos a un índice.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String folderPath = "c:\\MyDocuments\\";
String filePath = "c:\\Documents\\MyFile.txt";
Index index = new Index(indexFolder); // Creando índice en la carpeta especificada
index.add(folderPath); // Indexando documentos en la carpeta especificada
index.add(filePath); // Indexando el documento especificado
 
```
 
````

|

### add(String path, IndexingOptions options) {#add-java.lang.String-com.groupdocs.search.options.IndexingOptions-}
```
public final void add(String path, IndexingOptions options)
```


Realiza la operación de indexación.
Agrega un archivo o carpeta mediante una ruta absoluta o relativa.
Los documentos de todas las subcarpetas serán indexados.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | path | java.lang.String | La ruta a un archivo o carpeta que será indexado. |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | Las opciones de indexación. |

El ejemplo muestra cómo agregar documentos a un índice con opciones de indexación particulares.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String folderPath = "c:\\MyDocuments\\";
String filePath = "c:\\Documents\\MyFile.txt";
Index index = new Index(indexFolder); // Creando índice en la carpeta especificada
IndexingOptions options = new IndexingOptions();
options.setThreads(2); // Estableciendo el número de hilos de indexación
index.add(folderPath, options); // Indexando documentos en la carpeta especificada
index.add(filePath, options); // Indexando el documento especificado
 
```
 
````

|

### add(String[] paths) {#add-java.lang.String---}
```
public final void add(String[] paths)
```


Realiza la operación de indexación.
Agrega archivos o carpetas mediante una ruta absoluta o relativa.
Los documentos de todas las subcarpetas serán indexados.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | paths | java.lang.String[] | Las rutas a los archivos o carpetas que se indexarán. |

El ejemplo muestra cómo agregar documentos a un índice.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String folderPath = "c:\\MyDocuments\\";
String filePath = "c:\\Documents\\MyFile.txt";
Index index = new Index(indexFolder); // Creando índice en la carpeta especificada
String[] paths = new String[] { folderPath, filePath };
index.add(paths); // Indexando documentos en las rutas especificadas
 
```
 
````

|

### add(String[] paths, IndexingOptions options) {#add-java.lang.String---com.groupdocs.search.options.IndexingOptions-}
```
public final void add(String[] paths, IndexingOptions options)
```


Realiza la operación de indexación.
Agrega archivos o carpetas mediante una ruta absoluta o relativa.
Los documentos de todas las subcarpetas serán indexados.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | paths | java.lang.String[] | Las rutas a los archivos o carpetas que se indexarán. |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | Las opciones de indexación. |

El ejemplo muestra cómo agregar documentos a un índice con opciones de indexación particulares.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String folderPath = "c:\\MyDocuments\\";
String filePath = "c:\\Documents\\MyFile.txt";
Index index = new Index(indexFolder); // Creando índice en la carpeta especificada
IndexingOptions options = new IndexingOptions();
options.setThreads(2); // Estableciendo el número de hilos de indexación
String[] paths = new String[] { folderPath, filePath };
index.add(paths, options); // Indexando documentos en las rutas especificadas
 
```
 
````

|

### add(Document[] documents, IndexingOptions options) {#add-com.groupdocs.search.Document---com.groupdocs.search.options.IndexingOptions-}
```
public final void add(Document[] documents, IndexingOptions options)
```


Realiza la operación de indexación.
Agrega documentos desde el sistema de archivos, flujo o estructura.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | documents | [Document\[\]](../../com.groupdocs.search/document) | Los documentos del sistema de archivos, flujo o estructura. |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | Las opciones de indexación. |
|

### add(ExtractedData[] data, IndexingOptions options) {#add-com.groupdocs.search.ExtractedData---com.groupdocs.search.options.IndexingOptions-}
```
public final void add(ExtractedData[] data, IndexingOptions options)
```


Realiza la operación de indexación.
Agrega los datos extraídos al índice.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | data | [ExtractedData\[\]](../../com.groupdocs.search/extracteddata) | Los datos extraídos. |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | Las opciones de indexación. |
|

### update() {#update--}
```
public final void update()
```


Re-indexa documentos que han sido modificados o eliminados desde la última actualización.
Agrega nuevos archivos que se han añadido a las carpetas indexadas.

El ejemplo muestra cómo actualizar un índice.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Creando índice en la carpeta especificada
index.add(documentsFolder); // Indexando documentos de la carpeta especificada
// Eliminar documentos de la carpeta de documentos o modificarlos o agregar nuevos documentos a la carpeta
index.update(); // Actualizando el índice
 
```
 
````



### update(UpdateOptions options) {#update-com.groupdocs.search.options.UpdateOptions-}
```
public final void update(UpdateOptions options)
```


Re-indexa documentos que han sido modificados o eliminados desde la última actualización.
Agrega nuevos archivos que se han añadido a las carpetas indexadas.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | options | [UpdateOptions](../../com.groupdocs.search.options/updateoptions) | Las opciones de actualización. |

El ejemplo muestra cómo actualizar un índice con opciones de actualización particulares.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Creando índice en la carpeta especificada
index.add(documentsFolder); // Indexando documentos de la carpeta especificada
// Eliminar documentos de la carpeta de documentos o modificarlos o agregar nuevos documentos a la carpeta
UpdateOptions options = new UpdateOptions();
options.setThreads(2); // Estableciendo el número de hilos de indexación
index.update(options); // Actualizando el índice
 
```
 
````

|

### getIndexingReports() {#getIndexingReports--}
```
public final IndexingReport[] getIndexingReports()
```


Obtiene los informes sobre operaciones de indexación.


**Returns:**
com.groupdocs.search.common.IndexingReport[] - Los informes de indexación.

El ejemplo muestra cómo obtener los informes de indexación.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Creando índice en la carpeta especificada
index.add(documentsFolder); // Indexando documentos de la carpeta especificada
IndexingReport[] reports = index.getIndexingReports(); // Obteniendo los informes de indexación
 
```
 
````


### getSearchReports() {#getSearchReports--}
```
public final SearchReport[] getSearchReports()
```


Obtiene los informes sobre operaciones de búsqueda.


**Returns:**
com.groupdocs.search.common.SearchReport[] - Los informes de búsqueda.

El ejemplo muestra cómo obtener los informes de búsqueda.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query1 = "Einstein";
String query2 = "Newton";
Index index = new Index(indexFolder); // Creando índice en la carpeta especificada
index.add(documentsFolder); // Indexando documentos de la carpeta especificada
SearchResult result1 = index.search(query1); // Buscando
SearchResult result2 = index.search(query2);
SearchResult result3 = index.search(query1 + " & " + query2);
SearchReport[] reports = index.getSearchReports(); // Obteniendo los informes de búsqueda
 
```
 
````


### search(String query) {#search-java.lang.String-}
```
public final SearchResult search(String query)
```


Busca en el índice.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | query | java.lang.String | La consulta de búsqueda. |

El siguiente ejemplo muestra cómo realizar una búsqueda simple.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // Creando índice en la carpeta especificada
index.add(documentsFolder); // Indexando documentos de la carpeta especificada
SearchResult result = index.search(query); // Buscando
 
```
 
````

El siguiente ejemplo muestra cómo realizar una búsqueda Regex.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Creando índice en la carpeta especificada
index.add(documentsFolder); // Indexando documentos de la carpeta especificada
String query = "^[0-9]{3,}"; // El símbolo de intercalación al inicio de la consulta de búsqueda indica al índice que es una consulta Regex
SearchResult result = index.search(query); // Buscando
 
```
 
````

El siguiente ejemplo muestra cómo realizar una búsqueda facetada.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Creando índice en la carpeta especificada
index.add(documentsFolder); // Indexando documentos de la carpeta especificada
String query = "content:Newton"; // La palabra antes de los dos puntos en la consulta indica el nombre del campo del documento a buscar
SearchResult result = index.search(query); // Buscando
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(String query, SearchOptions options) {#search-java.lang.String-com.groupdocs.search.options.SearchOptions-}
```
public final SearchResult search(String query, SearchOptions options)
```


Busca en el índice.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | query | java.lang.String | La consulta de búsqueda. |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | Las opciones de búsqueda. |

El siguiente ejemplo muestra cómo realizar una búsqueda difusa.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Creando índice en la carpeta especificada
index.add(documentsFolder); // Indexando documentos de la carpeta especificada
SearchOptions options = new SearchOptions();
options.getFuzzySearch().setEnabled(true); // Habilitando la búsqueda difusa
options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(1)); // Estableciendo el número de diferencias posibles para cada palabra
// Las comillas dobles al principio y al final indican al índice que es una consulta de búsqueda de frase
String query = "\"The Pursuit of Happiness\"";
SearchResult result = index.search(query, options); // Buscando
 
```
 
````

El siguiente ejemplo muestra cómo realizar una búsqueda de sinónimos.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Creando índice en la carpeta especificada
index.add(documentsFolder); // Indexando documentos de la carpeta especificada
SearchOptions options = new SearchOptions();
options.setUseSynonymSearch(true); // Habilitando la búsqueda de sinónimos
String query = "cry";
SearchResult result = index.search(query, options); // Buscando
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(SearchQuery query) {#search-com.groupdocs.search.SearchQuery-}
```
public final SearchResult search(SearchQuery query)
```


Busca en el índice.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | La consulta de búsqueda. |

El siguiente ejemplo muestra cómo realizar una búsqueda usando la consulta en forma de objeto.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Creando índice en la carpeta especificada
index.add(documentsFolder); // Indexando documentos de la carpeta especificada
// Creando subconsulta 1
SearchQuery subquery1 = SearchQuery.createWordQuery("accommodation");
subquery1.setSearchOptions(new SearchOptions()); // Estableciendo opciones de búsqueda solo para la subconsulta 1
subquery1.getSearchOptions().getFuzzySearch().setEnabled(true); // Activando la búsqueda difusa
subquery1.getSearchOptions().getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(3)); // Estableciendo el número máximo de diferencias
// Creando subconsulta 2
SearchQuery subquery2 = SearchQuery.createNumericRangeQuery(1, 1000000);
// Creando subconsulta 3
SearchQuery subquery3 = SearchQuery.createRegexQuery("(.)\\1");
// Combinando subconsultas en una sola consulta
SearchQuery query = SearchQuery.createPhraseSearchQuery(subquery1, subquery2, subquery3);
SearchResult result = index.search(query); // Buscando
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(SearchQuery query, SearchOptions options) {#search-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-}
```
public final SearchResult search(SearchQuery query, SearchOptions options)
```


Busca en el índice.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | La consulta de búsqueda. |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | Las opciones de búsqueda. |

El siguiente ejemplo muestra cómo realizar una búsqueda usando la consulta en forma de objeto.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Creando índice en la carpeta especificada
index.add(documentsFolder); // Indexando documentos de la carpeta especificada
// Creando subconsulta de búsqueda por rango de fechas
SearchQuery subquery1 = SearchQuery.createDateRangeQuery(new Date(2011, 6, 17), new Date(2013, 1, 1));
// Creando subconsulta de comodín con número de palabras omitidas de 0 a 2
SearchQuery subquery2 = SearchQuery.createWildcardQuery(0, 2);
// Creando subconsulta de palabra simple
SearchQuery subquery3 = SearchQuery.createWordQuery("birth");
subquery3.setSearchOptions(new SearchOptions()); // Configurando opciones de búsqueda solo para la subconsulta 3
subquery3.getSearchOptions().getFuzzySearch().setEnabled(true);
subquery3.getSearchOptions().getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(1));
// Combinando subconsultas en una sola consulta
SearchQuery query = SearchQuery.createPhraseSearchQuery(subquery1, subquery2, subquery3);
// Creando objeto de opciones de búsqueda con mayor capacidad de ocurrencias encontradas
SearchOptions options = new SearchOptions(); // Opciones de búsqueda generales
options.setMaxOccurrenceCountPerTerm(1000000);
options.setMaxTotalOccurrenceCount(10000000);
SearchResult result = index.search(query, options); // Buscando
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(SearchImage image, ImageSearchOptions options) {#search-com.groupdocs.search.common.SearchImage-com.groupdocs.search.options.ImageSearchOptions-}
```
public final ImageSearchResult search(SearchImage image, ImageSearchOptions options)
```


Realiza una búsqueda inversa de imágenes en el índice.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | image | [SearchImage](../../com.groupdocs.search.common/searchimage) | La imagen a buscar. |
|
|  | options | [ImageSearchOptions](../../com.groupdocs.search.options/imagesearchoptions) | Las opciones de búsqueda de la imagen. |
|

**Returns:**
[ImageSearchResult](../../com.groupdocs.search.results/imagesearchresult) - The result of a reverse image search.

### searchNext(ChunkSearchToken chunkSearchToken) {#searchNext-com.groupdocs.search.common.ChunkSearchToken-}
```
public final SearchResult searchNext(ChunkSearchToken chunkSearchToken)
```


Continúa la búsqueda por fragmentos iniciada con el método Search.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | chunkSearchToken | [ChunkSearchToken](../../com.groupdocs.search.common/chunksearchtoken) | El token de búsqueda de fragmento. |

El ejemplo muestra cómo realizar una búsqueda de fragmento.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // Creando índice en la carpeta especificada
index.add(documentsFolder); // Indexando documentos de la carpeta especificada
SearchOptions options = new SearchOptions();
options.setChunkSearch(true); // Activando la búsqueda de fragmento
SearchResult result = index.search(query, options); // Iniciando la búsqueda de fragmento
System.out.println("Recuento de documentos: " + result.getDocumentCount());
System.out.println("Recuento de ocurrencias: " + result.getOccurrenceCount());
while (result.getNextChunkSearchToken() != null) {
result = index.searchNext(result.getNextChunkSearchToken()); // Continuando la búsqueda de fragmento
System.out.println("Recuento de documentos: " + result.getDocumentCount());
System.out.println("Recuento de ocurrencias: " + result.getOccurrenceCount());
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


Continúa la búsqueda por fragmentos iniciada con el método Search.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | chunkSearchToken | [ChunkSearchToken](../../com.groupdocs.search.common/chunksearchtoken) | El token de búsqueda de fragmento. |
|
|  | cancellation | [Cancellation](../../com.groupdocs.search.common/cancellation) | El objeto de cancelación. |

El ejemplo muestra cómo realizar una búsqueda usando la consulta en forma de objeto.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // Creando índice en la carpeta especificada
index.add(documentsFolder); // Indexando documentos de la carpeta especificada
Cancellation cancellation = new Cancellation(); // Este objeto de cancelación aborta todas las continuaciones de búsqueda si se cancela
SearchOptions options = new SearchOptions();
options.setChunkSearch(true); // Activando la búsqueda de fragmento
options.setCancellation(cancellation);
SearchResult result = index.search(query, options); // Iniciando la búsqueda de fragmento
System.out.println("Recuento de documentos: " + result.getDocumentCount());
System.out.println("Recuento de ocurrencias: " + result.getOccurrenceCount());
while (result.getNextChunkSearchToken() != null) {
result = index.searchNext(result.getNextChunkSearchToken(), cancellation); // Continuando la búsqueda de fragmento
System.out.println("Recuento de documentos: " + result.getDocumentCount());
System.out.println("Recuento de ocurrencias: " + result.getOccurrenceCount());
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


Minimiza el número de segmentos del índice fusionándolos uno con otro.
Esta operación mejora el rendimiento de la búsqueda.

El ejemplo muestra cómo combinar segmentos de un índice.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder1 = "c:\\MyDocuments1\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
String documentsFolder3 = "c:\\MyDocuments3\\";
Index index = new Index(indexFolder); // Creando índice en la carpeta especificada
index.add(documentsFolder1); // Indexando documentos desde la carpeta especificada
index.add(documentsFolder2); // Cada llamada a AddToIndex crea al menos un nuevo segmento en el índice
index.add(documentsFolder3);
// Fusionando segmentos del índice
index.optimize();
 
```
 
````



### optimize(MergeOptions options) {#optimize-com.groupdocs.search.options.MergeOptions-}
```
public final void optimize(MergeOptions options)
```


Minimiza el número de segmentos del índice fusionándolos uno con otro.
Esta operación mejora el rendimiento de la búsqueda.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | options | [MergeOptions](../../com.groupdocs.search.options/mergeoptions) | Las opciones de fusión. |

El ejemplo muestra cómo fusionar segmentos de un índice con opciones de fusión particulares.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder1 = "c:\\MyDocuments1\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
String documentsFolder3 = "c:\\MyDocuments3\\";
Index index = new Index(indexFolder); // Creando índice en la carpeta especificada
index.add(documentsFolder1); // Indexando documentos desde la carpeta especificada
index.add(documentsFolder2); // Cada llamada a AddToIndex crea al menos un nuevo segmento en el índice
index.add(documentsFolder3);
MergeOptions options = new MergeOptions();
options.setAsync(true); // Operación asíncrona
options.setCancellation(new Cancellation()); // Creando objeto de cancelación
// Fusionando segmentos del índice
index.optimize(options); // Este método devolverá antes de que la operación se complete
options.getCancellation().cancelAfter(10000); // Estableciendo la duración máxima de la operación a 10 segundos
 
```
 
````

|

### merge(Index index, MergeOptions options) {#merge-com.groupdocs.search.Index-com.groupdocs.search.options.MergeOptions-}
```
public final void merge(Index index, MergeOptions options)
```


Fusiona el índice especificado en el índice actual.
Nota que el otro índice no será modificado.


Si el otro índice tiene una versión anterior, debe actualizarse antes de fusionarse con
IndexUpdater
.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | index | [Index](../../com.groupdocs.search/index) | El índice en el que fusionar. |
|
|  | options | [MergeOptions](../../com.groupdocs.search.options/mergeoptions) | Las opciones de fusión. |

El ejemplo muestra cómo fusionar un índice en el índice actual.

````
 ```

String indexFolder1 = "c:\\MyIndex1\\";
String indexFolder2 = "c:\\MyIndex2\\";
String documentsFolder1 = "c:\\MyDocuments1\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
Index index1 = new Index(indexFolder1); // Creando index1
index1.add(documentsFolder1); // Indexando documentos
Index index2 = new Index(indexFolder2); // Creando index2
index2.add(documentsFolder2); // Indexando documentos
MergeOptions options = new MergeOptions();
options.setCancellation(new Cancellation()); // Creando objeto de cancelación
// Fusionando index2 en index1. Nota que los archivos de index2 no serán modificados.
index1.merge(index2, options);
 
```
 
````

|

### merge(IndexRepository repository, MergeOptions options) {#merge-com.groupdocs.search.IndexRepository-com.groupdocs.search.options.MergeOptions-}
```
public final void merge(IndexRepository repository, MergeOptions options)
```


Fusiona índices del repositorio de índices especificado en el índice actual.
Tenga en cuenta que los índices en el repositorio no se cambiarán.


Si otros índices tienen una versión anterior, deben actualizarse antes de fusionarse con
IndexUpdater
.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | repository | [IndexRepository](../../com.groupdocs.search/indexrepository) | El repositorio de índices en el que fusionar. |
|
|  | options | [MergeOptions](../../com.groupdocs.search.options/mergeoptions) | Las opciones de fusión. |

El ejemplo muestra cómo fusionar un repositorio de índices en el índice actual.

````
 ```

String indexFolder1 = "c:\\MyIndex1\\";
String indexFolder2 = "c:\\MyIndex2\\";
String indexFolder3 = "c:\\MyIndex3\\";
String documentsFolder1 = "c:\\MyDocuments1\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
String documentsFolder3 = "c:\\MyDocuments3\\";
Index index1 = new Index(indexFolder1); // Creando index1
index1.add(documentsFolder1); // Indexando documentos
IndexRepository repository = new IndexRepository(); // Creando repositorio de índices
Index index2 = repository.create(indexFolder2); // Creando index2
index2.add(documentsFolder2); // Indexando documentos
Index index3 = repository.create(indexFolder3); // Creando index3
index3.add(documentsFolder3); // Indexando documentos
MergeOptions options = new MergeOptions();
options.setCancellation(new Cancellation()); // Creando objeto de cancelación
// Fusionando todos los índices en el repositorio de índices en index1. Tenga en cuenta que index2 y index3 no se cambiarán.
index1.merge(repository, options);
 
```
 
````

|

### highlight(FoundDocument document, Highlighter highlighter) {#highlight-com.groupdocs.search.results.FoundDocument-com.groupdocs.search.highlighters.Highlighter-}
```
public final void highlight(FoundDocument document, Highlighter highlighter)
```


Genera texto con formato HTML con los términos encontrados resaltados.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | document | [FoundDocument](../../com.groupdocs.search.results/founddocument) | El documento encontrado. |
|
|  | highlighter | [Highlighter](../../com.groupdocs.search.highlighters/highlighter) | El resaltador de resultados de búsqueda. |

El ejemplo muestra cómo resaltar ocurrencias en texto con formato HTML.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentFolder = "c:\\MyDocuments\\";
// Creando un índice
Index index = new Index(indexFolder);
// Indexando documentos de la carpeta especificada
index.add(documentFolder);
// Buscar la palabra 'eternity'
SearchResult result = index.search("eternity");
// Resaltando ocurrencias en el texto
if (result.getDocumentCount() > 0) {
FoundDocument document = result.getFoundDocument(0); // Obteniendo el primer documento encontrado
OutputAdapter outputAdapter = new FileOutputAdapter("c:\\Highlighted.html"); // Creando un adaptador de salida al archivo
Highlighter highlighter = new HtmlHighlighter(outputAdapter); // Creando el objeto resaltador
index.highlight(document, highlighter); // Generando texto con formato HTML con ocurrencias resaltadas
}
 
```
 
````

|

### highlight(FoundDocument document, Highlighter highlighter, HighlightOptions options) {#highlight-com.groupdocs.search.results.FoundDocument-com.groupdocs.search.highlighters.Highlighter-com.groupdocs.search.options.HighlightOptions-}
```
public final void highlight(FoundDocument document, Highlighter highlighter, HighlightOptions options)
```


Genera texto con formato HTML con los términos encontrados resaltados.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | document | [FoundDocument](../../com.groupdocs.search.results/founddocument) | El documento encontrado. |
|
|  | highlighter | [Highlighter](../../com.groupdocs.search.highlighters/highlighter) | El resaltador de resultados de búsqueda. |
|
|  | options | [HighlightOptions](../../com.groupdocs.search.options/highlightoptions) | Las opciones de resaltado. |

El ejemplo muestra cómo resaltar ocurrencias en texto con formato HTML.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentFolder = "c:\\MyDocuments\\";
// Creando un índice
Index index = new Index(indexFolder);
// Indexando documentos de la carpeta especificada
index.add(documentFolder);
// Buscar la palabra 'eternity'
SearchResult result = index.search("eternity");
// Resaltando ocurrencias en el texto
if (result.getDocumentCount() > 0) {
FoundDocument document = result.getFoundDocument(0); // Obteniendo el primer documento encontrado
OutputAdapter outputAdapter = new FileOutputAdapter("c:\\Highlighted.html"); // Creando un adaptador de salida al archivo
Highlighter highlighter = new HtmlHighlighter(outputAdapter); // Creando el objeto resaltador
HighlightOptions options = new HighlightOptions(); // Creando el objeto de opciones de resaltado
options.setTermsBefore(5);
options.setTermsAfter(5);
options.setTermsTotal(15);
index.highlight(document, highlighter, options); // Generando texto con formato HTML con ocurrencias resaltadas
}
 
```
 
````

|

### getIndexedDocuments() {#getIndexedDocuments--}
```
public final DocumentInfo[] getIndexedDocuments()
```


Obtiene una matriz de todos los documentos indexados.


**Returns:**
com.groupdocs.search.results.DocumentInfo[] - Una matriz de todos los documentos indexados.

El ejemplo muestra cómo obtener una lista de documentos indexados desde un índice.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Creando un índice en la carpeta especificada
Index index = new Index(indexFolder);
// Indexando documentos de la carpeta especificada
index.add(documentsFolder);
// Obteniendo la lista de documentos indexados
DocumentInfo[] documents = index.getIndexedDocuments();
 
```
 
````


### getIndexedDocumentItems(DocumentInfo documentInfo) {#getIndexedDocumentItems-com.groupdocs.search.results.DocumentInfo-}
```
public final DocumentInfo[] getIndexedDocumentItems(DocumentInfo documentInfo)
```


Obtiene una matriz de elementos de documento.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | documentInfo | [DocumentInfo](../../com.groupdocs.search.results/documentinfo) | Una información de documento. |

El ejemplo muestra cómo obtener una lista de elementos de un documento indexado desde un índice.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Creando un índice en la carpeta especificada
Index index = new Index(indexFolder);
// Indexando documentos de la carpeta especificada
index.add(documentsFolder);
// Obteniendo la lista de documentos indexados
DocumentInfo[] documents = index.getIndexedDocuments();
for (int i = 0; i < documents.length; i++) {
DocumentInfo document = documents[i];
System.out.println(document.getFilePath());
DocumentInfo[] items = index.getIndexedDocumentItems(document); // Obteniendo la lista de elementos del documento
for (int j = 0; j < items.length; j++) {
DocumentInfo item = items[j];
System.out.println("\t" + item.getInnerPath());
}
}
 
```
 
````

|

**Returns:**
com.groupdocs.search.results.DocumentInfo[] - Una matriz de elementos de un documento.

### GetIndexedDocument(String documentKey) {#GetIndexedDocument-java.lang.String-}
```
public DocumentInfo GetIndexedDocument(String documentKey)
```


Obtiene un documento indexado por clave de documento.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | documentKey | java.lang.String | La clave del documento. |
|

**Returns:**
[DocumentInfo](../../com.groupdocs.search.results/documentinfo) - The indexed document.

### getDocumentText(DocumentInfo documentInfo, OutputAdapter adapter) {#getDocumentText-com.groupdocs.search.results.DocumentInfo-com.groupdocs.search.common.OutputAdapter-}
```
public final void getDocumentText(DocumentInfo documentInfo, OutputAdapter adapter)
```


Genera el texto de un documento indexado y lo pasa a través de un adaptador de salida.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | documentInfo | [DocumentInfo](../../com.groupdocs.search.results/documentinfo) | La información del documento indexado. |
|
|  | adapter | [OutputAdapter](../../com.groupdocs.search.common/outputadapter) | El adaptador de salida. |

El ejemplo muestra cómo obtener el texto de un documento indexado desde un índice.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Creando un índice en la carpeta especificada
Index index = new Index(indexFolder);
// Indexando documentos de la carpeta especificada
index.add(documentsFolder);
// Obteniendo la lista de documentos indexados
DocumentInfo[] documents = index.getIndexedDocuments();
// Obtención del texto de un documento
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


Genera texto con formato HTML para el documento indexado y lo transfiere a través del adaptador de salida.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | documentInfo | [DocumentInfo](../../com.groupdocs.search.results/documentinfo) | La información del documento indexado. |
|
|  | adapter | [OutputAdapter](../../com.groupdocs.search.common/outputadapter) | El adaptador de salida. |
|
|  | options | [TextOptions](../../com.groupdocs.search.options/textoptions) | Las opciones de recuperación de texto. |
|

### getIndexedPaths() {#getIndexedPaths--}
```
public final String[] getIndexedPaths()
```


Obtiene una matriz de rutas indexadas: documentos o carpetas.


**Returns:**
java.lang.String[] - Una matriz de rutas indexadas.

### delete(String[] paths, UpdateOptions options) {#delete-java.lang.String---com.groupdocs.search.options.UpdateOptions-}
```
public final DeleteResult delete(String[] paths, UpdateOptions options)
```


Elimina archivos o carpetas indexados del índice. Luego actualiza el índice sin las rutas eliminadas.
Tenga en cuenta que un documento individual no puede eliminarse del índice si se añadió al índice como parte de una carpeta.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | paths | java.lang.String[] | Las rutas a los archivos o carpetas a eliminar. |
|
|  | options | [UpdateOptions](../../com.groupdocs.search.options/updateoptions) | Las opciones de actualización. |

El ejemplo muestra cómo eliminar rutas indexadas de un índice.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder1 = "c:\\MyDocuments\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
// Creando un índice en la carpeta especificada
Index index = new Index(indexFolder);
// Indexando documentos de las carpetas especificadas
index.add(documentsFolder1);
index.add(documentsFolder2);
// Obtención de rutas indexadas del índice
String[] indexedPaths1 = index.getIndexedPaths();
// Escribiendo rutas indexadas en la consola
System.out.println("Rutas indexadas:");
for (String path : indexedPaths1) {
System.out.println("\t" + path);
}
// Eliminando la ruta del índice
DeleteResult deleteResult = index.delete(new String[] { documentsFolder1 }, new UpdateOptions());
// Obtención de rutas indexadas después de la eliminación
String[] indexedPaths2 = index.getIndexedPaths();
System.out.println("\nRutas eliminadas: " + deleteResult.getSuccessCount());
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


Elimina documentos indexados desde flujos o estructuras. Luego actualiza el índice sin los documentos eliminados.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | options | [UpdateOptions](../../com.groupdocs.search.options/updateoptions) | Las opciones de actualización. |
|
|  | documentKeys | java.lang.String[] | Las claves de los documentos añadidos desde flujos o estructuras. |
|

**Returns:**
[DeleteResult](../../com.groupdocs.search.results/deleteresult) - An object describing the result of deleting documents from the index.

### notifyIndex(Notification notification) {#notifyIndex-com.groupdocs.search.Notification-}
```
public final boolean notifyIndex(Notification notification)
```


Pasa el objeto de notificación especificado al índice para realizar la notificación.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | notification | [Notification](../../com.groupdocs.search/notification) | El objeto de notificación. |
|

**Returns:**
boolean - Devuelve  true  si la notificación se realizó con éxito; de lo contrario  false .

### changeAttributes(AttributeChangeBatch batch) {#changeAttributes-com.groupdocs.search.common.AttributeChangeBatch-}
```
public final void changeAttributes(AttributeChangeBatch batch)
```


Aplica el lote especificado de cambios de atributos a documentos indexados sin reindexar durante la operación de actualización.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | batch | [AttributeChangeBatch](../../com.groupdocs.search.common/attributechangebatch) | El lote de cambios de atributos. |
|

### getAttributes(String path) {#getAttributes-java.lang.String-}
```
public final String[] getAttributes(String path)
```


Obtiene todos los atributos asociados con el documento indexado especificado.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | path | java.lang.String | La ruta del documento. |
|

**Returns:**
java.lang.String[] - Atributos asociados al documento.

### loadIntoMemoryCompletely(String indexFolder) {#loadIntoMemoryCompletely-java.lang.String-}
```
public static Index loadIntoMemoryCompletely(String indexFolder)
```


Carga todo el índice en la memoria.
Cualquier cambio en el índice no se guarda automáticamente en la carpeta original.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | indexFolder | java.lang.String | La ruta de la carpeta del índice. |
|

**Returns:**
[Index](../../com.groupdocs.search/index) - The loaded in-memory index.

### loadIntoMemoryCompletely(String indexFolder, IndexSettings settings) {#loadIntoMemoryCompletely-java.lang.String-com.groupdocs.search.IndexSettings-}
```
public static Index loadIntoMemoryCompletely(String indexFolder, IndexSettings settings)
```


Carga todo el índice en la memoria.
Cualquier cambio en el índice no se guarda automáticamente en la carpeta original.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | indexFolder | java.lang.String | La ruta de la carpeta del índice. |
|
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | El objeto de configuración del índice. |
|

**Returns:**
[Index](../../com.groupdocs.search/index) - The loaded in-memory index.

