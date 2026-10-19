---
title: "Add"
second_title: "Referencia de la API de GroupDocs.Search para .NET"
description: "Realiza una operación de indexación. Añade un archivo o carpeta mediante una ruta absoluta o relativa. Los documentos de todas las subcarpetas serán indexados."
type: docs
weight: 80
url: /es/net/groupdocs.search/index/add/
---
## Add(string) {#add_2}

Realiza una operación de indexación. Añade un archivo o carpeta mediante una ruta absoluta o relativa. Los documentos de todas las subcarpetas serán indexados.

```csharp
public void Add(string path)
```

| Parameter | Type | Descripción |
| --- | --- | --- |
| ruta | String | La ruta a un archivo o carpeta que se indexará. |

### Ejemplos

El ejemplo muestra cómo agregar documentos a un índice.

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(folderPath); // Indexing documents in the specified folder
index.Add(filePath); // Indexing the specified document
```

### Ver también

* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Add(string, IndexingOptions) {#add_3}

Realiza una operación de indexación. Añade un archivo o carpeta mediante una ruta absoluta o relativa. Los documentos de todas las subcarpetas serán indexados.

```csharp
public void Add(string path, IndexingOptions options)
```

| Parameter | Type | Descripción |
| --- | --- | --- |
| ruta | String | La ruta a un archivo o carpeta que se indexará. |
| opciones | IndexingOptions | Las opciones de indexación. |

### Ejemplos

El ejemplo muestra cómo agregar documentos a un índice con opciones de indexación particulares.

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // Creating index in the specified folder

IndexingOptions options = new IndexingOptions();
options.Threads = 2; // Setting the number of indexing threads
index.Add(folderPath, options); // Indexing documents in the specified folder
index.Add(filePath, options); // Indexing the specified document
```

### Ver también

* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Add(string[]) {#add_4}

Realiza una operación de indexación. Añade archivos o carpetas mediante una ruta absoluta o relativa. Los documentos de todas las subcarpetas serán indexados.

```csharp
public void Add(string[] paths)
```

| Parameter | Type | Descripción |
| --- | --- | --- |
| rutas | String[] | Las rutas a archivos o carpetas que se indexarán. |

### Ejemplos

El ejemplo muestra cómo agregar documentos a un índice.

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // Creating index in the specified folder

string[] paths = new string[] { folderPath, filePath };
index.Add(paths); // Indexing documents at the specified paths
```

### Ver también

* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Add(string[], IndexingOptions) {#add_5}

Realiza una operación de indexación. Añade archivos o carpetas mediante una ruta absoluta o relativa. Los documentos de todas las subcarpetas serán indexados.

```csharp
public void Add(string[] paths, IndexingOptions options)
```

| Parameter | Type | Descripción |
| --- | --- | --- |
| rutas | String[] | Las rutas a archivos o carpetas que se indexarán. |
| opciones | IndexingOptions | Las opciones de indexación. |

### Ejemplos

El ejemplo muestra cómo agregar documentos a un índice con opciones de indexación particulares.

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // Creating index in the specified folder

IndexingOptions options = new IndexingOptions();
options.Threads = 2; // Setting the number of indexing threads
string[] paths = new string[] { folderPath, filePath };
index.Add(paths, options); // Indexing documents at the specified paths
```

### Ver también

* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Add(Document[], IndexingOptions) {#add}

Realiza una operación de indexación. Añade documentos desde el sistema de archivos, flujo o estructura.

```csharp
public void Add(Document[] documents, IndexingOptions options)
```

| Parameter | Type | Descripción |
| --- | --- | --- |
| documentos | Document[] | Los documentos del sistema de archivos, flujo o estructura. |
| opciones | IndexingOptions | Las opciones de indexación. |

### Ver también

* class [Document](../../../groupdocs.search.common/document)
* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Add(ExtractedData[], IndexingOptions) {#add_1}

Realiza una operación de indexación. Añade los datos extraídos al índice.

```csharp
public void Add(ExtractedData[] data, IndexingOptions options)
```

| Parameter | Type | Descripción |
| --- | --- | --- |
| datos | ExtractedData[] | Los datos extraídos. |
| opciones | IndexingOptions | Las opciones de indexación. |

### Ver también

* class [ExtractedData](../../../groupdocs.search.common/extracteddata)
* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.search.dll -->
