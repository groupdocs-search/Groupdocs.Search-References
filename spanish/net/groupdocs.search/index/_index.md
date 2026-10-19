---
title: "Index"
second_title: "Referencia de la API de GroupDocs.Search para .NET"
description: "Representa la clase principal para indexar documentos y buscar a través de ellos."
type: docs
weight: 700
url: /es/net/groupdocs.search/index/
---
## Index class

Representa la clase principal para indexar documentos y buscar a través de ellos.

```csharp
public class Index : IDisposable
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [Index](index#constructor)() | Inicializa una nueva instancia de la clase [`Index`](../index) en memoria. |
| [Index](index#constructor_1)(IndexSettings) | Inicializa una nueva instancia de la clase [`Index`](../index) en memoria con configuraciones de índice particulares. |
| [Index](index#constructor_2)(string) | Inicializa una nueva instancia de la clase [`Index`](../index). Crea un nuevo índice o abre uno existente en disco. |
| [Index](index#constructor_3)(string, bool) | Inicializa una nueva instancia de la clase [`Index`](../index). Carga un índice existente desde disco si *overwriteIfExists* es `false`; de lo contrario, crea un nuevo índice en disco. |
| [Index](index#constructor_4)(string, IndexSettings) | Inicializa una nueva instancia de la clase [`Index`](../index). Crea un nuevo índice con configuraciones particulares o abre un índice existente en el disco. |
| [Index](index#constructor_5)(string, IndexSettings, bool) | Inicializa una nueva instancia de la clase [`Index`](../index). Carga un índice existente del disco si *overwriteIfExists* es `false`; de lo contrario crea un nuevo índice en el disco con configuraciones de índice particulares. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Dictionaries](../../groupdocs.search/index/dictionaries) { get; } | Obtiene el repositorio de diccionario. |
| [Events](../../groupdocs.search/index/events) { get; } | Obtiene el hub de eventos para suscribirse a eventos. |
| [IndexInfo](../../groupdocs.search/index/indexinfo) { get; } | Obtiene la información básica del índice. |
| [IndexSettings](../../groupdocs.search/index/indexsettings) { get; } | Obtiene la configuración del índice. |
| [Repository](../../groupdocs.search/index/repository) { get; } | Obtiene el objeto del repositorio de índice si el índice está contenido en él. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| static [LoadIntoMemoryCompletely](../../groupdocs.search/index/loadintomemorycompletely#loadintomemorycompletely)(string) | Carga todo el índice en memoria. Cualquier cambio en el índice no se guarda automáticamente en la carpeta original. |
| static [LoadIntoMemoryCompletely](../../groupdocs.search/index/loadintomemorycompletely#loadintomemorycompletely_1)(string, IndexSettings) | Carga todo el índice en memoria. Cualquier cambio en el índice no se guarda automáticamente en la carpeta original. |
| [Add](../../groupdocs.search/index/add#add_2)(string) | Realiza una operación de indexación. Añade un archivo o carpeta mediante una ruta absoluta o relativa. Los documentos de todas las subcarpetas serán indexados. |
| [Add](../../groupdocs.search/index/add#add_4)(string[]) | Realiza una operación de indexación. Añade archivos o carpetas mediante una ruta absoluta o relativa. Los documentos de todas las subcarpetas serán indexados. |
| [Add](../../groupdocs.search/index/add#add)(Document[], IndexingOptions) | Realiza una operación de indexación. Añade documentos desde el sistema de archivos, flujo o estructura. |
| [Add](../../groupdocs.search/index/add#add_1)(ExtractedData[], IndexingOptions) | Realiza una operación de indexación. Añade los datos extraídos al índice. |
| [Add](../../groupdocs.search/index/add#add_3)(string, IndexingOptions) | Realiza una operación de indexación. Añade un archivo o carpeta mediante una ruta absoluta o relativa. Los documentos de todas las subcarpetas serán indexados. |
| [Add](../../groupdocs.search/index/add#add_5)(string[], IndexingOptions) | Realiza una operación de indexación. Añade archivos o carpetas mediante una ruta absoluta o relativa. Los documentos de todas las subcarpetas serán indexados. |
| [ChangeAttributes](../../groupdocs.search/index/changeattributes)(AttributeChangeBatch) | Aplica el lote especificado de cambios de atributos a los documentos indexados sin volver a indexar durante la operación de actualización. |
| [CheckSegments](../../groupdocs.search/index/checksegments)(bool) | Comprueba el índice en busca de archivos de segmento dañados en el disco. El método repara la funcionalidad del índice en presencia de segmentos dañados, si *fixIndexFunctionality* es true; de lo contrario no repara. |
| [Delete](../../groupdocs.search/index/delete#delete_1)(string[], UpdateOptions) | Elimina archivos o carpetas indexados del índice. Luego actualiza el índice sin las rutas eliminadas. Tenga en cuenta que un documento individual no puede eliminarse del índice si fue añadido al índice como parte de una carpeta. |
| [Delete](../../groupdocs.search/index/delete#delete)(UpdateOptions, string[]) | Elimina documentos indexados de flujos o estructuras. Luego actualiza el índice sin los documentos eliminados. |
| [Dispose](../../groupdocs.search/index/dispose)() | Libera todos los recursos utilizados por el [`Index`](../index). |
| [GetAttributes](../../groupdocs.search/index/getattributes)(string) | Obtiene todos los atributos asociados con el documento indexado especificado. |
| [GetDocumentText](../../groupdocs.search/index/getdocumenttext#getdocumenttext)(DocumentInfo, OutputAdapter) | Genera el texto de un documento indexado y lo pasa a través de un adaptador de salida. |
| [GetDocumentText](../../groupdocs.search/index/getdocumenttext#getdocumenttext_1)(DocumentInfo, OutputAdapter, TextOptions) | Genera texto con formato HTML para el documento indexado y lo transfiere a través del adaptador de salida. |
| [GetIndexedDocument](../../groupdocs.search/index/getindexeddocument)(string) | Obtiene un documento indexado por clave de documento. |
| [GetIndexedDocumentItems](../../groupdocs.search/index/getindexeddocumentitems)(DocumentInfo) | Obtiene una matriz de elementos anidados del documento especificado (para documentos contenedores como ZIP, OST, PST). |
| [GetIndexedDocuments](../../groupdocs.search/index/getindexeddocuments)() | Obtiene una matriz de todos los documentos indexados. |
| [GetIndexedPaths](../../groupdocs.search/index/getindexedpaths)() | Obtiene una matriz de rutas indexadas: documentos o carpetas. |
| [GetIndexingReports](../../groupdocs.search/index/getindexingreports)() | Obtiene los informes sobre operaciones de indexación. |
| [GetSearchReports](../../groupdocs.search/index/getsearchreports)() | Obtiene los informes sobre operaciones de búsqueda. |
| [Highlight](../../groupdocs.search/index/highlight#highlight)(FoundDocument, Highlighter) | Genera texto con formato HTML con los términos encontrados resaltados. |
| [Highlight](../../groupdocs.search/index/highlight#highlight_1)(FoundDocument, Highlighter, HighlightOptions) | Genera texto con formato HTML con los términos encontrados resaltados. |
| [Merge](../../groupdocs.search/index/merge#merge)(Index, MergeOptions) | Fusiona el índice especificado con el índice actual. Tenga en cuenta que el otro índice no se modificará. |
| [Merge](../../groupdocs.search/index/merge#merge_1)(IndexRepository, MergeOptions) | Fusiona índices del repositorio de índices especificado con el índice actual. Tenga en cuenta que los índices en el repositorio no se modificarán. |
| [Notify](../../groupdocs.search/index/notify)(Notification) | Pasa el objeto de notificación especificado al índice para realizar la notificación. |
| [Optimize](../../groupdocs.search/index/optimize#optimize)() | Minimiza el número de segmentos del índice fusionándolos uno con otro. Esta operación mejora el rendimiento de la búsqueda. |
| [Optimize](../../groupdocs.search/index/optimize#optimize_1)(MergeOptions) | Minimiza el número de segmentos del índice fusionándolos uno con otro. Esta operación mejora el rendimiento de la búsqueda. |
| [SaveTo](../../groupdocs.search/index/saveto)(string) | Guarda el índice en memoria en el disco. También guarda el índice regular en otra carpeta. No cambia la configuración de este índice. |
| [Search](../../groupdocs.search/index/search#search_1)(SearchQuery) | Busca en el índice. |
| [Search](../../groupdocs.search/index/search#search_3)(string) | Busca en el índice. |
| [Search](../../groupdocs.search/index/search#search)(SearchImage, ImageSearchOptions) | Realiza una búsqueda inversa de imágenes en el índice. |
| [Search](../../groupdocs.search/index/search#search_2)(SearchQuery, SearchOptions) | Busca en el índice. |
| [Search](../../groupdocs.search/index/search#search_4)(string, SearchOptions) | Busca en el índice. |
| [SearchNext](../../groupdocs.search/index/searchnext#searchnext)(ChunkSearchToken) | Continúa la búsqueda por fragmentos iniciada con el método Search. |
| [SearchNext](../../groupdocs.search/index/searchnext#searchnext_1)(ChunkSearchToken, Cancellation) | Continúa la búsqueda por fragmentos iniciada con el método Search. |
| [Update](../../groupdocs.search/index/update#update)() | Reindexa los documentos que se han cambiado o eliminado desde la última actualización. Añade los archivos nuevos que se han agregado a las carpetas indexadas. |
| [Update](../../groupdocs.search/index/update#update_1)(UpdateOptions) | Reindexa los documentos que se han cambiado o eliminado desde la última actualización. Añade los archivos nuevos que se han agregado a las carpetas indexadas. |

### Observaciones

**Learn more**

* [Creating an index](https://docs.groupdocs.com/display/searchnet/Creating+an+index)
* [Indexing](https://docs.groupdocs.com/display/searchnet/Indexing)
* [Searching](https://docs.groupdocs.com/display/searchnet/Searching)

### Ejemplos

El ejemplo muestra un uso típico de la clase.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

SearchResult result = index.Search(query); // Searching in index
```

### Ver también

* namespace [GroupDocs.Search](../../groupdocs.search)
* assembly [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.search.dll -->
