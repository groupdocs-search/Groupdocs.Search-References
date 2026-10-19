---
title: "CreateRenameNotification"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Crea un oggetto di notifica per rinominare un documento indicizzato che è stato rinominato e non necessita di essere reindicizzato. Il documento rinominato non verrà reindicizzato durante la prossima operazione di aggiornamento anche se il suo contenuto è stato modificato."
type: docs
weight: 10
url: /it/net/groupdocs.search.common/notification/createrenamenotification/
---
## Notification.CreateRenameNotification method

Crea un oggetto di notifica per rinominare un documento indicizzato che è stato rinominato e non necessita di essere reindicizzato. Il documento rinominato non verrà reindicizzato durante la prossima operazione di aggiornamento, anche se il suo contenuto è stato modificato.

```csharp
public static Notification CreateRenameNotification(string oldPath, string newPath)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| oldPath | String | Il vecchio percorso del documento indicizzato. |
| newPath | String | Il nuovo percorso del documento indicizzato. |

### Valore di ritorno

Un nuovo oggetto di notifica di rinomina.

### Vedi anche

* class [Notification](../../notification)
* namespace [GroupDocs.Search.Common](../../../groupdocs.search.common)
* assembly [GroupDocs.Search](../../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
