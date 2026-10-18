---
title: "IndexErrorEventArgs"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Représente les arguments de l'événement d'une erreur d'index survenue."
type: docs
weight: 560
url: /fr/net/groupdocs.search.events/indexerroreventargs/
---
## IndexErrorEventArgs class

Représente les arguments de l'événement d'une erreur d'index survenue.

```csharp
public class IndexErrorEventArgs : BaseIndexEventArgs
```

## Propriétés

| Nom | Description |
| --- | --- |
| [IndexFolder](../../groupdocs.search.events/baseindexeventargs/indexfolder) { get; } | Obtient le dossier d'index. |
| [IndexId](../../groupdocs.search.events/baseindexeventargs/indexid) { get; } | Obtient l'ID de l'index. |
| [IsCritical](../../groupdocs.search.events/indexerroreventargs/iscritical) { get; } | Obtient un indicateur indiquant que l'erreur survenue est critique et que l'index doit être redémarré. |
| [Message](../../groupdocs.search.events/indexerroreventargs/message) { get; } | Obtient le message d'erreur. |
| [Status](../../groupdocs.search.events/baseindexeventargs/status) { get; } | Obtient le statut de l'index. |
| [Time](../../groupdocs.search.events/baseindexeventargs/time) { get; } | Obtient le moment d'un événement. |

### Remarques

**Learn more**

* [Search index events](https://docs.groupdocs.com/display/searchnet/Search+index+events)

### Voir aussi

* class [BaseIndexEventArgs](../baseindexeventargs)
* namespace [GroupDocs.Search.Events](../../groupdocs.search.events)
* assembly [GroupDocs.Search](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
