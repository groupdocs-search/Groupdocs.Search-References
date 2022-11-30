---
title: FileIndexingEventArgs
second_title: GroupDocs. ابحث عن مرجع .NET API
description: يمثل وسيطات لحدث بدء فهرسة المستند.
type: docs
weight: 510
url: /ar/net/groupdocs.search.events/fileindexingeventargs/
---
## FileIndexingEventArgs class

يمثل وسيطات لحدث بدء فهرسة المستند.

```csharp
public class FileIndexingEventArgs : BaseIndexEventArgs
```

## الخصائص

| اسم | وصف |
| --- | --- |
| [AdditionalFields](../../groupdocs.search.events/fileindexingeventargs/additionalfields) { get; set; } | الحصول على أو تعيين الحقول الإضافية للمستند. |
| [Attributes](../../groupdocs.search.events/fileindexingeventargs/attributes) { get; set; } | الحصول على سمات المستند أو تعيينها. |
| [CustomExtractor](../../groupdocs.search.events/fileindexingeventargs/customextractor) { get; set; } | الحصول على أو تعيين مستخرج النص المخصص. |
| [Document](../../groupdocs.search.events/fileindexingeventargs/document) { get; } | يحصل على المستند . |
| [DocumentFullPath](../../groupdocs.search.events/fileindexingeventargs/documentfullpath) { get; } | يحصل على المسار الكامل للمستند . |
| [DocumentKey](../../groupdocs.search.events/fileindexingeventargs/documentkey) { get; } | يحصل على مفتاح المستند. |
| [Encoding](../../groupdocs.search.events/fileindexingeventargs/encoding) { get; set; } | الحصول على أو تعيين ترميز المستند. |
| [IndexFolder](../../groupdocs.search.events/baseindexeventargs/indexfolder) { get; } | يحصل على مجلد الفهرس. |
| [IndexId](../../groupdocs.search.events/baseindexeventargs/indexid) { get; } | يحصل على معرف الفهرس . |
| [SkipIndexing](../../groupdocs.search.events/fileindexingeventargs/skipindexing) { get; set; } | الحصول على أو تعيين قيمة تشير إلى ضرورة تخطي فهرسة المستند. |
| [Status](../../groupdocs.search.events/baseindexeventargs/status) { get; } | يحصل على حالة الفهرس . |
| [Time](../../groupdocs.search.events/baseindexeventargs/time) { get; } | الحصول على وقت الحدث . |

### ملاحظات

**يتعلم أكثر**

* [أحداث فهرس البحث](https://docs.groupdocs.com/display/searchnet/Search+index+events)

### أنظر أيضا

* class [BaseIndexEventArgs](../baseindexeventargs)
* مساحة الاسم [GroupDocs.Search.Events](../../groupdocs.search.events)
* المجسم [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->