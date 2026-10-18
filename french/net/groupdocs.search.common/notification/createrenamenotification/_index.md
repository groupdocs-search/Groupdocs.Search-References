---
title: "CreateRenameNotification"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Crée un objet de notification pour renommer un document indexé qui a été renommé et qui n'a pas besoin d'être réindexé. Le document renommé ne sera pas réindexé lors de la prochaine opération de mise à jour même si son contenu a été modifié."
type: docs
weight: 10
url: /fr/net/groupdocs.search.common/notification/createrenamenotification/
---
## Notification.CreateRenameNotification method

Crée un objet de notification pour renommer un document indexé qui a été renommé et qui n'a pas besoin d'être réindexé. Le document renommé ne sera pas réindexé lors de la prochaine opération de mise à jour, même si son contenu a été modifié.

```csharp
public static Notification CreateRenameNotification(string oldPath, string newPath)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| oldPath | String | L'ancien chemin du document indexé. |
| newPath | String | Le nouveau chemin du document indexé. |

### Valeur de retour

Un nouvel objet de notification de renommage.

### Voir aussi

* class [Notification](../../notification)
* namespace [GroupDocs.Search.Common](../../../groupdocs.search.common)
* assembly [GroupDocs.Search](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
