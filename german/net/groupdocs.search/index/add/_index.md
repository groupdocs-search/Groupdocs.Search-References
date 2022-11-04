---
title: Add
second_title: GroupDocs.Suche nach .NET-API-Referenz
description: Führt einen Indizierungsvorgang durch. Fügt eine Datei oder einen Ordner über einen absoluten oder relativen Pfad hinzu. Dokumente aus allen Unterordnern werden indiziert.
type: docs
weight: 70
url: /de/net/groupdocs.search/index/add/
---
## Add(string) {#add_2}

Führt einen Indizierungsvorgang durch. Fügt eine Datei oder einen Ordner über einen absoluten oder relativen Pfad hinzu. Dokumente aus allen Unterordnern werden indiziert.

```csharp
public void Add(string path)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| path | String | Der Pfad zu einer Datei oder einem Ordner, der indiziert werden soll. |

### Beispiele

Das Beispiel zeigt, wie Dokumente zu einem Index hinzugefügt werden.

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // Index im angegebenen Ordner erstellen
index.Add(folderPath); // Dokumente im angegebenen Ordner indizieren
index.Add(filePath); // Indizierung des angegebenen Dokuments
```

### Siehe auch

* class [Index](../../index)
* namensraum [GroupDocs.Search](../../index)
* Montage [GroupDocs.Search](../../../)

---

## Add(string, IndexingOptions) {#add_3}

Führt einen Indizierungsvorgang durch. Fügt eine Datei oder einen Ordner über einen absoluten oder relativen Pfad hinzu. Dokumente aus allen Unterordnern werden indiziert.

```csharp
public void Add(string path, IndexingOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| path | String | Der Pfad zu einer Datei oder einem Ordner, der indiziert werden soll. |
| options | IndexingOptions | Die Indizierungsoptionen. |

### Beispiele

Das Beispiel demonstriert das Hinzufügen von Dokumenten zu einem Index mit bestimmten Indizierungsoptionen.

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // Index im angegebenen Ordner erstellen

IndexingOptions options = new IndexingOptions();
options.Threads = 2; // Festlegen der Anzahl der Indizierungsthreads
index.Add(folderPath, options); // Dokumente im angegebenen Ordner indizieren
index.Add(filePath, options); // Indizierung des angegebenen Dokuments
```

### Siehe auch

* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* namensraum [GroupDocs.Search](../../index)
* Montage [GroupDocs.Search](../../../)

---

## Add(string[]) {#add_4}

Führt einen Indizierungsvorgang durch. Fügt Dateien oder Ordner über einen absoluten oder relativen Pfad hinzu. Dokumente aus allen Unterordnern werden indiziert.

```csharp
public void Add(string[] paths)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| paths | String[] | Die Pfade zu Dateien oder Ordnern, die indiziert werden sollen. |

### Beispiele

Das Beispiel zeigt, wie Dokumente zu einem Index hinzugefügt werden.

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // Index im angegebenen Ordner erstellen

string[] paths = new string[] { folderPath, filePath };
index.Add(paths); // Dokumente in den angegebenen Pfaden indizieren
```

### Siehe auch

* class [Index](../../index)
* namensraum [GroupDocs.Search](../../index)
* Montage [GroupDocs.Search](../../../)

---

## Add(string[], IndexingOptions) {#add_5}

Führt einen Indizierungsvorgang durch. Fügt Dateien oder Ordner über einen absoluten oder relativen Pfad hinzu. Dokumente aus allen Unterordnern werden indiziert.

```csharp
public void Add(string[] paths, IndexingOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| paths | String[] | Die Pfade zu Dateien oder Ordnern, die indiziert werden sollen. |
| options | IndexingOptions | Die Indizierungsoptionen. |

### Beispiele

Das Beispiel demonstriert das Hinzufügen von Dokumenten zu einem Index mit bestimmten Indizierungsoptionen.

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // Index im angegebenen Ordner erstellen

IndexingOptions options = new IndexingOptions();
options.Threads = 2; // Festlegen der Anzahl der Indizierungsthreads
string[] paths = new string[] { folderPath, filePath };
index.Add(paths, options); // Dokumente in den angegebenen Pfaden indizieren
```

### Siehe auch

* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* namensraum [GroupDocs.Search](../../index)
* Montage [GroupDocs.Search](../../../)

---

## Add(Document[], IndexingOptions) {#add}

Führt Indizierungsoperationen durch. Fügt Dokumente aus Dateisystem, Stream oder Struktur hinzu.

```csharp
public void Add(Document[] documents, IndexingOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| documents | Document[] | Die Dokumente aus Dateisystem, Stream oder Struktur. |
| options | IndexingOptions | Die Indizierungsoptionen. |

### Siehe auch

* class [Document](../../../groupdocs.search.common/document)
* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* namensraum [GroupDocs.Search](../../index)
* Montage [GroupDocs.Search](../../../)

---

## Add(ExtractedData[], IndexingOptions) {#add_1}

Führt den Indexierungsvorgang durch. Fügt die extrahierten Daten dem Index hinzu.

```csharp
public void Add(ExtractedData[] data, IndexingOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| data | ExtractedData[] | Die extrahierten Daten. |
| options | IndexingOptions | Die Indizierungsoptionen. |

### Siehe auch

* class [ExtractedData](../../../groupdocs.search.common/extracteddata)
* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* namensraum [GroupDocs.Search](../../index)
* Montage [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
