---
title: "Aggiorna"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Aggiorna tutti gli indici nel repository."
type: docs
weight: 80
url: /it/net/groupdocs.search/indexrepository/update/
---
## Update() {#update}

Aggiorna tutti gli indici nel repository.

```csharp
public void Update()
```

### Esempi

L'esempio dimostra come aggiornare gli indici nel repository.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

IndexRepository repository = new IndexRepository();

Index index = repository.Create(indexFolder); // Creating index
index.Add(documentsFolder); // Indexing documents

// Elimina i documenti dalla cartella dei documenti o modificali o aggiungi nuovi documenti alla cartella

repository.Update();
```

### Vedi anche

* class [IndexRepository](../../indexrepository)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Update(UpdateOptions) {#update_1}

Aggiorna tutti gli indici nel repository.

```csharp
public void Update(UpdateOptions options)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| opzioni | UpdateOptions | Le opzioni di aggiornamento. |

### Esempi

L'esempio dimostra come aggiornare gli indici nel repository.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

IndexRepository repository = new IndexRepository();

Index index = repository.Create(indexFolder); // Creating index
index.Add(documentsFolder); // Indexing documents

// Elimina i documenti dalla cartella dei documenti o modificali o aggiungi nuovi documenti alla cartella

UpdateOptions options = new UpdateOptions();
options.Threads = 2; // Setting the number of indexing threads
repository.Update(options);
```

### Vedi anche

* class [UpdateOptions](../../../groupdocs.search.options/updateoptions)
* class [IndexRepository](../../indexrepository)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
