---
title: "Index"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Initialise une nouvelle instance de la classe Indexgroupdocs.search/index en mémoire."
type: docs
weight: 10
url: /fr/net/groupdocs.search/index/index/
---
## Index() {#constructor}

Initialise une nouvelle instance de la classe [`Index`](../../index) en mémoire.

```csharp
public Index()
```

### Exemples

L'exemple montre comment créer un index en mémoire sans enregistrer les fichiers sur le disque.

```csharp
Index index = new Index(); 
```

### Voir aussi

* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Index(IndexSettings) {#constructor_1}

Initialise une nouvelle instance de la classe [`Index`](../../index) en mémoire avec des paramètres d'index particuliers.

```csharp
public Index(IndexSettings settings)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| settings | IndexSettings | L'objet de paramètres d'index. |

### Exemples

L'exemple montre comment créer un index en mémoire sans enregistrer les fichiers sur le disque avec des paramètres d'index particuliers.

```csharp
IndexSettings settings = new IndexSettings();
settings.IndexType = IndexType.CompactIndex;
Index index = new Index(settings);
```

### Voir aussi

* class [IndexSettings](../../indexsettings)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Index(string) {#constructor_2}

Initialise une nouvelle instance de la classe [`Index`](../../index). Crée un nouvel index ou ouvre un index existant sur le disque.

```csharp
public Index(string indexFolder)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| indexFolder | String | Le chemin du dossier d'index. |

### Exemples

L'exemple montre comment créer un index sur le disque ou ouvrir un index existé.

```csharp
string indexFolder = @"c:\MyIndex\";
Index index = new Index(indexFolder); 
```

### Voir aussi

* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Index(string, IndexSettings) {#constructor_4}

Initialise une nouvelle instance de la classe [`Index`](../../index). Crée un nouvel index avec des paramètres particuliers ou ouvre un index existant sur le disque.

```csharp
public Index(string indexFolder, IndexSettings settings)
```

| Paramètre | Type | Description |
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

### Voir aussi

* class [IndexSettings](../../indexsettings)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Index(string, bool) {#constructor_3}

Initialise une nouvelle instance de la classe [`Index`](../../index). Charge un index existant depuis le disque si *overwriteIfExists* est `false` ; crée un nouvel index sur le disque sinon.

```csharp
public Index(string indexFolder, bool overwriteIfExists)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| indexFolder | String | Le chemin du dossier d'index. |
| overwriteIfExists | Boolean | Le drapeau de remplacement du dossier d'index. |

### Exemples

L'exemple montre comment créer un nouvel index dans un dossier qui contient déjà un autre index.

```csharp
string indexFolder = @"c:\MyIndex\";
Index index = new Index(indexFolder, true);
```

### Voir aussi

* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Index(string, IndexSettings, bool) {#constructor_5}

Initialise une nouvelle instance de la classe [`Index`](../../index). Charge un index existant depuis le disque si *overwriteIfExists* est `false` ; crée un nouvel index sur le disque avec des paramètres d'index particuliers sinon.

```csharp
public Index(string indexFolder, IndexSettings settings, bool overwriteIfExists)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| indexFolder | String | Le chemin du dossier d'index. |
| settings | IndexSettings | L'objet de paramètres d'index. |
| overwriteIfExists | Boolean | Le drapeau de remplacement du dossier d'index. |

### Exemples

L'exemple montre comment créer un index sur un disque avec des paramètres d'index particuliers.

```csharp
string indexFolder = @"c:\MyIndex\";
IndexSettings settings = new IndexSettings();
settings.IndexType = IndexType.CompactIndex;
Index index = new Index(indexFolder, settings, true);
```

### Voir aussi

* class [IndexSettings](../../indexsettings)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
