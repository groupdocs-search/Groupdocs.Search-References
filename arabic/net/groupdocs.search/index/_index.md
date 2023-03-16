---
title: Index
second_title: GroupDocs. ابحث عن مرجع .NET API
description: يمثل الفئة الرئيسية لفهرسة المستندات والبحث فيها.
type: docs
weight: 680
url: /ar/net/groupdocs.search/index/
---
## Index class

يمثل الفئة الرئيسية لفهرسة المستندات والبحث فيها.

```csharp
public class Index : IDisposable
```

## المنشئون

| اسم | وصف |
| --- | --- |
| [Index](index#constructor)() | يقوم بتهيئة مثيل جديد لملف[`Index`](../index) فئة في الذاكرة. |
| [Index](index#constructor_1)(IndexSettings) | يقوم بتهيئة مثيل جديد لملف[`Index`](../index) فئة في الذاكرة مع إعدادات فهرس معينة. |
| [Index](index#constructor_2)(string) | يقوم بتهيئة مثيل جديد لملف[`Index`](../index) class. إنشاء فهرس جديد أو فتح فهرس موجود على القرص. |
| [Index](index#constructor_3)(string, bool) | يقوم بتهيئة مثيل جديد لملف[`Index`](../index) class. تحميل فهرس موجود من القرص إذا*overwriteIfExists* يكون`خطأ شنيع`؛ ينشئ فهرسًا جديدًا على القرص وإلا. |
| [Index](index#constructor_4)(string, IndexSettings) | يقوم بتهيئة مثيل جديد لملف[`Index`](../index) class. ينشئ فهرسًا جديدًا بإعدادات معينة أو يفتح فهرسًا موجودًا على القرص. |
| [Index](index#constructor_5)(string, IndexSettings, bool) | يقوم بتهيئة مثيل جديد لملف[`Index`](../index) class. تحميل فهرس موجود من القرص إذا*overwriteIfExists* يكون`خطأ شنيع` ؛ ينشئ فهرسًا جديدًا على القرص بإعدادات فهرس معينة. |

## الخصائص

| اسم | وصف |
| --- | --- |
| [Dictionaries](../../groupdocs.search/index/dictionaries) { get; } | الحصول على مستودع القاموس . |
| [Events](../../groupdocs.search/index/events) { get; } | الحصول على مركز الحدث للاشتراك في الأحداث. |
| [IndexInfo](../../groupdocs.search/index/indexinfo) { get; } | يحصل على المعلومات الأساسية عن الفهرس. |
| [IndexSettings](../../groupdocs.search/index/indexsettings) { get; } | يحصل على إعدادات الفهرس . |
| [Repository](../../groupdocs.search/index/repository) { get; } | يحصل على كائن مستودع الفهرس إذا كان الفهرس متضمنًا فيه. |

## طُرق

| اسم | وصف |
| --- | --- |
| [Add](../../groupdocs.search/index/add#add_2)(string) | يقوم بعملية الفهرسة. يضيف ملفًا أو مجلدًا بواسطة مسار مطلق أو نسبي. ستتم فهرسة المستندات من كافة المجلدات الفرعية. |
| [Add](../../groupdocs.search/index/add#add_4)(string[]) | يقوم بعملية الفهرسة. يضيف ملفات أو مجلدات بواسطة مسار مطلق أو نسبي. ستتم فهرسة المستندات من كافة المجلدات الفرعية. |
| [Add](../../groupdocs.search/index/add#add)(Document[], IndexingOptions) | يقوم بعملية الفهرسة. يضيف المستندات من نظام الملفات أو الدفق أو الهيكل . |
| [Add](../../groupdocs.search/index/add#add_1)(ExtractedData[], IndexingOptions) | يقوم بعملية الفهرسة . يضيف البيانات المستخرجة إلى الفهرس . |
| [Add](../../groupdocs.search/index/add#add_3)(string, IndexingOptions) | يقوم بعملية الفهرسة. يضيف ملفًا أو مجلدًا بواسطة مسار مطلق أو نسبي. ستتم فهرسة المستندات من كافة المجلدات الفرعية. |
| [Add](../../groupdocs.search/index/add#add_5)(string[], IndexingOptions) | يقوم بعملية الفهرسة. يضيف ملفات أو مجلدات بواسطة مسار مطلق أو نسبي. ستتم فهرسة المستندات من كافة المجلدات الفرعية. |
| [ChangeAttributes](../../groupdocs.search/index/changeattributes)(AttributeChangeBatch) | يطبق الدفعة المحددة لتغييرات السمات على المستندات المفهرسة دون إعادة الفهرسة أثناء عملية التحديث. |
| [Delete](../../groupdocs.search/index/delete#delete_1)(string[], UpdateOptions) | حذف الملفات أو المجلدات المفهرسة من الفهرس. ثم يقوم بتحديث الفهرس بدون حذف المسارات. لاحظ أنه لا يمكن حذف مستند فردي من الفهرس إذا تمت إضافته إلى الفهرس كجزء من مجلد. |
| [Delete](../../groupdocs.search/index/delete#delete)(UpdateOptions, string[]) | حذف المستندات المفهرسة من التدفقات أو الهياكل. ثم يقوم بتحديث الفهرس بدون حذف المستندات. |
| [Dispose](../../groupdocs.search/index/dispose)() | يقوم بإصدار كافة الموارد التي يستخدمها ملف[`Index`](../index) . |
| [GetAttributes](../../groupdocs.search/index/getattributes)(string) | يحصل على جميع السمات المرتبطة بالمستند المفهرس المحدد. |
| [GetDocumentText](../../groupdocs.search/index/getdocumenttext#getdocumenttext)(DocumentInfo, OutputAdapter) | يولد نصًا بتنسيق HTML للمستند المفهرس وينقله عبر محول الإخراج. |
| [GetDocumentText](../../groupdocs.search/index/getdocumenttext#getdocumenttext_1)(DocumentInfo, OutputAdapter, TextOptions) | يولد نصًا بتنسيق HTML للمستند المفهرس وينقله عبر محول الإخراج. |
| [GetIndexedDocumentItems](../../groupdocs.search/index/getindexeddocumentitems)(DocumentInfo) | الحصول على مصفوفة من العناصر المتداخلة للمستند المحدد (لمستندات الحاوية مثل ZIP و OST و PST) . |
| [GetIndexedDocuments](../../groupdocs.search/index/getindexeddocuments)() | الحصول على مصفوفة من كافة المستندات المفهرسة . |
| [GetIndexedPaths](../../groupdocs.search/index/getindexedpaths)() | يحصل على مجموعة من المسارات المفهرسة - المستندات أو المجلدات. |
| [GetIndexingReports](../../groupdocs.search/index/getindexingreports)() | الحصول على تقارير حول عمليات الفهرسة . |
| [GetSearchReports](../../groupdocs.search/index/getsearchreports)() | الحصول على تقارير حول عمليات البحث . |
| [Highlight](../../groupdocs.search/index/highlight#highlight)(FoundDocument, Highlighter) | يولد نصًا بتنسيق HTML مع تحديد المصطلحات الموجودة. |
| [Highlight](../../groupdocs.search/index/highlight#highlight_1)(FoundDocument, Highlighter, HighlightOptions) | يولد نصًا بتنسيق HTML مع تحديد المصطلحات الموجودة. |
| [Merge](../../groupdocs.search/index/merge#merge)(Index, MergeOptions) | يدمج الفهرس المحدد في الفهرس الحالي. لاحظ أن الفهرس الآخر لن يتغير . |
| [Merge](../../groupdocs.search/index/merge#merge_1)(IndexRepository, MergeOptions) | يدمج الفهارس من مستودع الفهرس المحدد في الفهرس الحالي . لاحظ أن الفهارس في المستودع لن تتغير . |
| [Notify](../../groupdocs.search/index/notify)(Notification) | تمرير كائن الإعلام المحدد إلى الفهرس لإجراء الإخطار. |
| [Optimize](../../groupdocs.search/index/optimize#optimize)() | تقلل عدد مقاطع الفهرس عن طريق دمجها مع بعضها البعض. تعمل هذه العملية على تحسين أداء البحث . |
| [Optimize](../../groupdocs.search/index/optimize#optimize_1)(MergeOptions) | تقلل عدد مقاطع الفهرس عن طريق دمجها مع بعضها البعض. تعمل هذه العملية على تحسين أداء البحث . |
| [Search](../../groupdocs.search/index/search#search_1)(SearchQuery) | عمليات البحث في الفهرس . |
| [Search](../../groupdocs.search/index/search#search_3)(string) | عمليات البحث في الفهرس . |
| [Search](../../groupdocs.search/index/search#search)(SearchImage, ImageSearchOptions) | يقوم بإجراء بحث عكسي عن الصور في الفهرس. |
| [Search](../../groupdocs.search/index/search#search_2)(SearchQuery, SearchOptions) | عمليات البحث في الفهرس . |
| [Search](../../groupdocs.search/index/search#search_4)(string, SearchOptions) | عمليات البحث في الفهرس . |
| [SearchNext](../../groupdocs.search/index/searchnext#searchnext)(ChunkSearchToken) | يواصل البحث المقتطع الذي بدأ باستخدام طريقة البحث. |
| [SearchNext](../../groupdocs.search/index/searchnext#searchnext_1)(ChunkSearchToken, Cancellation) | يواصل البحث المقتطع الذي بدأ باستخدام طريقة البحث. |
| [Update](../../groupdocs.search/index/update#update)() | إعادة فهرسة المستندات التي تم تغييرها أو حذفها منذ آخر تحديث . إضافة الملفات الجديدة التي تمت إضافتها إلى المجلدات المفهرسة. |
| [Update](../../groupdocs.search/index/update#update_1)(UpdateOptions) | إعادة فهرسة المستندات التي تم تغييرها أو حذفها منذ آخر تحديث . إضافة الملفات الجديدة التي تمت إضافتها إلى المجلدات المفهرسة. |

### ملاحظات

**يتعلم أكثر**

* [إنشاء فهرس](https://docs.groupdocs.com/display/searchnet/Creating+an+index)
* [الفهرسة](https://docs.groupdocs.com/display/searchnet/Indexing)
* [يبحث](https://docs.groupdocs.com/display/searchnet/Searching)

### أمثلة

يوضح المثال استخدامًا نموذجيًا للفئة.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

Index index = new Index(indexFolder); // إنشاء الفهرس في المجلد المحدد
index.Add(documentsFolder); // فهرسة المستندات من المجلد المحدد

SearchResult result = index.Search(query); // البحث في الفهرس
```

### أنظر أيضا

* مساحة الاسم [GroupDocs.Search](../../groupdocs.search)
* المجسم [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
