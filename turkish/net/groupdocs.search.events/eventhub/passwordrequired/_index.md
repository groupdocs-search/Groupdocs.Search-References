---
title: PasswordRequired
second_title: .NET API Başvurusu için GroupDocs.Search
description: Bir belge açmak için parola gerektirdiğinde oluşur.
type: docs
weight: 60
url: /tr/net/groupdocs.search.events/eventhub/passwordrequired/
---
## EventHub.PasswordRequired event

Bir belge açmak için parola gerektirdiğinde oluşur.

```csharp
public event EventHandler<PasswordRequiredEventArgs> PasswordRequired;
```

### Örnekler

Örnek, olayın nasıl kullanılacağını gösterir.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

// Bir dizin oluşturma
Index index = new Index(indexFolder);

// Etkinliğe abone oluyoruz
index.Events.PasswordRequired += (sender, args) =>
{
    if (args.DocumentFullPath.EndsWith("ProtectedDocument.pdf", StringComparison.InvariantCultureIgnoreCase))
    {
        args.Password = "123456";
    }
};

// Belgeleri belirtilen klasörden indeksleme
index.Add(documentsFolder);
```

### Ayrıca bakınız

* class [PasswordRequiredEventArgs](../../passwordrequiredeventargs)
* class [EventHub](../../eventhub)
* ad alanı [GroupDocs.Search.Events](../../eventhub)
* toplantı [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->