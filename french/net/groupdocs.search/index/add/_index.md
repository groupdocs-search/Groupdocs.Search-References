---
title: Add
second_title: Référence de l'API GroupDocs.Search pour .NET
description: Effectue une opération dindexation. Ajoute un fichier ou un dossier par un chemin absolu ou relatif. Les documents de tous les sousdossiers seront indexés.
type: docs
weight: 70
url: /fr/net/groupdocs.search/index/add/
---
## Add(string) {#add_2}

Effectue une opération d'indexation. Ajoute un fichier ou un dossier par un chemin absolu ou relatif. Les documents de tous les sous-dossiers seront indexés.

```csharp
public void Add(string path)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| path | String | Chemin d'accès à un fichier ou dossier à indexer. |

### Exemples

L'exemple montre comment ajouter des documents à un index.

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // Création d'un index dans le dossier spécifié
index.Add(folderPath); // Indexation des documents dans le dossier spécifié
index.Add(filePath); // Indexation du document spécifié
```

### Voir également

* class [Index](../../index)
* espace de noms [GroupDocs.Search](../../index)
* Assemblée [GroupDocs.Search](../../../)

---

## Add(string, IndexingOptions) {#add_3}

Effectue une opération d'indexation. Ajoute un fichier ou un dossier par un chemin absolu ou relatif. Les documents de tous les sous-dossiers seront indexés.

```csharp
public void Add(string path, IndexingOptions options)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| path | String | Chemin d'accès à un fichier ou dossier à indexer. |
| options | IndexingOptions | Les options d'indexation. |

### Exemples

L'exemple montre comment ajouter des documents à un index avec des options d'indexation particulières.

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // Création d'un index dans le dossier spécifié

IndexingOptions options = new IndexingOptions();
options.Threads = 2; // Définition du nombre de threads d'indexation
index.Add(folderPath, options); // Indexation des documents dans le dossier spécifié
index.Add(filePath, options); // Indexation du document spécifié
```

### Voir également

* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* espace de noms [GroupDocs.Search](../../index)
* Assemblée [GroupDocs.Search](../../../)

---

## Add(string[]) {#add_4}

Effectue une opération d'indexation. Ajoute des fichiers ou des dossiers par un chemin absolu ou relatif. Les documents de tous les sous-dossiers seront indexés.

```csharp
public void Add(string[] paths)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| paths | String[] | Chemins d'accès aux fichiers ou dossiers à indexer. |

### Exemples

L'exemple montre comment ajouter des documents à un index.

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // Création d'un index dans le dossier spécifié

string[] paths = new string[] { folderPath, filePath };
index.Add(paths); // Indexation des documents aux chemins spécifiés
```

### Voir également

* class [Index](../../index)
* espace de noms [GroupDocs.Search](../../index)
* Assemblée [GroupDocs.Search](../../../)

---

## Add(string[], IndexingOptions) {#add_5}

Effectue une opération d'indexation. Ajoute des fichiers ou des dossiers par un chemin absolu ou relatif. Les documents de tous les sous-dossiers seront indexés.

```csharp
public void Add(string[] paths, IndexingOptions options)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| paths | String[] | Chemins d'accès aux fichiers ou dossiers à indexer. |
| options | IndexingOptions | Les options d'indexation. |

### Exemples

L'exemple montre comment ajouter des documents à un index avec des options d'indexation particulières.

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // Création d'un index dans le dossier spécifié

IndexingOptions options = new IndexingOptions();
options.Threads = 2; // Définition du nombre de threads d'indexation
string[] paths = new string[] { folderPath, filePath };
index.Add(paths, options); // Indexation des documents aux chemins spécifiés
```

### Voir également

* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* espace de noms [GroupDocs.Search](../../index)
* Assemblée [GroupDocs.Search](../../../)

---

## Add(Document[], IndexingOptions) {#add}

Effectue une opération d'indexation. Ajoute des documents à partir du système de fichiers, du flux ou de la structure.

```csharp
public void Add(Document[] documents, IndexingOptions options)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| documents | Document[] | Les documents du système de fichiers, du flux ou de la structure. |
| options | IndexingOptions | Les options d'indexation. |

### Voir également

* class [Document](../../../groupdocs.search.common/document)
* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* espace de noms [GroupDocs.Search](../../index)
* Assemblée [GroupDocs.Search](../../../)

---

## Add(ExtractedData[], IndexingOptions) {#add_1}

Effectue l'opération d'indexation. Ajoute les données extraites à l'index.

```csharp
public void Add(ExtractedData[] data, IndexingOptions options)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| data | ExtractedData[] | Les données extraites. |
| options | IndexingOptions | Les options d'indexation. |

### Voir également

* class [ExtractedData](../../../groupdocs.search.common/extracteddata)
* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* espace de noms [GroupDocs.Search](../../index)
* Assemblée [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
