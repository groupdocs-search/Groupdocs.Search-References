---
title: "Create"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Crée un nouvel index en mémoire."
type: docs
weight: 50
url: /fr/net/groupdocs.search/indexrepository/create/
---
## Create() {#create}

Crée un nouvel index en mémoire.

```csharp
public Index Create()
```

### Valeur de retour

L'index créé.

### Exemples

L'exemple montre comment créer un index en mémoire via le référentiel d'index.

```csharp
IndexRepository indexRepository = new IndexRepository();
Index index = indexRepository.Create();
```

### Voir aussi

* class [Index](../../index)
* class [IndexRepository](../../indexrepository)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Create(IndexSettings) {#create_1}

Crée un nouvel index en mémoire.

```csharp
public Index Create(IndexSettings settings)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| settings | IndexSettings | Les paramètres de l'index. |

### Valeur de retour

L'index créé.

### Exemples

L'exemple montre comment créer un index en mémoire via le référentiel d'index.

```csharp
IndexRepository indexRepository = new IndexRepository();

IndexSettings settings = new IndexSettings();
settings.UseStopWords = false; // Disabling use of stop words during indexing

Index index = indexRepository.Create(settings);
```

### Voir aussi

* class [Index](../../index)
* class [IndexSettings](../../indexsettings)
* class [IndexRepository](../../indexrepository)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Create(string) {#create_2}

Crée un nouvel index sur disque. Le dossier d'index sera nettoyé avant la création de l'index.

```csharp
public Index Create(string indexFolder)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| indexFolder | String | Le dossier d'index. |

### Valeur de retour

L'index créé.

### Exemples

L'exemple montre comment créer un index sur disque via le référentiel d'index.

```csharp
string indexFolder = @"c:\MyIndex\";

IndexRepository indexRepository = new IndexRepository();
Index index = indexRepository.Create(indexFolder);
```

### Voir aussi

* class [Index](../../index)
* class [IndexRepository](../../indexrepository)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Create(string, IndexSettings) {#create_3}

Crée un nouvel index sur disque. Le dossier d'index sera nettoyé avant la création de l'index.

```csharp
public Index Create(string indexFolder, IndexSettings settings)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| indexFolder | String | Le dossier d'index. |
| settings | IndexSettings | Les paramètres de l'index. |

### Valeur de retour

L'index créé.

### Exemples

L'exemple montre comment créer un index sur disque via le référentiel d'index.

```csharp
string indexFolder = @"c:\MyIndex\";

IndexRepository indexRepository = new IndexRepository();

IndexSettings settings = new IndexSettings();
settings.UseStopWords = false; // Disabling use of stop words during indexing

Index index = indexRepository.Create(indexFolder, settings);
```

### Voir aussi

* class [Index](../../index)
* class [IndexSettings](../../indexsettings)
* class [IndexRepository](../../indexrepository)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
