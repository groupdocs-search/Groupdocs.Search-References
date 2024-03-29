---
title: DateFormat
second_title: GroupDocs. ابحث عن مرجع .NET API
description: يمثل تنسيق التاريخ .
type: docs
weight: 770
url: /ar/net/groupdocs.search.options/dateformat/
---
## DateFormat class

يمثل تنسيق التاريخ .

```csharp
public class DateFormat
```

## المنشئون

| اسم | وصف |
| --- | --- |
| [DateFormat](dateformat#constructor)(DateFormatElement[], string) | يقوم بتهيئة مثيل جديد لملف[`DateFormat`](../dateformat) فئة . |
| [DateFormat](dateformat#constructor_1)(string, DateFormatElement[]) | يقوم بتهيئة مثيل جديد لملف[`DateFormat`](../dateformat) فئة . |

## الخصائص

| اسم | وصف |
| --- | --- |
| [DateSeparator](../../groupdocs.search.options/dateformat/dateseparator) { get; } | يحصل على فاصل التاريخ . |

## طُرق

| اسم | وصف |
| --- | --- |
| override [ToString](../../groupdocs.search.options/dateformat/tostring)() | إرجاع أString التي تمثل التيار[`DateFormat`](../dateformat) . |

### ملاحظات

**يتعلم أكثر**

* [البحث في النطاق الزمني](https://docs.groupdocs.com/display/searchnet/Date+range+search)

### أمثلة

يوضح المثال استخدامًا نموذجيًا للفئة.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "daterange(2017-01-01 ~~ 2019-12-31)";

Index index = new Index(indexFolder); // إنشاء فهرس في المجلد المحدد
index.Add(documentsFolder); // فهرسة المستندات من المجلد المحدد

SearchOptions options = new SearchOptions();
options.DateFormats.Clear(); // إزالة تنسيقات التاريخ الافتراضية
DateFormatElement[] elements = new DateFormatElement[]
{
    DateFormatElement.MonthTwoDigits,
    DateFormatElement.DateSeparator,
    DateFormatElement.DayOfMonthTwoDigits,
    DateFormatElement.DateSeparator,
    DateFormatElement.YearFourDigits,
};
// إنشاء نمط تنسيق التاريخ "MM / dd / yyyy"
DateFormat dateFormat = new DateFormat(elements, "/");
options.DateFormats.Add(dateFormat);

SearchResult result = index.Search(query, options); // بحث في الفهرس
```

### أنظر أيضا

* مساحة الاسم [GroupDocs.Search.Options](../../groupdocs.search.options)
* المجسم [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
