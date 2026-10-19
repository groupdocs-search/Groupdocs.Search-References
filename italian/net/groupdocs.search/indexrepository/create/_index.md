---
title: "Create"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Crea un nuovo indice in memoria."
type: docs
weight: 50
url: /it/net/groupdocs.search/indexrepository/create/
---
## Create() {#create}

Crea un nuovo indice in memoria.

```csharp
public Index Create()
```

### Valore di ritorno

L'indice creato.

### Esempi

L'esempio dimostra come creare un indice in memoria tramite il repository degli indici.

```csharp
IndexRepository indexRepository = new IndexRepository();
Index index = indexRepository.Create();
```

### Vedi anche

* class [Index](../../index)
* class [IndexRepository](../../indexrepository)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Create(IndexSettings) {#create_1}

Crea un nuovo indice in memoria.

```csharp
public Index Create(IndexSettings settings)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| settings | IndexSettings | Le impostazioni dell'indice. |

### Valore di ritorno

L'indice creato.

### Esempi

L'esempio dimostra come creare un indice in memoria tramite il repository degli indici.

```csharp
IndexRepository indexRepository = new IndexRepository();

IndexSettings settings = new IndexSettings();
settings.UseStopWords = false; // Disabling use of stop words during indexing

Index index = indexRepository.Create(settings);
```

### Vedi anche

* class [Index](../../index)
* class [IndexSettings](../../indexsettings)
* class [IndexRepository](../../indexrepository)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Create(string) {#create_2}

Crea un nuovo indice su disco. La cartella dell'indice verrà pulita prima della creazione dell'indice.

```csharp
public Index Create(string indexFolder)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| indexFolder | String | La cartella dell'indice. |

### Valore di ritorno

L'indice creato.

### Esempi

L'esempio dimostra come creare un indice su disco tramite il repository degli indici.

```csharp
string indexFolder = @"c:\MyIndex\";

IndexRepository indexRepository = new IndexRepository();
Index index = indexRepository.Create(indexFolder);
```

### Vedi anche

* class [Index](../../index)
* class [IndexRepository](../../indexrepository)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Create(string, IndexSettings) {#create_3}

Crea un nuovo indice su disco. La cartella dell'indice verrà pulita prima della creazione dell'indice.

```csharp
public Index Create(string indexFolder, IndexSettings settings)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| indexFolder | String | La cartella dell'indice. |
| settings | IndexSettings | Le impostazioni dell'indice. |

### Valore di ritorno

L'indice creato.

### Esempi

L'esempio dimostra come creare un indice su disco tramite il repository degli indici.

```csharp
string indexFolder = @"c:\MyIndex\";

IndexRepository indexRepository = new IndexRepository();

IndexSettings settings = new IndexSettings();
settings.UseStopWords = false; // Disabling use of stop words during indexing

Index index = indexRepository.Create(indexFolder, settings);
```

### Vedi anche

* class [Index](../../index)
* class [IndexSettings](../../indexsettings)
* class [IndexRepository](../../indexrepository)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
