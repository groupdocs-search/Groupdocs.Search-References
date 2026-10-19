---
title: "Add"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Esegue l'operazione di indicizzazione. Aggiunge un file o una cartella tramite un percorso assoluto o relativo. I documenti di tutte le sottocartelle verranno indicizzati."
type: docs
weight: 80
url: /it/net/groupdocs.search/index/add/
---
## Add(string) {#add_2}

Esegue l'operazione di indicizzazione. Aggiunge un file o una cartella tramite un percorso assoluto o relativo. I documenti di tutte le sottocartelle verranno indicizzati.

```csharp
public void Add(string path)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| percorso | String | Il percorso a un file o cartella da indicizzare. |

### Esempi

L'esempio dimostra come aggiungere documenti a un indice.

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(folderPath); // Indexing documents in the specified folder
index.Add(filePath); // Indexing the specified document
```

### Vedi anche

* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Add(string, IndexingOptions) {#add_3}

Esegue l'operazione di indicizzazione. Aggiunge un file o una cartella tramite un percorso assoluto o relativo. I documenti di tutte le sottocartelle verranno indicizzati.

```csharp
public void Add(string path, IndexingOptions options)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| percorso | String | Il percorso a un file o cartella da indicizzare. |
| opzioni | IndexingOptions | Le opzioni di indicizzazione. |

### Esempi

L'esempio dimostra come aggiungere documenti a un indice con specifiche opzioni di indicizzazione.

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

### Vedi anche

* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Add(string[]) {#add_4}

Esegue l'operazione di indicizzazione. Aggiunge file o cartelle tramite un percorso assoluto o relativo. I documenti di tutte le sottocartelle verranno indicizzati.

```csharp
public void Add(string[] paths)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| percorsi | String[] | I percorsi a file o cartelle da indicizzare. |

### Esempi

L'esempio dimostra come aggiungere documenti a un indice.

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // Creating index in the specified folder

string[] paths = new string[] { folderPath, filePath };
index.Add(paths); // Indexing documents at the specified paths
```

### Vedi anche

* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Add(string[], IndexingOptions) {#add_5}

Esegue l'operazione di indicizzazione. Aggiunge file o cartelle tramite un percorso assoluto o relativo. I documenti di tutte le sottocartelle verranno indicizzati.

```csharp
public void Add(string[] paths, IndexingOptions options)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| percorsi | String[] | I percorsi a file o cartelle da indicizzare. |
| opzioni | IndexingOptions | Le opzioni di indicizzazione. |

### Esempi

L'esempio dimostra come aggiungere documenti a un indice con specifiche opzioni di indicizzazione.

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

### Vedi anche

* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Add(Document[], IndexingOptions) {#add}

Esegue l'operazione di indicizzazione. Aggiunge documenti dal file system, dallo stream o dalla struttura.

```csharp
public void Add(Document[] documents, IndexingOptions options)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| documenti | Document[] | I documenti dal file system, dal flusso o dalla struttura. |
| opzioni | IndexingOptions | Le opzioni di indicizzazione. |

### Vedi anche

* class [Document](../../../groupdocs.search.common/document)
* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Add(ExtractedData[], IndexingOptions) {#add_1}

Esegue l'operazione di indicizzazione. Aggiunge i dati estratti all'indice.

```csharp
public void Add(ExtractedData[] data, IndexingOptions options)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| dati | ExtractedData[] | I dati estratti. |
| opzioni | IndexingOptions | Le opzioni di indicizzazione. |

### Vedi anche

* class [ExtractedData](../../../groupdocs.search.common/extracteddata)
* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
