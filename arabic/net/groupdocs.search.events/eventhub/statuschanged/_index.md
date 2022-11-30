---
title: StatusChanged
second_title: GroupDocs. ابحث عن مرجع .NET API
description: يحدث عندما تتغير حالة الفهرس .
type: docs
weight: 80
url: /ar/net/groupdocs.search.events/eventhub/statuschanged/
---
## EventHub.StatusChanged event

يحدث عندما تتغير حالة الفهرس .

```csharp
public event EventHandler<BaseIndexEventArgs> StatusChanged;
```

### أمثلة

يوضح المثال كيفية استخدام الحدث.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

// إنشاء فهرس
Index index = new Index(indexFolder);

// الاشتراك في الحدث
index.Events.StatusChanged += (sender, args) =>
{
    if (args.Status != IndexStatus.InProgress)
    {
        // يجب أن يكون هنا إشعار بإتمام العملية
    }
};

// تعيين علامة الفهرسة غير المتزامنة
IndexingOptions options = new IndexingOptions();
options.IsAsync = true;

// وثائق فهرسة غير متزامنة من المجلد المحدد
// الطريقة تنتهي قبل اكتمال العملية
index.Add(documentsFolder, options);
```

### أنظر أيضا

* class [BaseIndexEventArgs](../../baseindexeventargs)
* class [EventHub](../../eventhub)
* مساحة الاسم [GroupDocs.Search.Events](../../eventhub)
* المجسم [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->