---
title: GetIndexingReports
second_title: GroupDocs. ابحث عن مرجع .NET API
description: الحصول على تقارير حول عمليات الفهرسة .
type: docs
weight: 160
url: /ar/net/groupdocs.search/index/getindexingreports/
---
## Index.GetIndexingReports method

الحصول على تقارير حول عمليات الفهرسة .

```csharp
public IndexingReport[] GetIndexingReports()
```

### قيمة الإرجاع

تقارير الفهرسة.

### أمثلة

يوضح المثال كيفية الحصول على تقارير الفهرسة.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // إنشاء الفهرس في المجلد المحدد
index.Add(documentsFolder); // فهرسة المستندات من المجلد المحدد

IndexingReport[] reports = index.GetIndexingReports(); // الحصول على تقارير الفهرسة
```

### أنظر أيضا

* class [IndexingReport](../../../groupdocs.search.common/indexingreport)
* class [Index](../../index)
* مساحة الاسم [GroupDocs.Search](../../index)
* المجسم [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->