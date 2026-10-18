---
title: "Ajouter"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Effectue une opération d'indexation. Ajoute un fichier ou un dossier via un chemin absolu ou relatif. Les documents de tous les sous‑dossiers seront indexés."
type: docs
weight: 80
url: /fr/net/groupdocs.search/index/add/
---
## Add(string) {#add_2}

Effectue une opération d'indexation. Ajoute un fichier ou un dossier via un chemin absolu ou relatif. Les documents de tous les sous‑dossiers seront indexés.

```csharp
public void Add(string path)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| path | String | Le chemin vers un fichier ou un dossier à indexer. |

### Exemples

L'exemple montre comment ajouter des documents à un index.

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(folderPath); // Indexing documents in the specified folder
index.Add(filePath); // Indexing the specified document
```

### Voir aussi

* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Add(string, IndexingOptions) {#add_3}

Effectue une opération d'indexation. Ajoute un fichier ou un dossier via un chemin absolu ou relatif. Les documents de tous les sous‑dossiers seront indexés.

```csharp
public void Add(string path, IndexingOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| path | String | Le chemin vers un fichier ou un dossier à indexer. |
| options | IndexingOptions | Les options d'indexation. |

### Exemples

L'exemple montre comment ajouter des documents à un index avec des options d'indexation particulières.

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

### Voir aussi

* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Add(string[]) {#add_4}

Effectue une opération d'indexation. Ajoute des fichiers ou des dossiers via un chemin absolu ou relatif. Les documents de tous les sous‑dossiers seront indexés.

```csharp
public void Add(string[] paths)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| paths | String[] | Les chemins vers des fichiers ou dossiers à indexer. |

### Exemples

L'exemple montre comment ajouter des documents à un index.

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // Creating index in the specified folder

string[] paths = new string[] { folderPath, filePath };
index.Add(paths); // Indexing documents at the specified paths
```

### Voir aussi

* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Add(string[], IndexingOptions) {#add_5}

Effectue une opération d'indexation. Ajoute des fichiers ou des dossiers via un chemin absolu ou relatif. Les documents de tous les sous‑dossiers seront indexés.

```csharp
public void Add(string[] paths, IndexingOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| paths | String[] | Les chemins vers des fichiers ou dossiers à indexer. |
| options | IndexingOptions | Les options d'indexation. |

### Exemples

L'exemple montre comment ajouter des documents à un index avec des options d'indexation particulières.

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

### Voir aussi

* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Add(Document[], IndexingOptions) {#add}

Effectue une opération d'indexation. Ajoute des documents depuis le système de fichiers, un flux ou une structure.

```csharp
public void Add(Document[] documents, IndexingOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| documents | Document[] | Les documents provenant du système de fichiers, du flux ou de la structure. |
| options | IndexingOptions | Les options d'indexation. |

### Voir aussi

* class [Document](../../../groupdocs.search.common/document)
* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Add(ExtractedData[], IndexingOptions) {#add_1}

Effectue une opération d'indexation. Ajoute les données extraites à l'index.

```csharp
public void Add(ExtractedData[] data, IndexingOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| données | ExtractedData[] | Les données extraites. |
| options | IndexingOptions | Les options d'indexation. |

### Voir aussi

* class [ExtractedData](../../../groupdocs.search.common/extracteddata)
* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
