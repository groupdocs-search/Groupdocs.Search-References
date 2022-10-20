---
title: FileIndexing
second_title: GroupDocs.Search для справочника API .NET
description: Происходит когда документ будет проиндексирован.
type: docs
weight: 20
url: /ru/net/groupdocs.search.events/eventhub/fileindexing/
---
## EventHub.FileIndexing event

Происходит, когда документ будет проиндексирован.

```csharp
public event EventHandler<FileIndexingEventArgs> FileIndexing;
```

### Примеры

В примере показано, как использовать событие.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

// Создание индекса
Index index = new Index(indexFolder);

// Подписка на событие
index.Events.FileIndexing += (sender, args) =>
{
    if (args.DocumentFullPath.EndsWith("Protected.pdf", StringComparison.InvariantCultureIgnoreCase))
    {
        args.AdditionalFields = new DocumentField[]
        {
            new DocumentField("Tags", "Protected")
        };
    }
    if (!args.DocumentFullPath.ToLowerInvariant().Contains("important"))
    {
        args.SkipIndexing = true;
    }
};

// Индексация документов из указанной папки
index.Add(documentsFolder);
```

### Смотрите также

* class [FileIndexingEventArgs](../../fileindexingeventargs)
* class [EventHub](../../eventhub)
* пространство имен [GroupDocs.Search.Events](../../eventhub)
* сборка [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->