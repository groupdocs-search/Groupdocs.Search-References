---
title: "Hinzufügen"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Führt einen Indexierungsvorgang aus. Fügt eine Datei oder einen Ordner über einen absoluten oder relativen Pfad hinzu. Dokumente aus allen Unterordnern werden indexiert."
type: docs
weight: 80
url: /de/net/groupdocs.search/index/add/
---
## Add(string) {#add_2}

Führt einen Indexierungsvorgang aus. Fügt eine Datei oder einen Ordner über einen absoluten oder relativen Pfad hinzu. Dokumente aus allen Unterordnern werden indexiert.

```csharp
public void Add(string path)
```

| Parameter | Type | Beschreibung |
| --- | --- | --- |
| path | String | Der Pfad zu einer Datei oder einem Ordner, der indiziert werden soll. |

### Beispiele

Das Beispiel zeigt, wie Dokumente zu einem Index hinzugefügt werden.

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(folderPath); // Indexing documents in the specified folder
index.Add(filePath); // Indexing the specified document
```

### Siehe auch

* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Add(string, IndexingOptions) {#add_3}

Führt einen Indexierungsvorgang aus. Fügt eine Datei oder einen Ordner über einen absoluten oder relativen Pfad hinzu. Dokumente aus allen Unterordnern werden indexiert.

```csharp
public void Add(string path, IndexingOptions options)
```

| Parameter | Type | Beschreibung |
| --- | --- | --- |
| path | String | Der Pfad zu einer Datei oder einem Ordner, der indiziert werden soll. |
| Optionen | IndexingOptions | Die Indexierungsoptionen. |

### Beispiele

Das Beispiel demonstriert, wie man Dokumente zu einem Index mit bestimmten Indexierungsoptionen hinzufügt.

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

### Siehe auch

* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Add(string[]) {#add_4}

Führt einen Indexierungsvorgang aus. Fügt Dateien oder Ordner über einen absoluten oder relativen Pfad hinzu. Dokumente aus allen Unterordnern werden indexiert.

```csharp
public void Add(string[] paths)
```

| Parameter | Type | Beschreibung |
| --- | --- | --- |
| paths | String[] | Die Pfade zu Dateien oder Ordnern, die indiziert werden sollen. |

### Beispiele

Das Beispiel zeigt, wie Dokumente zu einem Index hinzugefügt werden.

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // Creating index in the specified folder

string[] paths = new string[] { folderPath, filePath };
index.Add(paths); // Indexing documents at the specified paths
```

### Siehe auch

* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Add(string[], IndexingOptions) {#add_5}

Führt einen Indexierungsvorgang aus. Fügt Dateien oder Ordner über einen absoluten oder relativen Pfad hinzu. Dokumente aus allen Unterordnern werden indexiert.

```csharp
public void Add(string[] paths, IndexingOptions options)
```

| Parameter | Type | Beschreibung |
| --- | --- | --- |
| paths | String[] | Die Pfade zu Dateien oder Ordnern, die indiziert werden sollen. |
| Optionen | IndexingOptions | Die Indexierungsoptionen. |

### Beispiele

Das Beispiel demonstriert, wie man Dokumente zu einem Index mit bestimmten Indexierungsoptionen hinzufügt.

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

### Siehe auch

* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Add(Document[], IndexingOptions) {#add}

Führt einen Indexierungsvorgang aus. Fügt Dokumente aus dem Dateisystem, Stream oder einer Struktur hinzu.

```csharp
public void Add(Document[] documents, IndexingOptions options)
```

| Parameter | Type | Beschreibung |
| --- | --- | --- |
| Dokumente | Document[] | Die Dokumente aus dem Dateisystem, Stream oder einer Struktur. |
| Optionen | IndexingOptions | Die Indexierungsoptionen. |

### Siehe auch

* class [Document](../../../groupdocs.search.common/document)
* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Add(ExtractedData[], IndexingOptions) {#add_1}

Führt einen Indexierungsvorgang aus. Fügt die extrahierten Daten dem Index hinzu.

```csharp
public void Add(ExtractedData[] data, IndexingOptions options)
```

| Parameter | Type | Beschreibung |
| --- | --- | --- |
| Daten | ExtractedData[] | Die extrahierten Daten. |
| Optionen | IndexingOptions | Die Indexierungsoptionen. |

### Siehe auch

* class [ExtractedData](../../../groupdocs.search.common/extracteddata)
* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
