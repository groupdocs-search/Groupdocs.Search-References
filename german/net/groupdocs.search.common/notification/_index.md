---
title: "Notification"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Die Basisklasse für alle Benachrichtigungen an den Index. Diese Klasse enthält außerdem Methoden zum Erstellen von Benachrichtigungsobjekten."
type: docs
weight: 260
url: /de/net/groupdocs.search.common/notification/
---
## Notification class

Die Basisklasse für alle Benachrichtigungen an den Index. Diese Klasse enthält außerdem Methoden zum Erstellen von Benachrichtigungsobjekten.

```csharp
public abstract class Notification
```

## Methoden

| Name | Beschreibung |
| --- | --- |
| static [CreateRenameNotification](../../groupdocs.search.common/notification/createrenamenotification)(string, string) | Erstellt ein Benachrichtigungsobjekt, um ein indiziertes Dokument umzubenennen, das bereits umbenannt wurde und nicht erneut indiziert werden muss. Das umbenannte Dokument wird während des nächsten Aktualisierungsvorgangs nicht erneut indiziert, selbst wenn sein Inhalt geändert wurde. |

### Hinweise

**Learn more**

* [Document renaming](https://docs.groupdocs.com/display/searchnet/Document+renaming)

### Siehe auch

* namespace [GroupDocs.Search.Common](../../groupdocs.search.common)
* assembly [GroupDocs.Search](../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
