---
title: "StatusChanged"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Se produit lorsque l'état de l'index change."
type: docs
weight: 90
url: /fr/net/groupdocs.search.events/eventhub/statuschanged/
---
## EventHub.StatusChanged event

Se produit lorsque l'état de l'index change.

```csharp
public event EventHandler<BaseIndexEventArgs> StatusChanged;
```

### Exemples

L'exemple montre comment utiliser l'événement.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

// Création d'un index
Index index = new Index(indexFolder);

// S'abonner à l'événement
index.Events.StatusChanged += (sender, args) =>
{
    if (args.Status != IndexStatus.InProgress)
    {
        // Une notification de la fin de l'opération devrait être ici
    }
};

// Définir le drapeau pour l'indexation asynchrone
IndexingOptions options = new IndexingOptions();
options.IsAsync = true;

// Indexation asynchrone des documents depuis le dossier spécifié
// La méthode se termine avant que l'opération ne soit terminée
index.Add(documentsFolder, options);
```

### Voir aussi

* class [BaseIndexEventArgs](../../baseindexeventargs)
* class [EventHub](../../eventhub)
* namespace [GroupDocs.Search.Events](../../../groupdocs.search.events)
* assembly [GroupDocs.Search](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
