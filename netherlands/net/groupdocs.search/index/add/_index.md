---
title: Add
second_title: GroupDocs. Zoek naar .NET API-referentie
description: Voert indexering uit. Voegt een bestand of map toe via een absoluut of relatief pad. Documenten uit alle submappen worden geïndexeerd.
type: docs
weight: 70
url: /nl/net/groupdocs.search/index/add/
---
## Add(string) {#add_2}

Voert indexering uit. Voegt een bestand of map toe via een absoluut of relatief pad. Documenten uit alle submappen worden geïndexeerd.

```csharp
public void Add(string path)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| path | String | Het pad naar een te indexeren bestand of map. |

### Voorbeelden

Het voorbeeld laat zien hoe u documenten toevoegt aan een index.

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // Index maken in de opgegeven map
index.Add(folderPath); // Documenten indexeren in de opgegeven map
index.Add(filePath); // Het opgegeven document indexeren
```

### Zie ook

* class [Index](../../index)
* naamruimte [GroupDocs.Search](../../index)
* montage [GroupDocs.Search](../../../)

---

## Add(string, IndexingOptions) {#add_3}

Voert indexering uit. Voegt een bestand of map toe via een absoluut of relatief pad. Documenten uit alle submappen worden geïndexeerd.

```csharp
public void Add(string path, IndexingOptions options)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| path | String | Het pad naar een te indexeren bestand of map. |
| options | IndexingOptions | De indexeringsopties. |

### Voorbeelden

Het voorbeeld laat zien hoe u documenten kunt toevoegen aan een index met bepaalde indexeringsopties.

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // Index maken in de opgegeven map

IndexingOptions options = new IndexingOptions();
options.Threads = 2; // Het aantal indexthreads instellen
index.Add(folderPath, options); // Documenten indexeren in de opgegeven map
index.Add(filePath, options); // Het opgegeven document indexeren
```

### Zie ook

* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* naamruimte [GroupDocs.Search](../../index)
* montage [GroupDocs.Search](../../../)

---

## Add(string[]) {#add_4}

Voert indexering uit. Voegt bestanden of mappen toe via een absoluut of relatief pad. Documenten uit alle submappen worden geïndexeerd.

```csharp
public void Add(string[] paths)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| paths | String[] | De paden naar bestanden of mappen die moeten worden geïndexeerd. |

### Voorbeelden

Het voorbeeld laat zien hoe u documenten toevoegt aan een index.

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // Index maken in de opgegeven map

string[] paths = new string[] { folderPath, filePath };
index.Add(paths); // Documenten indexeren op de opgegeven paden
```

### Zie ook

* class [Index](../../index)
* naamruimte [GroupDocs.Search](../../index)
* montage [GroupDocs.Search](../../../)

---

## Add(string[], IndexingOptions) {#add_5}

Voert indexering uit. Voegt bestanden of mappen toe via een absoluut of relatief pad. Documenten uit alle submappen worden geïndexeerd.

```csharp
public void Add(string[] paths, IndexingOptions options)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| paths | String[] | De paden naar bestanden of mappen die moeten worden geïndexeerd. |
| options | IndexingOptions | De indexeringsopties. |

### Voorbeelden

Het voorbeeld laat zien hoe u documenten kunt toevoegen aan een index met bepaalde indexeringsopties.

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // Index maken in de opgegeven map

IndexingOptions options = new IndexingOptions();
options.Threads = 2; // Het aantal indexthreads instellen
string[] paths = new string[] { folderPath, filePath };
index.Add(paths, options); // Documenten indexeren op de opgegeven paden
```

### Zie ook

* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* naamruimte [GroupDocs.Search](../../index)
* montage [GroupDocs.Search](../../../)

---

## Add(Document[], IndexingOptions) {#add}

Voert indexering uit. Voegt documenten toe vanuit bestandssysteem, stream of structuur.

```csharp
public void Add(Document[] documents, IndexingOptions options)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| documents | Document[] | De documenten uit bestandssysteem, stream of structuur. |
| options | IndexingOptions | De indexeringsopties. |

### Zie ook

* class [Document](../../../groupdocs.search.common/document)
* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* naamruimte [GroupDocs.Search](../../index)
* montage [GroupDocs.Search](../../../)

---

## Add(ExtractedData[], IndexingOptions) {#add_1}

Voert indexering uit. Voegt de geëxtraheerde gegevens toe aan de index.

```csharp
public void Add(ExtractedData[] data, IndexingOptions options)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| data | ExtractedData[] | De geëxtraheerde gegevens. |
| options | IndexingOptions | De indexeringsopties. |

### Zie ook

* class [ExtractedData](../../../groupdocs.search.common/extracteddata)
* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* naamruimte [GroupDocs.Search](../../index)
* montage [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
