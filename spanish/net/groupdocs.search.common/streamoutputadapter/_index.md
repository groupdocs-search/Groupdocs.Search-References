---
title: StreamOutputAdapter
second_title: GroupDocs.Buscar referencia de API de .NET
description: Representa un adaptador de salida que recopila la salida en unStream .
type: docs
weight: 300
url: /es/net/groupdocs.search.common/streamoutputadapter/
---
## StreamOutputAdapter class

Representa un adaptador de salida que recopila la salida en unStream .

```csharp
public class StreamOutputAdapter : OutputAdapter
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [StreamOutputAdapter](streamoutputadapter#constructor)(OutputFormat, Stream) | Inicializa una nueva instancia del[`StreamOutputAdapter`](../streamoutputadapter) clase. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [OutputFormat](../../groupdocs.search.common/resultbuilderfactory/outputformat) { get; } | Obtiene el formato de salida. |
| [Stream](../../groupdocs.search.common/streamoutputadapter/stream) { get; } | Obtiene un flujo de salida. |

### Observaciones

**Aprende más**

* [Adaptadores de salida](https://docs.groupdocs.com/display/searchnet/Output+adapters)

### Ejemplos

El ejemplo demuestra un uso típico de la clase.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creando un índice en la carpeta especificada

index.Add(documentsFolder); // Indexación de documentos de la carpeta especificada

DocumentInfo[] documents = index.GetIndexedDocuments(); // Obtener información sobre documentos indexados

using (Stream stream = new MemoryStream()) // Creando un flujo
{
    StreamOutputAdapter adapter = new StreamOutputAdapter(stream); // Creando un flujo output adapter
    index.GetDocumentText(documents[0], adapter); // Generando un documento de texto en la secuencia
}
```

### Ver también

* class [OutputAdapter](../outputadapter)
* espacio de nombres [GroupDocs.Search.Common](../../groupdocs.search.common)
* asamblea [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
