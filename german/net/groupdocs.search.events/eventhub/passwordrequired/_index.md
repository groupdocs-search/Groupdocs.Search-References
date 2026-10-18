---
title: "PasswordRequired"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Tritt auf, wenn ein Dokument ein Passwort zum Öffnen benötigt."
type: docs
weight: 70
url: /de/net/groupdocs.search.events/eventhub/passwordrequired/
---
## EventHub.PasswordRequired event

Tritt auf, wenn ein Dokument ein Passwort zum Öffnen benötigt.

```csharp
public event EventHandler<PasswordRequiredEventArgs> PasswordRequired;
```

### Beispiele

Das Beispiel zeigt, wie das Ereignis verwendet wird.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

// Erstellen eines Index
Index index = new Index(indexFolder);

// Abonnieren des Ereignisses
index.Events.PasswordRequired += (sender, args) =>
{
    if (args.DocumentFullPath.EndsWith("ProtectedDocument.pdf", StringComparison.InvariantCultureIgnoreCase))
    {
        args.Password = "123456";
    }
};

// Indizierung von Dokumenten aus dem angegebenen Ordner
index.Add(documentsFolder);
```

### Siehe auch

* class [PasswordRequiredEventArgs](../../passwordrequiredeventargs)
* class [EventHub](../../eventhub)
* namespace [GroupDocs.Search.Events](../../../groupdocs.search.events)
* assembly [GroupDocs.Search](../../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
