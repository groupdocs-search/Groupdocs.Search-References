---
title: Optimize
second_title: GroupDocs.Buscar referencia de API de .NET
description: Minimiza el número de segmentos de índice fusionándolos uno con otro. Esta operación mejora el rendimiento de la búsqueda.
type: docs
weight: 210
url: /es/net/groupdocs.search/index/optimize/
---
## Optimize() {#optimize}

Minimiza el número de segmentos de índice fusionándolos uno con otro. Esta operación mejora el rendimiento de la búsqueda.

```csharp
public void Optimize()
```

### Ejemplos

El ejemplo muestra cómo fusionar segmentos de un índice.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder1 = @"c:\MyDocuments1\";
string documentsFolder2 = @"c:\MyDocuments2\";
string documentsFolder3 = @"c:\MyDocuments3\";

Index index = new Index(indexFolder); // Creando índice en la carpeta especificada

index.Add(documentsFolder1); // Indexación de documentos de la carpeta especificada
index.Add(documentsFolder2); // Cada llamada a Add crea al menos un nuevo segmento en el índice
index.Add(documentsFolder3);

// Fusionando segmentos del índice
index.Optimize();
```

### Ver también

* class [Index](../../index)
* espacio de nombres [GroupDocs.Search](../../index)
* asamblea [GroupDocs.Search](../../../)

---

## Optimize(MergeOptions) {#optimize_1}

Minimiza el número de segmentos de índice fusionándolos uno con otro. Esta operación mejora el rendimiento de la búsqueda.

```csharp
public void Optimize(MergeOptions options)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| options | MergeOptions | Las opciones de combinación. |

### Ejemplos

El ejemplo demuestra cómo fusionar segmentos de un índice con opciones de fusión particulares.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder1 = @"c:\MyDocuments1\";
string documentsFolder2 = @"c:\MyDocuments2\";
string documentsFolder3 = @"c:\MyDocuments3\";

Index index = new Index(indexFolder); // Creando índice en la carpeta especificada

index.Add(documentsFolder1); // Indexación de documentos de la carpeta especificada
index.Add(documentsFolder2); // Cada llamada a Add crea al menos un nuevo segmento en el índice
index.Add(documentsFolder3);

MergeOptions options = new MergeOptions();
options.IsAsync = true; // Operación asíncrona
options.Cancellation = new Cancellation(); // Creando objeto de cancelación

// Fusionando segmentos del índice
index.Optimize(options); // Este método regresará antes de que se complete la operación

options.Cancellation.CancelAfter(10000); // Estableciendo la duración máxima de la operación a 10 segundos
```

### Ver también

* class [MergeOptions](../../../groupdocs.search.options/mergeoptions)
* class [Index](../../index)
* espacio de nombres [GroupDocs.Search](../../index)
* asamblea [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
