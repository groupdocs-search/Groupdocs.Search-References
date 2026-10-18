---
title: "Notification"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "La classe de base pour toutes les notifications à l'index. Cette classe contient également des méthodes pour créer des objets de notification."
type: docs
weight: 260
url: /fr/net/groupdocs.search.common/notification/
---
## Notification class

La classe de base pour toutes les notifications à l'index. Cette classe contient également des méthodes pour créer des objets de notification.

```csharp
public abstract class Notification
```

## Méthodes

| Nom | Description |
| --- | --- |
| static [CreateRenameNotification](../../groupdocs.search.common/notification/createrenamenotification)(string, string) | Crée un objet de notification pour renommer un document indexé qui a été renommé et qui n'a pas besoin d'être réindexé. Le document renommé ne sera pas réindexé lors de la prochaine opération de mise à jour, même si son contenu a été modifié. |

### Remarques

**Learn more**

* [Document renaming](https://docs.groupdocs.com/display/searchnet/Document+renaming)

### Voir aussi

* namespace [GroupDocs.Search.Common](../../groupdocs.search.common)
* assembly [GroupDocs.Search](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
