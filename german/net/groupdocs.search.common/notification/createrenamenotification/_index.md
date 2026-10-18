---
title: "CreateRenameNotification"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Erstellt ein Benachrichtigungsobjekt, um ein indiziertes Dokument umzubenennen, das bereits umbenannt wurde und nicht erneut indiziert werden muss. Das umbenannte Dokument wird bei der nächsten Aktualisierungsoperation nicht erneut indiziert, selbst wenn sein Inhalt geändert wurde."
type: docs
weight: 10
url: /de/net/groupdocs.search.common/notification/createrenamenotification/
---
## Notification.CreateRenameNotification method

Erstellt ein Benachrichtigungsobjekt, um ein indiziertes Dokument umzubenennen, das bereits umbenannt wurde und nicht erneut indiziert werden muss. Das umbenannte Dokument wird während des nächsten Aktualisierungsvorgangs nicht erneut indiziert, selbst wenn sein Inhalt geändert wurde.

```csharp
public static Notification CreateRenameNotification(string oldPath, string newPath)
```

| Parameter | Type | Beschreibung |
| --- | --- | --- |
| oldPath | String | Der alte Pfad zum indizierten Dokument. |
| newPath | String | Der neue Pfad zum indizierten Dokument. |

### Rückgabewert

Ein neues Umbenennungsbenachrichtigungsobjekt.

### Siehe auch

* class [Notification](../../notification)
* namespace [GroupDocs.Search.Common](../../../groupdocs.search.common)
* assembly [GroupDocs.Search](../../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
