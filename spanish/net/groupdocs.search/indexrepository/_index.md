---
title: IndexRepository
second_title: GroupDocs.Buscar referencia de API de .NET
description: Representa un contenedor para combinar múltiples índices y realizar operaciones comunes en ellos.
type: docs
weight: 660
url: /es/net/groupdocs.search/indexrepository/
---
## IndexRepository class

Representa un contenedor para combinar múltiples índices y realizar operaciones comunes en ellos.

```csharp
public class IndexRepository : IDisposable
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [IndexRepository](indexrepository)() | Inicializa una nueva instancia del[`IndexRepository`](../indexrepository) clase. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Events](../../groupdocs.search/indexrepository/events) { get; } | Obtiene el centro de eventos para suscribirse a eventos. |
| [Indexes](../../groupdocs.search/indexrepository/indexes) { get; } | Obtiene los índices contenidos en este[`IndexRepository`](../indexrepository) . |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [AddToRepository](../../groupdocs.search/indexrepository/addtorepository#addtorepository)(Index) | Agrega un índice al repositorio de índices. |
| [AddToRepository](../../groupdocs.search/indexrepository/addtorepository#addtorepository_1)(string) | Abre y agrega un índice al repositorio de índices. |
| [Create](../../groupdocs.search/indexrepository/create#create)() | Crea un nuevo índice en memoria. |
| [Create](../../groupdocs.search/indexrepository/create#create_1)(IndexSettings) | Crea un nuevo índice en memoria. |
| [Create](../../groupdocs.search/indexrepository/create#create_2)(string) | Crea un nuevo índice en el disco. La carpeta del índice se limpiará antes de la creación del índice. |
| [Create](../../groupdocs.search/indexrepository/create#create_3)(string, IndexSettings) | Crea un nuevo índice en el disco. La carpeta del índice se limpiará antes de la creación del índice. |
| [Dispose](../../groupdocs.search/indexrepository/dispose)() | Libera todos los recursos utilizados por el[`IndexRepository`](../indexrepository) . |
| [Search](../../groupdocs.search/indexrepository/search#search)(SearchQuery) | Busca en todos los índices del repositorio. |
| [Search](../../groupdocs.search/indexrepository/search#search_2)(string) | Busca en todos los índices del repositorio. |
| [Search](../../groupdocs.search/indexrepository/search#search_1)(SearchQuery, SearchOptions) | Busca en todos los índices del repositorio. |
| [Search](../../groupdocs.search/indexrepository/search#search_3)(string, SearchOptions) | Busca en todos los índices del repositorio. |
| [Update](../../groupdocs.search/indexrepository/update#update)() | Actualiza todos los índices del repositorio. |
| [Update](../../groupdocs.search/indexrepository/update#update_1)(UpdateOptions) | Actualiza todos los índices del repositorio. |

### Observaciones

**Aprende más**

* [Repositorio de índice de búsqueda](https://docs.groupdocs.com/display/searchnet/Search+index+repository)

### Ejemplos

El ejemplo demuestra un uso típico de la clase.

```csharp
string indexFolder1 = @"c:\MyIndex\";
string indexFolder2 = @"c:\MyIndex\";
string query = "Einstein";

IndexRepository repository = new IndexRepository();
repository.AddToRepository(indexFolder1); // Cargando un índice existente
repository.AddToRepository(indexFolder2); // Cargando otro índice existente

SearchResult result = repository.Search(query); // Buscando en índices del repositorio
```

### Ver también

* espacio de nombres [GroupDocs.Search](../../groupdocs.search)
* asamblea [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->