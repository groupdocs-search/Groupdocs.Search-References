---
title: "PasswordRequiredEventArgs"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Représente les arguments de l'événement qui se produit lorsqu'un document protégé par un mot de passe est indexé."
type: docs
weight: 610
url: /fr/net/groupdocs.search.events/passwordrequiredeventargs/
---
## PasswordRequiredEventArgs class

Représente les arguments de l'événement qui se produit lorsqu'un document protégé par un mot de passe est indexé.

```csharp
public class PasswordRequiredEventArgs : BaseIndexEventArgs
```

## Propriétés

| Nom | Description |
| --- | --- |
| [DocumentFullPath](../../groupdocs.search.events/passwordrequiredeventargs/documentfullpath) { get; } | Obtient le chemin complet du document. |
| [IndexFolder](../../groupdocs.search.events/baseindexeventargs/indexfolder) { get; } | Obtient le dossier d'index. |
| [IndexId](../../groupdocs.search.events/baseindexeventargs/indexid) { get; } | Obtient l'ID de l'index. |
| [Password](../../groupdocs.search.events/passwordrequiredeventargs/password) { get; set; } | Obtient ou définit le mot de passe pour ouvrir le document. |
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
