---
title: Index
second_title: GroupDocs.Buscar referencia de API de .NET
description: Representa la clase principal para indexar documentos y buscar en ellos.
type: docs
weight: 680
url: /es/net/groupdocs.search/index/
---
## Index class

Representa la clase principal para indexar documentos y buscar en ellos.

```csharp
public class Index : IDisposable
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [Index](index#constructor)() | Inicializa una nueva instancia del[`Index`](../index) clase en memoria. |
| [Index](index#constructor_1)(IndexSettings) | Inicializa una nueva instancia del[`Index`](../index) clase en memoria con configuración de índice particular. |
| [Index](index#constructor_2)(string) | Inicializa una nueva instancia del[`Index`](../index) class. Crea un índice nuevo o abre uno existente en el disco. |
| [Index](index#constructor_3)(string, bool) | Inicializa una nueva instancia del[`Index`](../index) class. Carga un índice existente desde el disco si*overwriteIfExists* es`FALSO`; crea un nuevo índice en el disco de lo contrario. |
| [Index](index#constructor_4)(string, IndexSettings) | Inicializa una nueva instancia del[`Index`](../index) class. Crea un nuevo índice con una configuración particular o abre un índice existente en el disco. |
| [Index](index#constructor_5)(string, IndexSettings, bool) | Inicializa una nueva instancia del[`Index`](../index) class. Carga un índice existente desde el disco si*overwriteIfExists* es`FALSO` ; crea un nuevo índice en el disco con una configuración de índice particular de lo contrario. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Dictionaries](../../groupdocs.search/index/dictionaries) { get; } | Obtiene el repositorio de diccionarios. |
| [Events](../../groupdocs.search/index/events) { get; } | Obtiene el centro de eventos para suscribirse a eventos. |
| [IndexInfo](../../groupdocs.search/index/indexinfo) { get; } | Obtiene la información básica sobre el índice. |
| [IndexSettings](../../groupdocs.search/index/indexsettings) { get; } | Obtiene la configuración del índice. |
| [Repository](../../groupdocs.search/index/repository) { get; } | Obtiene el objeto del repositorio de índices si el índice está contenido en él. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Add](../../groupdocs.search/index/add#add_2)(string) | Realiza la operación de indexación. Agrega un archivo o carpeta por una ruta absoluta o relativa. Se indexarán los documentos de todas las subcarpetas. |
| [Add](../../groupdocs.search/index/add#add_4)(string[]) | Realiza la operación de indexación. Agrega archivos o carpetas por una ruta absoluta o relativa. Se indexarán los documentos de todas las subcarpetas. |
| [Add](../../groupdocs.search/index/add#add)(Document[], IndexingOptions) | Realiza la operación de indexación. Agrega documentos del sistema de archivos, flujo o estructura. |
| [Add](../../groupdocs.search/index/add#add_1)(ExtractedData[], IndexingOptions) | Realiza la operación de indexación. Agrega los datos extraídos al índice. |
| [Add](../../groupdocs.search/index/add#add_3)(string, IndexingOptions) | Realiza la operación de indexación. Agrega un archivo o carpeta por una ruta absoluta o relativa. Se indexarán los documentos de todas las subcarpetas. |
| [Add](../../groupdocs.search/index/add#add_5)(string[], IndexingOptions) | Realiza la operación de indexación. Agrega archivos o carpetas por una ruta absoluta o relativa. Se indexarán los documentos de todas las subcarpetas. |
| [ChangeAttributes](../../groupdocs.search/index/changeattributes)(AttributeChangeBatch) | Aplica el lote especificado de cambios de atributos a los documentos indexados sin volver a indexarlos durante la operación de actualización. |
| [Delete](../../groupdocs.search/index/delete#delete_1)(string[], UpdateOptions) | Elimina archivos o carpetas indexados del índice. Luego actualiza el índice sin rutas eliminadas. Tenga en cuenta que un documento individual no se puede eliminar del índice si se agregó al índice como parte de una carpeta. |
| [Delete](../../groupdocs.search/index/delete#delete)(UpdateOptions, string[]) | Elimina documentos indexados de flujos o estructuras. Luego actualiza el índice sin documentos eliminados. |
| [Dispose](../../groupdocs.search/index/dispose)() | Libera todos los recursos utilizados por el[`Index`](../index) . |
| [GetAttributes](../../groupdocs.search/index/getattributes)(string) | Obtiene todos los atributos asociados con el documento indexado especificado. |
| [GetDocumentText](../../groupdocs.search/index/getdocumenttext#getdocumenttext)(DocumentInfo, OutputAdapter) | Genera texto con formato HTML para el documento indexado y lo transfiere a través del adaptador de salida. |
| [GetDocumentText](../../groupdocs.search/index/getdocumenttext#getdocumenttext_1)(DocumentInfo, OutputAdapter, TextOptions) | Genera texto con formato HTML para el documento indexado y lo transfiere a través del adaptador de salida. |
| [GetIndexedDocumentItems](../../groupdocs.search/index/getindexeddocumentitems)(DocumentInfo) | Obtiene una matriz de elementos anidados del documento especificado (para documentos contenedores como ZIP, OST, PST). |
| [GetIndexedDocuments](../../groupdocs.search/index/getindexeddocuments)() | Obtiene una matriz de todos los documentos indexados. |
| [GetIndexedPaths](../../groupdocs.search/index/getindexedpaths)() | Obtiene una matriz de rutas indexadas: documentos o carpetas. |
| [GetIndexingReports](../../groupdocs.search/index/getindexingreports)() | Obtiene los informes sobre las operaciones de indexación. |
| [GetSearchReports](../../groupdocs.search/index/getsearchreports)() | Obtiene los informes sobre las operaciones de búsqueda. |
| [Highlight](../../groupdocs.search/index/highlight#highlight)(FoundDocument, Highlighter) | Genera texto en formato HTML con los términos encontrados resaltados. |
| [Highlight](../../groupdocs.search/index/highlight#highlight_1)(FoundDocument, Highlighter, HighlightOptions) | Genera texto en formato HTML con los términos encontrados resaltados. |
| [Merge](../../groupdocs.search/index/merge#merge)(Index, MergeOptions) | Fusiona el índice especificado con el índice actual. Tenga en cuenta que el otro índice no cambiará. |
| [Merge](../../groupdocs.search/index/merge#merge_1)(IndexRepository, MergeOptions) | Fusiona índices del repositorio de índices especificado en el índice actual. Tenga en cuenta que los índices del repositorio no cambiarán. |
| [Notify](../../groupdocs.search/index/notify)(Notification) | Pasa el objeto de notificación especificado al índice para realizar la notificación. |
| [Optimize](../../groupdocs.search/index/optimize#optimize)() | Minimiza el número de segmentos de índice fusionándolos uno con otro. Esta operación mejora el rendimiento de la búsqueda. |
| [Optimize](../../groupdocs.search/index/optimize#optimize_1)(MergeOptions) | Minimiza el número de segmentos de índice fusionándolos uno con otro. Esta operación mejora el rendimiento de la búsqueda. |
| [Search](../../groupdocs.search/index/search#search_1)(SearchQuery) | Búsquedas en index. |
| [Search](../../groupdocs.search/index/search#search_3)(string) | Búsquedas en index. |
| [Search](../../groupdocs.search/index/search#search)(SearchImage, ImageSearchOptions) | Realiza una búsqueda inversa de imágenes en el índice. |
| [Search](../../groupdocs.search/index/search#search_2)(SearchQuery, SearchOptions) | Búsquedas en index. |
| [Search](../../groupdocs.search/index/search#search_4)(string, SearchOptions) | Búsquedas en index. |
| [SearchNext](../../groupdocs.search/index/searchnext#searchnext)(ChunkSearchToken) | Continúa la búsqueda de fragmentos iniciada con el método Buscar. |
| [SearchNext](../../groupdocs.search/index/searchnext#searchnext_1)(ChunkSearchToken, Cancellation) | Continúa la búsqueda de fragmentos iniciada con el método Buscar. |
| [Update](../../groupdocs.search/index/update#update)() | Vuelve a indexar documentos que se han modificado o eliminado desde la última actualización. Agrega nuevos archivos que se han agregado a las carpetas indexadas. |
| [Update](../../groupdocs.search/index/update#update_1)(UpdateOptions) | Vuelve a indexar documentos que se han modificado o eliminado desde la última actualización. Agrega nuevos archivos que se han agregado a las carpetas indexadas. |

### Observaciones

**Aprende más**

* [Crear un índice](https://docs.groupdocs.com/display/searchnet/Creating+an+index)
* [Indexación](https://docs.groupdocs.com/display/searchnet/Indexing)
* [buscando](https://docs.groupdocs.com/display/searchnet/Searching)

### Ejemplos

El ejemplo demuestra un uso típico de la clase.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

Index index = new Index(indexFolder); // Creando índice en la carpeta especificada
index.Add(documentsFolder); // Indexación de documentos de la carpeta especificada

SearchResult result = index.Search(query); // Buscando en el índice
```

### Ver también

* espacio de nombres [GroupDocs.Search](../../groupdocs.search)
* asamblea [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
