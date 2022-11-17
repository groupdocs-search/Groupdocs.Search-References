---
title: Add
second_title: GroupDocs.Search efter .NET API Reference
description: Utför indexeringsoperation. Lägger till en fil eller mapp med en absolut eller relativ sökväg. Dokument från alla undermappar kommer att indexeras.
type: docs
weight: 70
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

Index index = new Index(indexFolder); // Skapar index i den angivna mappen
index.Add(folderPath); // Indexering av dokument i den angivna mappen
index.Add(filePath); // Indexering av det angivna dokumentet
```

### Se även

* class [Index](../../index)
* namnutrymme [GroupDocs.Search](../../index)
* hopsättning [GroupDocs.Search](../../../)

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

Exemplet visar hur man lägger till dokument till ett index med särskilda indexeringsalternativ.

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // Skapar index i den angivna mappen

IndexingOptions options = new IndexingOptions();
options.Threads = 2; // Ställa in antalet indexeringstrådar
index.Add(folderPath, options); // Indexering av dokument i den angivna mappen
index.Add(filePath, options); // Indexering av det angivna dokumentet
```

### Se även

* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* namnutrymme [GroupDocs.Search](../../index)
* hopsättning [GroupDocs.Search](../../../)

---

## Add(string[]) {#add_4}

Utför indexeringsoperation. Lägger till filer eller mappar med en absolut eller relativ sökväg. Dokument från alla undermappar kommer att indexeras.

```csharp
public void Add(string[] paths)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| paths | String[] | Sökvägarna till en fil eller mapp som ska indexeras. |

### Exempel

Exemplet visar hur man lägger till dokument i ett index.

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // Skapar index i den angivna mappen

string[] paths = new string[] { folderPath, filePath };
index.Add(paths); // Indexering av dokument på de angivna sökvägarna
```

### Se även

* class [Index](../../index)
* namnutrymme [GroupDocs.Search](../../index)
* hopsättning [GroupDocs.Search](../../../)

---

## Add(string[], IndexingOptions) {#add_5}

Utför indexeringsoperation. Lägger till filer eller mappar med en absolut eller relativ sökväg. Dokument från alla undermappar kommer att indexeras.

```csharp
public void Add(string[] paths, IndexingOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| paths | String[] | Sökvägarna till en fil eller mapp som ska indexeras. |
| options | IndexingOptions | Indexeringsalternativen. |

### Exempel

Exemplet visar hur man lägger till dokument till ett index med särskilda indexeringsalternativ.

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // Skapar index i den angivna mappen

IndexingOptions options = new IndexingOptions();
options.Threads = 2; // Ställa in antalet indexeringstrådar
string[] paths = new string[] { folderPath, filePath };
index.Add(paths, options); // Indexering av dokument på de angivna sökvägarna
```

### Se även

* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* namnutrymme [GroupDocs.Search](../../index)
* hopsättning [GroupDocs.Search](../../../)

---

## Add(Document[], IndexingOptions) {#add}

Utför indexeringsoperation. Lägger till dokument från filsystem, ström eller struktur.

```csharp
public void Add(Document[] documents, IndexingOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| documents | Document[] | Dokumenten från filsystem, ström eller struktur. |
| options | IndexingOptions | Indexeringsalternativen. |

### Se även

* class [Document](../../../groupdocs.search.common/document)
* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* namnutrymme [GroupDocs.Search](../../index)
* hopsättning [GroupDocs.Search](../../../)

---

## Add(ExtractedData[], IndexingOptions) {#add_1}

Utför indexeringsoperation. Lägger till extraherade data till indexet.

```csharp
public void Add(ExtractedData[] data, IndexingOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| data | ExtractedData[] | De extraherade uppgifterna. |
| options | IndexingOptions | Indexeringsalternativen. |

### Se även

* class [ExtractedData](../../../groupdocs.search.common/extracteddata)
* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* namnutrymme [GroupDocs.Search](../../index)
* hopsättning [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
