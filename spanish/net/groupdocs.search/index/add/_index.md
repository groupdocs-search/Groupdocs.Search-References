---
title: Add
second_title: GroupDocs.Buscar referencia de API de .NET
description: Realiza la operación de indexación. Agrega un archivo o carpeta por una ruta absoluta o relativa. Se indexarán los documentos de todas las subcarpetas.
type: docs
weight: 70
url: /es/net/groupdocs.search/index/add/
---
## Add(string) {#add_2}

Realiza la operación de indexación. Agrega un archivo o carpeta por una ruta absoluta o relativa. Se indexarán los documentos de todas las subcarpetas.

```csharp
public void Add(string path)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| path | String | La ruta a un archivo o carpeta que se va a indexar. |

### Ejemplos

El ejemplo muestra cómo agregar documentos a un índice.

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // Creando índice en la carpeta especificada
index.Add(folderPath); // Indexación de documentos en la carpeta especificada
index.Add(filePath); // Indexando el documento especificado
```

### Ver también

* class [Index](../../index)
* espacio de nombres [GroupDocs.Search](../../index)
* asamblea [GroupDocs.Search](../../../)

---

## Add(string, IndexingOptions) {#add_3}

Realiza la operación de indexación. Agrega un archivo o carpeta por una ruta absoluta o relativa. Se indexarán los documentos de todas las subcarpetas.

```csharp
public void Add(string path, IndexingOptions options)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| path | String | La ruta a un archivo o carpeta que se va a indexar. |
| options | IndexingOptions | Las opciones de indexación. |

### Ejemplos

El ejemplo muestra cómo agregar documentos a un índice con opciones de indexación particulares.

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // Creando índice en la carpeta especificada

IndexingOptions options = new IndexingOptions();
options.Threads = 2; // Establecer el número de subprocesos de indexación
index.Add(folderPath, options); // Indexación de documentos en la carpeta especificada
index.Add(filePath, options); // Indexando el documento especificado
```

### Ver también

* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* espacio de nombres [GroupDocs.Search](../../index)
* asamblea [GroupDocs.Search](../../../)

---

## Add(string[]) {#add_4}

Realiza la operación de indexación. Agrega archivos o carpetas por una ruta absoluta o relativa. Se indexarán los documentos de todas las subcarpetas.

```csharp
public void Add(string[] paths)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| paths | String[] | Las rutas a los archivos o carpetas que se van a indexar. |

### Ejemplos

El ejemplo muestra cómo agregar documentos a un índice.

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // Creando índice en la carpeta especificada

string[] paths = new string[] { folderPath, filePath };
index.Add(paths); // Indexación de documentos en las rutas especificadas
```

### Ver también

* class [Index](../../index)
* espacio de nombres [GroupDocs.Search](../../index)
* asamblea [GroupDocs.Search](../../../)

---

## Add(string[], IndexingOptions) {#add_5}

Realiza la operación de indexación. Agrega archivos o carpetas por una ruta absoluta o relativa. Se indexarán los documentos de todas las subcarpetas.

```csharp
public void Add(string[] paths, IndexingOptions options)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| paths | String[] | Las rutas a los archivos o carpetas que se van a indexar. |
| options | IndexingOptions | Las opciones de indexación. |

### Ejemplos

El ejemplo muestra cómo agregar documentos a un índice con opciones de indexación particulares.

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // Creando índice en la carpeta especificada

IndexingOptions options = new IndexingOptions();
options.Threads = 2; // Establecer el número de subprocesos de indexación
string[] paths = new string[] { folderPath, filePath };
index.Add(paths, options); // Indexación de documentos en las rutas especificadas
```

### Ver también

* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* espacio de nombres [GroupDocs.Search](../../index)
* asamblea [GroupDocs.Search](../../../)

---

## Add(Document[], IndexingOptions) {#add}

Realiza la operación de indexación. Agrega documentos del sistema de archivos, flujo o estructura.

```csharp
public void Add(Document[] documents, IndexingOptions options)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| documents | Document[] | Los documentos del sistema de archivos, flujo o estructura. |
| options | IndexingOptions | Las opciones de indexación. |

### Ver también

* class [Document](../../../groupdocs.search.common/document)
* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* espacio de nombres [GroupDocs.Search](../../index)
* asamblea [GroupDocs.Search](../../../)

---

## Add(ExtractedData[], IndexingOptions) {#add_1}

Realiza la operación de indexación. Agrega los datos extraídos al índice.

```csharp
public void Add(ExtractedData[] data, IndexingOptions options)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| data | ExtractedData[] | Los datos extraídos. |
| options | IndexingOptions | Las opciones de indexación. |

### Ver también

* class [ExtractedData](../../../groupdocs.search.common/extracteddata)
* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* espacio de nombres [GroupDocs.Search](../../index)
* asamblea [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
