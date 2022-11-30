---
title: DocumentFilter
second_title: GroupDocs. ابحث عن مرجع .NET API
description: الحصول على أو تعيين عامل تصفية المستندDocumentFiltergroupdocs.search/indexsettings/documentfilter يعمل على منطق التضمين. استخدم ملفDocumentFiltergroupdocs.search.options/documentfilter فئة لإنشاء مثيلات مرشح المستند . القيمة الافتراضية هيلا شيء  مما يعني أنه تتم فهرسة جميع المستندات المضافة.
type: docs
weight: 40
url: /ar/net/groupdocs.search/indexsettings/documentfilter/
---
## IndexSettings.DocumentFilter property

الحصول على أو تعيين عامل تصفية المستند`DocumentFilter` يعمل على منطق التضمين. استخدم ملف[`DocumentFilter`](../../../groupdocs.search.options/documentfilter) فئة لإنشاء مثيلات مرشح المستند . القيمة الافتراضية هي`لا شيء` ، مما يعني أنه تتم فهرسة جميع المستندات المضافة.

```csharp
public DocumentFilter DocumentFilter { get; set; }
```

### Property_Value

مرشح الوثيقة.

### أمثلة

يوضح المثال كيفية تعيين مرشح المستند.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

// إنشاء عامل تصفية يتخطى المستندات ذات الامتدادات ".doc" ، ".docx" ، ".rtf"
IndexSettings settings = new IndexSettings();
DocumentFilter fileExtensionFilter = DocumentFilter.CreateFileExtension(".doc", ".docx", ".rtf"); // إنشاء مرشح امتداد الملف
DocumentFilter invertedFilter = DocumentFilter.CreateNot(fileExtensionFilter); // عكس مرشح امتداد الملف
settings.DocumentFilter = invertedFilter;

// إنشاء فهرس في المجلد المحدد
Index index = new Index(indexFolder, settings);

// فهرسة الوثائق
index.Add(documentsFolder);

// يبحث
SearchResult result = index.Search("Einstein");
```

### أنظر أيضا

* class [DocumentFilter](../../../groupdocs.search.options/documentfilter)
* class [IndexSettings](../../indexsettings)
* مساحة الاسم [GroupDocs.Search](../../indexsettings)
* المجسم [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->