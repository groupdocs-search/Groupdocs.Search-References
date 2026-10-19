---
title: "Aggiorna"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Reindicizza i documenti che sono stati modificati o eliminati dall'ultimo aggiornamento. Aggiunge i nuovi file che sono stati aggiunti alle cartelle indicizzate."
type: docs
weight: 280
url: /it/net/groupdocs.search/index/update/
---
## Update() {#update}

Reindicizza i documenti che sono stati modificati o eliminati dall'ultimo aggiornamento. Aggiunge i nuovi file inseriti nelle cartelle indicizzate.

```csharp
public void Update()
```

### Esempi

L'esempio dimostra come aggiornare un indice.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

// Elimina i documenti dalla cartella dei documenti o modificali o aggiungi nuovi documenti alla cartella

index.Update(); // Updating the index
```

### Vedi anche

* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Update(UpdateOptions) {#update_1}

Reindicizza i documenti che sono stati modificati o eliminati dall'ultimo aggiornamento. Aggiunge i nuovi file inseriti nelle cartelle indicizzate.

```csharp
public void Update(UpdateOptions options)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| opzioni | UpdateOptions | Le opzioni di aggiornamento. |

### Esempi

L'esempio dimostra come aggiornare un indice con opzioni di aggiornamento specifiche.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

// Elimina i documenti dalla cartella dei documenti o modificali o aggiungi nuovi documenti alla cartella

UpdateOptions options = new UpdateOptions();
options.Threads = 2; // Setting the number of indexing threads
index.Update(options); // Updating the index
```

### Vedi anche

* class [UpdateOptions](../../../groupdocs.search.options/updateoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
