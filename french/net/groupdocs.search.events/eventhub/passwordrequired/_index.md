---
title: "PasswordRequired"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Se produit lorsqu'un document nécessite un mot de passe pour être ouvert."
type: docs
weight: 70
url: /fr/net/groupdocs.search.events/eventhub/passwordrequired/
---
## EventHub.PasswordRequired event

Se produit lorsqu'un document nécessite un mot de passe pour être ouvert.

```csharp
public event EventHandler<PasswordRequiredEventArgs> PasswordRequired;
```

### Exemples

L'exemple montre comment utiliser l'événement.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

// Création d'un index
Index index = new Index(indexFolder);

// S'abonner à l'événement
index.Events.PasswordRequired += (sender, args) =>
{
    if (args.DocumentFullPath.EndsWith("ProtectedDocument.pdf", StringComparison.InvariantCultureIgnoreCase))
    {
        args.Password = "123456";
    }
};

// Indexation des documents depuis le dossier spécifié
index.Add(documentsFolder);
```

### Voir aussi

* class [PasswordRequiredEventArgs](../../passwordrequiredeventargs)
* class [EventHub](../../eventhub)
* namespace [GroupDocs.Search.Events](../../../groupdocs.search.events)
* assembly [GroupDocs.Search](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
