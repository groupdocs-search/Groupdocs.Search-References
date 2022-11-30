---
title: Remove
second_title: GroupDocs. ابحث عن مرجع .NET API
description: يزيل الاسم المستعار المحدد من ملفAliasDictionarygroupdocs.search.dictionaries/aliasdictionary الكائن .
type: docs
weight: 80
url: /ar/net/groupdocs.search.dictionaries/aliasdictionary/remove/
---
## AliasDictionary.Remove method

يزيل الاسم المستعار المحدد من ملف[`AliasDictionary`](../../aliasdictionary) الكائن .

```csharp
public bool Remove(string alias)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| alias | String | الاسم المستعار المطلوب إزالته. |

### قيمة الإرجاع

هذه الطريقة ترجع`حقيقي` إذا تم العثور على الاسم المستعار وإزالته بنجاح. هذه الطريقة ترجع`خاطئة` إذا لم يتم العثور على الاسم المستعار في ملف[`AliasDictionary`](../../aliasdictionary) الكائن .

### استثناءات

| استثناء | حالة |
| --- | --- |
| ArgumentNullException | عندما ألقيت*alias* هو`لا شيء`. |

### أنظر أيضا

* class [AliasDictionary](../../aliasdictionary)
* مساحة الاسم [GroupDocs.Search.Dictionaries](../../aliasdictionary)
* المجسم [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->