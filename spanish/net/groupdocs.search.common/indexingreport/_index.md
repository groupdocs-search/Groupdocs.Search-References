---
title: IndexingReport
second_title: GroupDocs.Buscar referencia de API de .NET
description: Representa información detallada sobre una operación de indexación.
type: docs
weight: 240
url: /es/net/groupdocs.search.common/indexingreport/
---
## IndexingReport class

Representa información detallada sobre una operación de indexación.

```csharp
public class IndexingReport
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [EndTime](../../groupdocs.search.common/indexingreport/endtime) { get; } | Obtiene la hora de finalización de la indexación. |
| [Errors](../../groupdocs.search.common/indexingreport/errors) { get; } | Obtiene la lista de errores. |
| [IndexedDocuments](../../groupdocs.search.common/indexingreport/indexeddocuments) { get; } | Obtiene la lista de documentos indexados. |
| [IndexedDocumentsSize](../../groupdocs.search.common/indexingreport/indexeddocumentssize) { get; } | Obtiene la longitud total de los documentos indexados en MB. |
| [IndexingTime](../../groupdocs.search.common/indexingreport/indexingtime) { get; } | Obtiene la duración de la indexación. |
| [RemovedDocuments](../../groupdocs.search.common/indexingreport/removeddocuments) { get; } | Obtiene la lista de documentos eliminados del índice. |
| [SegmentCount](../../groupdocs.search.common/indexingreport/segmentcount) { get; } | Obtiene el número de segmentos de índice. |
| [StartTime](../../groupdocs.search.common/indexingreport/starttime) { get; } | Obtiene la hora de inicio de la indexación. |
| [TotalDocumentsInIndex](../../groupdocs.search.common/indexingreport/totaldocumentsinindex) { get; } | Obtiene el número total de documentos en el índice. |
| [TotalIndexSize](../../groupdocs.search.common/indexingreport/totalindexsize) { get; } | Obtiene el tamaño total del índice en bytes. |
| [TotalTermCount](../../groupdocs.search.common/indexingreport/totaltermcount) { get; } | Obtiene el número total de términos en index. |
| [UpdatedDocuments](../../groupdocs.search.common/indexingreport/updateddocuments) { get; } | Obtiene la lista de documentos actualizados. |

### Observaciones

**Aprende más**

* [Informes de indexación](https://docs.groupdocs.com/display/searchnet/Indexing+reports)

### Ejemplos

El ejemplo demuestra un uso típico de la clase.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder1 = @"c:\MyDocuments1\";
string documentsFolder2 = @"c:\MyDocuments2\";

// Creando un índice en la carpeta especificada
Index index = new Index(indexFolder);

// Indexación de documentos
index.Add(documentsFolder1);
index.Add(documentsFolder2);

// Obtener informes de indexación
IndexingReport[] reports = index.GetIndexingReports();

// Imprimiendo reportes a la consola
foreach (IndexingReport report in reports)
{
    Console.WriteLine("Time: " + report.StartTime);
    Console.WriteLine("Duration: " + report.IndexingTime);
    Console.WriteLine("Documents total: " + report.TotalDocumentsInIndex);
    Console.WriteLine("Terms total: " + report.TotalTermCount);
    Console.WriteLine("Indexed documents size (MB): " + report.IndexedDocumentsSize);
    Console.WriteLine("Index size (MB): " + (report.TotalIndexSize / 1024.0 / 1024.0));
    Console.WriteLine();
}
```

### Ver también

* espacio de nombres [GroupDocs.Search.Common](../../groupdocs.search.common)
* asamblea [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
