---
title: "EventHub"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Fournit des événements d'index pour s'abonner."
type: docs
weight: 530
url: /fr/net/groupdocs.search.events/eventhub/
---
## EventHub class

Fournit des événements d'index pour s'abonner.

```csharp
public class EventHub
```

## Événements

| Nom | Description |
| --- | --- |
| event [ErrorOccurred](../../groupdocs.search.events/eventhub/erroroccurred) | Se produit lorsqu'une erreur survient lors d'une opération d'index. |
| event [FileIndexing](../../groupdocs.search.events/eventhub/fileindexing) | Se produit lorsqu'un document va être indexé. |
| event [ImagePreparing](../../groupdocs.search.events/eventhub/imagepreparing) | Se produit lorsqu'une image va être préparée pour l'indexation. |
| event [OperationFinished](../../groupdocs.search.events/eventhub/operationfinished) | Se produit lorsqu'une opération d'index est terminée. |
| event [OperationProgressChanged](../../groupdocs.search.events/eventhub/operationprogresschanged) | Se produit lorsque la progression de l'indexation ou de la mise à jour change. |
| event [OptimizationProgressChanged](../../groupdocs.search.events/eventhub/optimizationprogresschanged) | Se produit lorsque la progression de l'opération d'optimisation change. |
| event [PasswordRequired](../../groupdocs.search.events/eventhub/passwordrequired) | Se produit lorsqu'un document nécessite un mot de passe pour être ouvert. |
| event [SearchPhaseCompleted](../../groupdocs.search.events/eventhub/searchphasecompleted) | Se produit lorsque la phase de recherche est terminée. |
| event [StatusChanged](../../groupdocs.search.events/eventhub/statuschanged) | Se produit lorsque l'état de l'index change. |

### Remarques

**Learn more**

* [Search index events](https://docs.groupdocs.com/display/searchnet/Search+index+events)

### Exemples

L'exemple montre une utilisation typique de l'interface.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

// Création d'un index
Index index = new Index(indexFolder);

// S'abonner à l'événement
index.Events.ErrorOccurred += (sender, args) =>
{
    Console.WriteLine(args.Message);
};

// Indexation des documents depuis le dossier spécifié
index.Add(documentsFolder);

// Recherche dans l'index
SearchResult result = index.Search(query);
```

### Voir aussi

* namespace [GroupDocs.Search.Events](../../groupdocs.search.events)
* assembly [GroupDocs.Search](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
