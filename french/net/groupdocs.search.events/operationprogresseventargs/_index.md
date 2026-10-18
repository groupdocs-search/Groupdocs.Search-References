---
title: "OperationProgressEventArgs"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Représente les arguments de l'événement de changement de progression de l'opération d'indexation."
type: docs
weight: 580
url: /fr/net/groupdocs.search.events/operationprogresseventargs/
---
## OperationProgressEventArgs class

Représente les arguments de l'événement de changement de progression de l'opération d'indexation.

```csharp
public class OperationProgressEventArgs : BaseIndexEventArgs
```

## Propriétés

| Nom | Description |
| --- | --- |
| [IndexFolder](../../groupdocs.search.events/baseindexeventargs/indexfolder) { get; } | Obtient le dossier d'index. |
| [IndexId](../../groupdocs.search.events/baseindexeventargs/indexid) { get; } | Obtient l'ID de l'index. |
| [LastDocumentKey](../../groupdocs.search.events/operationprogresseventargs/lastdocumentkey) { get; } | Obtient la clé du dernier document traité. |
| [LastDocumentPath](../../groupdocs.search.events/operationprogresseventargs/lastdocumentpath) { get; } | Obtient le chemin du dernier document traité. |
| [LastDocumentStatus](../../groupdocs.search.events/operationprogresseventargs/lastdocumentstatus) { get; } | Obtient l'état du dernier document traité. |
| [ProcessedDocuments](../../groupdocs.search.events/operationprogresseventargs/processeddocuments) { get; } | Obtient le nombre de documents traités avec succès. |
| [ProgressPercentage](../../groupdocs.search.events/operationprogresseventargs/progresspercentage) { get; } | Obtient le pourcentage de la progression. |
| [SkippedDocuments](../../groupdocs.search.events/operationprogresseventargs/skippeddocuments) { get; } | Obtient le nombre de documents ignorés. |
| [Status](../../groupdocs.search.events/baseindexeventargs/status) { get; } | Obtient le statut de l'index. |
| [Time](../../groupdocs.search.events/baseindexeventargs/time) { get; } | Obtient le moment d'un événement. |
| [TotalDocuments](../../groupdocs.search.events/operationprogresseventargs/totaldocuments) { get; } | Obtient le nombre total de documents à traiter. |

### Remarques

**Learn more**

* [Search index events](https://docs.groupdocs.com/display/searchnet/Search+index+events)

### Voir aussi

* class [BaseIndexEventArgs](../baseindexeventargs)
* namespace [GroupDocs.Search.Events](../../groupdocs.search.events)
* assembly [GroupDocs.Search](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
