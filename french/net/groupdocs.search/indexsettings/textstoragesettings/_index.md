---
title: TextStorageSettings
second_title: Référence de l'API GroupDocs.Search pour .NET
description: Obtient ou définit les paramètres de stockage de texte. La valeur par défaut estnul  ce qui signifie que les textes des documents ne sont pas stockés.
type: docs
weight: 110
url: /fr/net/groupdocs.search/indexsettings/textstoragesettings/
---
## IndexSettings.TextStorageSettings property

Obtient ou définit les paramètres de stockage de texte. La valeur par défaut est`nul` , ce qui signifie que les textes des documents ne sont pas stockés.

```csharp
public TextStorageSettings TextStorageSettings { get; set; }
```

### Valeur de la propriété

Les paramètres de stockage de texte.

### Exemples

L'exemple montre comment définir les paramètres de stockage de texte.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

// Création d'une instance de paramètres d'index
IndexSettings settings = new IndexSettings();
settings.TextStorageSettings = new TextStorageSettings(Compression.High); // Définition d'un niveau de compression élevé pour le stockage de texte d'index

// Création d'un index dans le dossier spécifié
Index index = new Index(indexFolder, settings);

// Indexation des documents
index.Add(documentsFolder);

// Recherche
SearchResult result = index.Search("Einstein");
```

### Voir également

* class [TextStorageSettings](../../../groupdocs.search.options/textstoragesettings)
* class [IndexSettings](../../indexsettings)
* espace de noms [GroupDocs.Search](../../indexsettings)
* Assemblée [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->