---
title: Index
second_title: Référence de l'API GroupDocs.Search pour .NET
description: Initialise une nouvelle instance duIndexgroupdocs.search/index classe en mémoire.
type: docs
weight: 10
url: /fr/net/groupdocs.search/index/index/
---
## Index() {#constructor}

Initialise une nouvelle instance du[`Index`](../../index) classe en mémoire.

```csharp
public Index()
```

### Exemples

L'exemple montre comment créer un index en mémoire sans enregistrer les fichiers sur le disque.

```csharp
Index index = new Index(); 
```

### Voir également

* class [Index](../../index)
* espace de noms [GroupDocs.Search](../../index)
* Assemblée [GroupDocs.Search](../../../)

---

## Index(IndexSettings) {#constructor_1}

Initialise une nouvelle instance du[`Index`](../../index) classe en mémoire avec des paramètres d'index particuliers.

```csharp
public Index(IndexSettings settings)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| settings | IndexSettings | L'objet de paramètres d'index. |

### Exemples

L'exemple montre comment créer un index en mémoire sans enregistrer les fichiers sur le disque avec des paramètres d'index particuliers.

```csharp
IndexSettings settings = new IndexSettings();
settings.IndexType = IndexType.CompactIndex;
Index index = new Index(settings);
```

### Voir également

* class [IndexSettings](../../indexsettings)
* class [Index](../../index)
* espace de noms [GroupDocs.Search](../../index)
* Assemblée [GroupDocs.Search](../../../)

---

## Index(string) {#constructor_2}

Initialise une nouvelle instance du[`Index`](../../index) class. Crée un nouvel index ou ouvre un index existant sur le disque.

```csharp
public Index(string indexFolder)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| indexFolder | String | Le chemin du dossier d'index. |

### Exemples

L'exemple montre comment créer un index sur un disque ou ouvrir un index existant.

```csharp
string indexFolder = @"c:\MyIndex\";
Index index = new Index(indexFolder); 
```

### Voir également

* class [Index](../../index)
* espace de noms [GroupDocs.Search](../../index)
* Assemblée [GroupDocs.Search](../../../)

---

## Index(string, IndexSettings) {#constructor_4}

Initialise une nouvelle instance du[`Index`](../../index) class. Crée un nouvel index avec des paramètres particuliers ou ouvre un index existant sur le disque.

```csharp
public Index(string indexFolder, IndexSettings settings)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| indexFolder | String | Le chemin du dossier d'index. |
| settings | IndexSettings | L'objet de paramètres d'index. |

### Exemples

L'exemple montre comment créer un index sur un disque avec des paramètres d'index particuliers.

```csharp
string indexFolder = @"c:\MyIndex\";
IndexSettings settings = new IndexSettings();
settings.IndexType = IndexType.CompactIndex;
Index index = new Index(indexFolder, settings);
```

### Voir également

* class [IndexSettings](../../indexsettings)
* class [Index](../../index)
* espace de noms [GroupDocs.Search](../../index)
* Assemblée [GroupDocs.Search](../../../)

---

## Index(string, bool) {#constructor_3}

Initialise une nouvelle instance du[`Index`](../../index) class. Charge un index existant à partir du disque si*overwriteIfExists* est`FAUX`; crée un nouvel index sur le disque sinon.

```csharp
public Index(string indexFolder, bool overwriteIfExists)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| indexFolder | String | Le chemin du dossier d'index. |
| overwriteIfExists | Boolean | L'indicateur d'écrasement du dossier d'index. |

### Exemples

L'exemple montre comment créer un nouvel index dans un dossier qui contient déjà un autre index.

```csharp
string indexFolder = @"c:\MyIndex\";
Index index = new Index(indexFolder, true);
```

### Voir également

* class [Index](../../index)
* espace de noms [GroupDocs.Search](../../index)
* Assemblée [GroupDocs.Search](../../../)

---

## Index(string, IndexSettings, bool) {#constructor_5}

Initialise une nouvelle instance du[`Index`](../../index) class. Charge un index existant à partir du disque si*overwriteIfExists* est`FAUX` ; crée un nouvel index sur le disque avec des paramètres d'index particuliers sinon.

```csharp
public Index(string indexFolder, IndexSettings settings, bool overwriteIfExists)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| indexFolder | String | Le chemin du dossier d'index. |
| settings | IndexSettings | L'objet de paramètres d'index. |
| overwriteIfExists | Boolean | L'indicateur d'écrasement du dossier d'index. |

### Exemples

L'exemple montre comment créer un index sur un disque avec des paramètres d'index particuliers.

```csharp
string indexFolder = @"c:\MyIndex\";
IndexSettings settings = new IndexSettings();
settings.IndexType = IndexType.CompactIndex;
Index index = new Index(indexFolder, settings, true);
```

### Voir également

* class [IndexSettings](../../indexsettings)
* class [Index](../../index)
* espace de noms [GroupDocs.Search](../../index)
* Assemblée [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
