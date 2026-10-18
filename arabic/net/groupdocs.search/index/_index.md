---
title: "Index"
second_title: "GroupDocs.Search for .NET API Reference"
description: "يمثل الفئة الرئيسية لفهرسة المستندات والبحث فيها."
type: docs
weight: 700
url: /ar/net/groupdocs.search/index/
---
## Index class

يمثل الفئة الرئيسية لفهرسة المستندات والبحث فيها.

```csharp
public class Index : IDisposable
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [Index](index#constructor)() | يقوم بتهيئة نسخة جديدة من الفئة [`Index`](../index) في الذاكرة. |
| [Index](index#constructor_1)(IndexSettings) | يقوم بتهيئة نسخة جديدة من الفئة [`Index`](../index) في الذاكرة مع إعدادات فهرس محددة. |
| [Index](index#constructor_2)(string) | يقوم بتهيئة نسخة جديدة من الفئة [`Index`](../index). ينشئ فهرسًا جديدًا أو يفتح فهرسًا موجودًا على القرص. |
| [Index](index#constructor_3)(string, bool) | يقوم بتهيئة نسخة جديدة من الفئة [`Index`](../index). يحمل فهرسًا موجودًا من القرص إذا كان *overwriteIfExists* يساوي `false`؛ وإلا ينشئ فهرسًا جديدًا على القرص. |
| [Index](index#constructor_4)(string, IndexSettings) | يُهيئ نسخة جديدة من الفئة [`Index`](../index). ينشئ فهرسًا جديدًا بإعدادات معينة أو يفتح فهرسًا موجودًا على القرص. |
| [Index](index#constructor_5)(string, IndexSettings, bool) | يُهيئ نسخة جديدة من الفئة [`Index`](../index). يحمل فهرسًا موجودًا من القرص إذا كان *overwriteIfExists* يساوي `false`؛ وإلا ينشئ فهرسًا جديدًا على القرص بإعدادات فهرس معينة. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Dictionaries](../../groupdocs.search/index/dictionaries) { get; } | يحصل على مستودع القاموس. |
| [Events](../../groupdocs.search/index/events) { get; } | يحصل على مركز الأحداث للاشتراك في الأحداث. |
| [IndexInfo](../../groupdocs.search/index/indexinfo) { get; } | يحصل على المعلومات الأساسية حول الفهرس. |
| [IndexSettings](../../groupdocs.search/index/indexsettings) { get; } | يحصل على إعدادات الفهرس. |
| [Repository](../../groupdocs.search/index/repository) { get; } | يحصل على كائن مستودع الفهرس إذا كان الفهرس موجودًا فيه. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| static [LoadIntoMemoryCompletely](../../groupdocs.search/index/loadintomemorycompletely#loadintomemorycompletely)(string) | يحمل الفهرس بالكامل في الذاكرة. أي تغييرات تُجرى على الفهرس لا تُحفظ تلقائيًا في المجلد الأصلي. |
| static [LoadIntoMemoryCompletely](../../groupdocs.search/index/loadintomemorycompletely#loadintomemorycompletely_1)(string, IndexSettings) | يحمل الفهرس بالكامل في الذاكرة. أي تغييرات تُجرى على الفهرس لا تُحفظ تلقائيًا في المجلد الأصلي. |
| [Add](../../groupdocs.search/index/add#add_2)(string) | ينفّذ عملية الفهرسة. يضيف ملفًا أو مجلدًا باستخدام مسار مطلق أو نسبي. سيتم فهرسة المستندات من جميع المجلدات الفرعية. |
| [Add](../../groupdocs.search/index/add#add_4)(string[]) | ينفّذ عملية الفهرسة. يضيف ملفات أو مجلدات باستخدام مسار مطلق أو نسبي. سيتم فهرسة المستندات من جميع المجلدات الفرعية. |
| [Add](../../groupdocs.search/index/add#add)(Document[], IndexingOptions) | ينفّذ عملية الفهرسة. يضيف مستندات من نظام الملفات أو التدفق أو الهيكل. |
| [Add](../../groupdocs.search/index/add#add_1)(ExtractedData[], IndexingOptions) | ينفّذ عملية الفهرسة. يضيف البيانات المستخرجة إلى الفهرس. |
| [Add](../../groupdocs.search/index/add#add_3)(string, IndexingOptions) | ينفّذ عملية الفهرسة. يضيف ملفًا أو مجلدًا باستخدام مسار مطلق أو نسبي. سيتم فهرسة المستندات من جميع المجلدات الفرعية. |
| [Add](../../groupdocs.search/index/add#add_5)(string[], IndexingOptions) | ينفّذ عملية الفهرسة. يضيف ملفات أو مجلدات باستخدام مسار مطلق أو نسبي. سيتم فهرسة المستندات من جميع المجلدات الفرعية. |
| [ChangeAttributes](../../groupdocs.search/index/changeattributes)(AttributeChangeBatch) | يطبق مجموعة التغييرات المحددة للسمات على المستندات المفهرسة دون إعادة الفهرسة أثناء عملية التحديث. |
| [CheckSegments](../../groupdocs.search/index/checksegments)(bool) | يفحص الفهرس بحثًا عن ملفات أجزاء تالفة على القرص. تُصلّح الطريقة وظيفة الفهرس في وجود أجزاء تالفة إذا كان *fixIndexFunctionality* صحيحًا؛ ولا تُصلّح في غير ذلك. |
| [Delete](../../groupdocs.search/index/delete#delete_1)(string[], UpdateOptions) | يحذف الملفات أو المجلدات المفهرسة من الفهرس. ثم يُحدّث الفهرس بدون المسارات المحذوفة. لاحظ أن المستند الفردي لا يمكن حذفه من الفهرس إذا تم إضافته إلى الفهرس كجزء من مجلد. |
| [Delete](../../groupdocs.search/index/delete#delete)(UpdateOptions, string[]) | يحذف المستندات المفهرسة من التدفقات أو الهياكل. ثم يُحدّث الفهرس بدون المستندات المحذوفة. |
| [Dispose](../../groupdocs.search/index/dispose)() | يطلق جميع الموارد المستخدمة من قبل [`Index`](../index). |
| [GetAttributes](../../groupdocs.search/index/getattributes)(string) | يحصل على جميع السمات المرتبطة بالمستند المفهرس المحدد. |
| [GetDocumentText](../../groupdocs.search/index/getdocumenttext#getdocumenttext)(DocumentInfo, OutputAdapter) | ينشئ نص المستند المفهرس ويمرره عبر محول الإخراج. |
| [GetDocumentText](../../groupdocs.search/index/getdocumenttext#getdocumenttext_1)(DocumentInfo, OutputAdapter, TextOptions) | ينشئ نصًا بتنسيق HTML للمستند المفهرس وينقله عبر محول الإخراج. |
| [GetIndexedDocument](../../groupdocs.search/index/getindexeddocument)(string) | يحصل على مستند مفهرس باستخدام مفتاح المستند. |
| [GetIndexedDocumentItems](../../groupdocs.search/index/getindexeddocumentitems)(DocumentInfo) | يحصل على مصفوفة من العناصر المتداخلة للمستند المحدد (للمستندات الحاوية مثل ZIP وOST وPST). |
| [GetIndexedDocuments](../../groupdocs.search/index/getindexeddocuments)() | يحصل على مصفوفة من جميع المستندات المفهرسة. |
| [GetIndexedPaths](../../groupdocs.search/index/getindexedpaths)() | يحصل على مصفوفة من المسارات المفهرسة - مستندات أو مجلدات. |
| [GetIndexingReports](../../groupdocs.search/index/getindexingreports)() | يحصل على التقارير حول عمليات الفهرسة. |
| [GetSearchReports](../../groupdocs.search/index/getsearchreports)() | يحصل على التقارير حول عمليات البحث. |
| [Highlight](../../groupdocs.search/index/highlight#highlight)(FoundDocument, Highlighter) | يولد نصًا بتنسيق HTML مع تسليط الضوء على المصطلحات التي تم العثور عليها. |
| [Highlight](../../groupdocs.search/index/highlight#highlight_1)(FoundDocument, Highlighter, HighlightOptions) | يولد نصًا بتنسيق HTML مع تسليط الضوء على المصطلحات التي تم العثور عليها. |
| [Merge](../../groupdocs.search/index/merge#merge)(Index, MergeOptions) | يدمج الفهرس المحدد في الفهرس الحالي. لاحظ أن الفهرس الآخر لن يتغير. |
| [Merge](../../groupdocs.search/index/merge#merge_1)(IndexRepository, MergeOptions) | يدمج الفهارس من مستودع الفهرس المحدد إلى الفهرس الحالي. لاحظ أن الفهارس في المستودع لن تتغير. |
| [Notify](../../groupdocs.search/index/notify)(Notification) | يمرر كائن الإشعار المحدد إلى الفهرس لتنفيذ الإشعار. |
| [Optimize](../../groupdocs.search/index/optimize#optimize)() | يقلل عدد أقسام الفهرس عن طريق دمجها واحدة مع الأخرى. هذه العملية تحسن أداء البحث. |
| [Optimize](../../groupdocs.search/index/optimize#optimize_1)(MergeOptions) | يقلل عدد أقسام الفهرس عن طريق دمجها واحدة مع الأخرى. هذه العملية تحسن أداء البحث. |
| [SaveTo](../../groupdocs.search/index/saveto)(string) | يحفظ الفهرس الموجود في الذاكرة إلى القرص. كما يحفظ الفهرس العادي إلى مجلد آخر. لا يغيّر إعدادات هذا الفهرس. |
| [Search](../../groupdocs.search/index/search#search_1)(SearchQuery) | يبحث في الفهرس. |
| [Search](../../groupdocs.search/index/search#search_3)(string) | يبحث في الفهرس. |
| [Search](../../groupdocs.search/index/search#search)(SearchImage, ImageSearchOptions) | ينفّذ بحثًا عكسيًا عن الصور في الفهرس. |
| [Search](../../groupdocs.search/index/search#search_2)(SearchQuery, SearchOptions) | يبحث في الفهرس. |
| [Search](../../groupdocs.search/index/search#search_4)(string, SearchOptions) | يبحث في الفهرس. |
| [SearchNext](../../groupdocs.search/index/searchnext#searchnext)(ChunkSearchToken) | يكمل بحث القطع الذي بدأ باستخدام طريقة Search. |
| [SearchNext](../../groupdocs.search/index/searchnext#searchnext_1)(ChunkSearchToken, Cancellation) | يكمل بحث القطع الذي بدأ باستخدام طريقة Search. |
| [Update](../../groupdocs.search/index/update#update)() | يعيد فهرسة المستندات التي تم تغييرها أو حذفها منذ آخر تحديث. يضيف الملفات الجديدة التي تم إضافتها إلى المجلدات المفهرسة. |
| [Update](../../groupdocs.search/index/update#update_1)(UpdateOptions) | يعيد فهرسة المستندات التي تم تغييرها أو حذفها منذ آخر تحديث. يضيف الملفات الجديدة التي تم إضافتها إلى المجلدات المفهرسة. |

### ملاحظات

**Learn more**

* [Creating an index](https://docs.groupdocs.com/display/searchnet/Creating+an+index)
* [Indexing](https://docs.groupdocs.com/display/searchnet/Indexing)
* [Searching](https://docs.groupdocs.com/display/searchnet/Searching)

### أمثلة

يوضح المثال استخدامًا نموذجيًا للفئة.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

SearchResult result = index.Search(query); // Searching in index
```

### انظر أيضًا

* namespace [GroupDocs.Search](../../groupdocs.search)
* assembly [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.search.dll -->
