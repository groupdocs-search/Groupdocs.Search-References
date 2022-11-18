---
title: Add
second_title: GroupDocs.Cerca il riferimento dell'API .NET
description: Esegue unoperazione di indicizzazione. Aggiunge un file o una cartella in base a un percorso assoluto o relativo. I documenti di tutte le sottocartelle verranno indicizzati.
type: docs
weight: 70
url: /it/net/groupdocs.search/index/add/
---
## Add(string) {#add_2}

Esegue un'operazione di indicizzazione. Aggiunge un file o una cartella in base a un percorso assoluto o relativo. I documenti di tutte le sottocartelle verranno indicizzati.

```csharp
public void Add(string path)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| path | String | Il percorso di un file o di una cartella da indicizzare. |

### Esempi

L'esempio mostra come aggiungere documenti a un indice.

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // Creazione dell'indice nella cartella specificata
index.Add(folderPath); // Indicizzazione dei documenti nella cartella specificata
index.Add(filePath); // Indicizzazione del documento specificato
```

### Guarda anche

* class [Index](../../index)
* spazio dei nomi [GroupDocs.Search](../../index)
* assemblea [GroupDocs.Search](../../../)

---

## Add(string, IndexingOptions) {#add_3}

Esegue un'operazione di indicizzazione. Aggiunge un file o una cartella in base a un percorso assoluto o relativo. I documenti di tutte le sottocartelle verranno indicizzati.

```csharp
public void Add(string path, IndexingOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| path | String | Il percorso di un file o di una cartella da indicizzare. |
| options | IndexingOptions | Le opzioni di indicizzazione. |

### Esempi

L'esempio mostra come aggiungere documenti a un indice con particolari opzioni di indicizzazione.

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // Creazione dell'indice nella cartella specificata

IndexingOptions options = new IndexingOptions();
options.Threads = 2; // Impostazione del numero di thread di indicizzazione
index.Add(folderPath, options); // Indicizzazione dei documenti nella cartella specificata
index.Add(filePath, options); // Indicizzazione del documento specificato
```

### Guarda anche

* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* spazio dei nomi [GroupDocs.Search](../../index)
* assemblea [GroupDocs.Search](../../../)

---

## Add(string[]) {#add_4}

Esegue un'operazione di indicizzazione. Aggiunge file o cartelle in base a un percorso assoluto o relativo. I documenti di tutte le sottocartelle verranno indicizzati.

```csharp
public void Add(string[] paths)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| paths | String[] | I percorsi di file o cartelle da indicizzare. |

### Esempi

L'esempio mostra come aggiungere documenti a un indice.

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // Creazione dell'indice nella cartella specificata

string[] paths = new string[] { folderPath, filePath };
index.Add(paths); // Indicizzazione dei documenti nei percorsi specificati
```

### Guarda anche

* class [Index](../../index)
* spazio dei nomi [GroupDocs.Search](../../index)
* assemblea [GroupDocs.Search](../../../)

---

## Add(string[], IndexingOptions) {#add_5}

Esegue un'operazione di indicizzazione. Aggiunge file o cartelle in base a un percorso assoluto o relativo. I documenti di tutte le sottocartelle verranno indicizzati.

```csharp
public void Add(string[] paths, IndexingOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| paths | String[] | I percorsi di file o cartelle da indicizzare. |
| options | IndexingOptions | Le opzioni di indicizzazione. |

### Esempi

L'esempio mostra come aggiungere documenti a un indice con particolari opzioni di indicizzazione.

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // Creazione dell'indice nella cartella specificata

IndexingOptions options = new IndexingOptions();
options.Threads = 2; // Impostazione del numero di thread di indicizzazione
string[] paths = new string[] { folderPath, filePath };
index.Add(paths, options); // Indicizzazione dei documenti nei percorsi specificati
```

### Guarda anche

* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* spazio dei nomi [GroupDocs.Search](../../index)
* assemblea [GroupDocs.Search](../../../)

---

## Add(Document[], IndexingOptions) {#add}

Esegue un'operazione di indicizzazione. Aggiunge documenti da file system, flusso o struttura.

```csharp
public void Add(Document[] documents, IndexingOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| documents | Document[] | I documenti dal file system, dal flusso o dalla struttura. |
| options | IndexingOptions | Le opzioni di indicizzazione. |

### Guarda anche

* class [Document](../../../groupdocs.search.common/document)
* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* spazio dei nomi [GroupDocs.Search](../../index)
* assemblea [GroupDocs.Search](../../../)

---

## Add(ExtractedData[], IndexingOptions) {#add_1}

Esegue l'operazione di indicizzazione. Aggiunge i dati estratti all'indice.

```csharp
public void Add(ExtractedData[] data, IndexingOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| data | ExtractedData[] | I dati estratti. |
| options | IndexingOptions | Le opzioni di indicizzazione. |

### Guarda anche

* class [ExtractedData](../../../groupdocs.search.common/extracteddata)
* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* spazio dei nomi [GroupDocs.Search](../../index)
* assemblea [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
