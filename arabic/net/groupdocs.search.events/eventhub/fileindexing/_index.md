---
title: FileIndexing
second_title: GroupDocs. ابحث عن مرجع .NET API
description: يحدث عند فهرسة مستند.
type: docs
weight: 20
url: /ar/net/groupdocs.search.events/eventhub/fileindexing/
---
## EventHub.FileIndexing event

يحدث عند فهرسة مستند.

```csharp
public event EventHandler<FileIndexingEventArgs> FileIndexing;
```

### أمثلة

يوضح المثال كيفية استخدام الحدث.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

// إنشاء فهرس
Index index = new Index(indexFolder);

// الاشتراك في الحدث
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

// فهرسة المستندات من المجلد المحدد
index.Add(documentsFolder);
```

### أنظر أيضا

* class [FileIndexingEventArgs](../../fileindexingeventargs)
* class [EventHub](../../eventhub)
* مساحة الاسم [GroupDocs.Search.Events](../../eventhub)
* المجسم [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->