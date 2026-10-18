---
title: "TextStorageSettings"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Obtient ou définit les paramètres de stockage du texte. La valeur par défaut est null, ce qui signifie que les textes des documents ne sont pas stockés."
type: docs
weight: 100
url: /fr/net/groupdocs.search/indexsettings/textstoragesettings/
---
## IndexSettings.TextStorageSettings property

Obtient ou définit les paramètres de stockage du texte. La valeur par défaut est `null`, ce qui signifie que les textes des documents ne sont pas stockés.

```csharp
public TextStorageSettings TextStorageSettings { get; set; }
```

### Property Value

Les paramètres de stockage du texte.

### Exemples

L'exemple montre comment définir les paramètres de stockage du texte.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

// Création d'une instance de paramètres d'index
IndexSettings settings = new IndexSettings();
settings.TextStorageSettings = new TextStorageSettings(Compression.High); // Setting high compression level for the index text storage

// Création d'un index dans le dossier spécifié
Index index = new Index(indexFolder, settings);

// Indexation des documents
index.Add(documentsFolder);

// Recherche
SearchResult result = index.Search("Einstein");
```

### Voir aussi

* class [TextStorageSettings](../../../groupdocs.search.options/textstoragesettings)
* class [IndexSettings](../../indexsettings)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
