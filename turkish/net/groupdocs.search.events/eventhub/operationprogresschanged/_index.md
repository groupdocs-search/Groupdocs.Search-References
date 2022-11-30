---
title: OperationProgressChanged
second_title: .NET API Başvurusu için GroupDocs.Search
description: İndeksleme veya güncelleme işleminin ilerlemesi değiştiğinde gerçekleşir.
type: docs
weight: 50
url: /tr/net/groupdocs.search.events/eventhub/operationprogresschanged/
---
## EventHub.OperationProgressChanged event

İndeksleme veya güncelleme işleminin ilerlemesi değiştiğinde gerçekleşir.

```csharp
public event EventHandler<OperationProgressEventArgs> OperationProgressChanged;
```

### Örnekler

Örnek, olayın nasıl kullanılacağını gösterir.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

// Bir dizin oluşturma
Index index = new Index(indexFolder);

// Etkinliğe abone oluyoruz
index.Events.OperationProgressChanged += (sender, args) =>
{
    Console.WriteLine("Last processed: " + args.LastDocumentPath);
    Console.WriteLine("Result: " + args.LastDocumentStatus);
    Console.WriteLine("Processed documents: " + args.TotalDocuments);
    Console.WriteLine("Progress percentage: " + args.ProgressPercentage);
};

// Belgeleri belirtilen klasörden indeksleme
index.Add(documentsFolder);
```

### Ayrıca bakınız

* class [OperationProgressEventArgs](../../operationprogresseventargs)
* class [EventHub](../../eventhub)
* ad alanı [GroupDocs.Search.Events](../../eventhub)
* toplantı [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->