---
title: TextStorageSettings
second_title: GroupDocs. ابحث عن مرجع .NET API
description: الحصول على أو تعيين إعدادات تخزين النص . القيمة الافتراضية هيباطل  مما يعني أنه لا يتم تخزين نصوص المستند.
type: docs
weight: 110
url: /ar/net/groupdocs.search/indexsettings/textstoragesettings/
---
## IndexSettings.TextStorageSettings property

الحصول على أو تعيين إعدادات تخزين النص . القيمة الافتراضية هي`باطل` ، مما يعني أنه لا يتم تخزين نصوص المستند.

```csharp
public TextStorageSettings TextStorageSettings { get; set; }
```

### Property_Value

إعدادات تخزين النص.

### أمثلة

يوضح المثال كيفية تعيين إعدادات تخزين النص.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

// إنشاء مثيل إعدادات الفهرس
IndexSettings settings = new IndexSettings();
settings.TextStorageSettings = new TextStorageSettings(Compression.High); // تعيين مستوى ضغط عالٍ لتخزين نص الفهرس

// إنشاء فهرس في المجلد المحدد
Index index = new Index(indexFolder, settings);

// فهرسة الوثائق
index.Add(documentsFolder);

// يبحث
SearchResult result = index.Search("Einstein");
```

### أنظر أيضا

* class [TextStorageSettings](../../../groupdocs.search.options/textstoragesettings)
* class [IndexSettings](../../indexsettings)
* مساحة الاسم [GroupDocs.Search](../../indexsettings)
* المجسم [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
