---
title: "Toevoegen"
second_title: "GroupDocs.Search voor .NET API-referentie"
description: "Voert een indexeerbewerking uit. Voegt een bestand of map toe via een absoluut of relatief pad. Documenten uit alle submappen worden geïndexeerd."
type: docs
weight: 80
url: /nl/net/groupdocs.search/index/add/
---
## Add(string) {#add_2}

Voert een indexeerbewerking uit. Voegt een bestand of map toe via een absoluut of relatief pad. Documenten uit alle submappen worden geïndexeerd.

```csharp
public void Add(string path)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| path | String | Het pad naar een bestand of map die geïndexeerd moet worden. |

### Voorbeelden

Het voorbeeld toont hoe documenten aan een index kunnen worden toegevoegd.

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(folderPath); // Indexing documents in the specified folder
index.Add(filePath); // Indexing the specified document
```

### Zie ook

* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Add(string, IndexingOptions) {#add_3}

Voert een indexeerbewerking uit. Voegt een bestand of map toe via een absoluut of relatief pad. Documenten uit alle submappen worden geïndexeerd.

```csharp
public void Add(string path, IndexingOptions options)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| path | String | Het pad naar een bestand of map die geïndexeerd moet worden. |
| opties | IndexingOptions | De indexeringsopties. |

### Voorbeelden

Het voorbeeld toont hoe documenten aan een index kunnen worden toegevoegd met specifieke indexeringsopties.

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

### Zie ook

* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Add(string[]) {#add_4}

Voert een indexeerbewerking uit. Voegt bestanden of mappen toe via een absoluut of relatief pad. Documenten uit alle submappen worden geïndexeerd.

```csharp
public void Add(string[] paths)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| paths | String[] | De paden naar bestanden of mappen die geïndexeerd moeten worden. |

### Voorbeelden

Het voorbeeld toont hoe documenten aan een index kunnen worden toegevoegd.

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // Creating index in the specified folder

string[] paths = new string[] { folderPath, filePath };
index.Add(paths); // Indexing documents at the specified paths
```

### Zie ook

* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Add(string[], IndexingOptions) {#add_5}

Voert een indexeerbewerking uit. Voegt bestanden of mappen toe via een absoluut of relatief pad. Documenten uit alle submappen worden geïndexeerd.

```csharp
public void Add(string[] paths, IndexingOptions options)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| paths | String[] | De paden naar bestanden of mappen die geïndexeerd moeten worden. |
| opties | IndexingOptions | De indexeringsopties. |

### Voorbeelden

Het voorbeeld toont hoe documenten aan een index kunnen worden toegevoegd met specifieke indexeringsopties.

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

### Zie ook

* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Add(Document[], IndexingOptions) {#add}

Voert een indexeerbewerking uit. Voegt documenten toe vanuit het bestandssysteem, een stream of een structuur.

```csharp
public void Add(Document[] documents, IndexingOptions options)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| documenten | Document[] | De documenten uit het bestandssysteem, de stroom of de structuur. |
| opties | IndexingOptions | De indexeringsopties. |

### Zie ook

* class [Document](../../../groupdocs.search.common/document)
* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Add(ExtractedData[], IndexingOptions) {#add_1}

Voert een indexeerbewerking uit. Voegt de geëxtraheerde gegevens toe aan de index.

```csharp
public void Add(ExtractedData[] data, IndexingOptions options)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| gegevens | ExtractedData[] | De geëxtraheerde gegevens. |
| opties | IndexingOptions | De indexeringsopties. |

### Zie ook

* class [ExtractedData](../../../groupdocs.search.common/extracteddata)
* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.search.dll -->
