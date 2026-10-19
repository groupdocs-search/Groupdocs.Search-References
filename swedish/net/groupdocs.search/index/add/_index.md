---
title: "Lägg till"
second_title: "GroupDocs.Search för .NET API-referens"
description: "Utför indexeringsoperation. Lägger till en fil eller mapp med en absolut eller relativ sökväg. Dokument från alla undermappar kommer att indexeras."
type: docs
weight: 80
url: /sv/net/groupdocs.search/index/add/
---
## Add(string) {#add_2}

Utför indexeringsoperation. Lägger till en fil eller mapp med en absolut eller relativ sökväg. Dokument från alla undermappar kommer att indexeras.

```csharp
public void Add(string path)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| path | String | Sökvägen till en fil eller mapp som ska indexeras. |

### Exempel

Exemplet visar hur man lägger till dokument i ett index.

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(folderPath); // Indexing documents in the specified folder
index.Add(filePath); // Indexing the specified document
```

### Se även

* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Add(string, IndexingOptions) {#add_3}

Utför indexeringsoperation. Lägger till en fil eller mapp med en absolut eller relativ sökväg. Dokument från alla undermappar kommer att indexeras.

```csharp
public void Add(string path, IndexingOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| path | String | Sökvägen till en fil eller mapp som ska indexeras. |
| options | IndexingOptions | Indexeringsalternativen. |

### Exempel

Exemplet visar hur man lägger till dokument i ett index med särskilda indexeringsalternativ.

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

### Se även

* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Add(string[]) {#add_4}

Utför indexeringsoperation. Lägger till filer eller mappar med en absolut eller relativ sökväg. Dokument från alla undermappar kommer att indexeras.

```csharp
public void Add(string[] paths)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| paths | String[] | Sökvägarna till filer eller mappar som ska indexeras. |

### Exempel

Exemplet visar hur man lägger till dokument i ett index.

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // Creating index in the specified folder

string[] paths = new string[] { folderPath, filePath };
index.Add(paths); // Indexing documents at the specified paths
```

### Se även

* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Add(string[], IndexingOptions) {#add_5}

Utför indexeringsoperation. Lägger till filer eller mappar med en absolut eller relativ sökväg. Dokument från alla undermappar kommer att indexeras.

```csharp
public void Add(string[] paths, IndexingOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| paths | String[] | Sökvägarna till filer eller mappar som ska indexeras. |
| options | IndexingOptions | Indexeringsalternativen. |

### Exempel

Exemplet visar hur man lägger till dokument i ett index med särskilda indexeringsalternativ.

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

### Se även

* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Add(Document[], IndexingOptions) {#add}

Utför indexeringsoperation. Lägger till dokument från filsystem, ström eller struktur.

```csharp
public void Add(Document[] documents, IndexingOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| dokument | Document[] | Dokumenten från filsystem, ström eller struktur. |
| options | IndexingOptions | Indexeringsalternativen. |

### Se även

* class [Document](../../../groupdocs.search.common/document)
* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Add(ExtractedData[], IndexingOptions) {#add_1}

Utför indexeringsoperation. Lägger till den extraherade datan i indexet.

```csharp
public void Add(ExtractedData[] data, IndexingOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| data | ExtractedData[] | Den extraherade datan. |
| options | IndexingOptions | Indexeringsalternativen. |

### Se även

* class [ExtractedData](../../../groupdocs.search.common/extracteddata)
* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.search.dll -->
