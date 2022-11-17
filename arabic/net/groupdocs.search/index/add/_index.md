---
title: Add
second_title: GroupDocs. ابحث عن مرجع .NET API
description: يقوم بعملية الفهرسة. يضيف ملفًا أو مجلدًا بواسطة مسار مطلق أو نسبي. ستتم فهرسة المستندات من كافة المجلدات الفرعية.
type: docs
weight: 70
url: /ar/net/groupdocs.search/index/add/
---
## Add(string) {#add_2}

يقوم بعملية الفهرسة. يضيف ملفًا أو مجلدًا بواسطة مسار مطلق أو نسبي. ستتم فهرسة المستندات من كافة المجلدات الفرعية.

```csharp
public void Add(string path)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| path | String | المسار إلى الملف أو المجلد المراد فهرسته. |

### أمثلة

يوضح المثال كيفية إضافة مستندات إلى فهرس.

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // إنشاء الفهرس في المجلد المحدد
index.Add(folderPath); // فهرسة المستندات في المجلد المحدد
index.Add(filePath); // فهرسة الوثيقة المحددة
```

### أنظر أيضا

* class [Index](../../index)
* مساحة الاسم [GroupDocs.Search](../../index)
* المجسم [GroupDocs.Search](../../../)

---

## Add(string, IndexingOptions) {#add_3}

يقوم بعملية الفهرسة. يضيف ملفًا أو مجلدًا بواسطة مسار مطلق أو نسبي. ستتم فهرسة المستندات من كافة المجلدات الفرعية.

```csharp
public void Add(string path, IndexingOptions options)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| path | String | المسار إلى الملف أو المجلد المراد فهرسته. |
| options | IndexingOptions | خيارات الفهرسة. |

### أمثلة

يوضح المثال كيفية إضافة مستندات إلى فهرس بخيارات فهرسة معينة.

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // إنشاء الفهرس في المجلد المحدد

IndexingOptions options = new IndexingOptions();
options.Threads = 2; // تحديد عدد سلاسل الفهرسة
index.Add(folderPath, options); // فهرسة المستندات في المجلد المحدد
index.Add(filePath, options); // فهرسة الوثيقة المحددة
```

### أنظر أيضا

* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* مساحة الاسم [GroupDocs.Search](../../index)
* المجسم [GroupDocs.Search](../../../)

---

## Add(string[]) {#add_4}

يقوم بعملية الفهرسة. يضيف ملفات أو مجلدات بواسطة مسار مطلق أو نسبي. ستتم فهرسة المستندات من كافة المجلدات الفرعية.

```csharp
public void Add(string[] paths)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| paths | String[] | المسارات إلى الملفات أو المجلدات المراد فهرستها. |

### أمثلة

يوضح المثال كيفية إضافة مستندات إلى فهرس.

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // إنشاء الفهرس في المجلد المحدد

string[] paths = new string[] { folderPath, filePath };
index.Add(paths); // فهرسة المستندات في المسارات المحددة
```

### أنظر أيضا

* class [Index](../../index)
* مساحة الاسم [GroupDocs.Search](../../index)
* المجسم [GroupDocs.Search](../../../)

---

## Add(string[], IndexingOptions) {#add_5}

يقوم بعملية الفهرسة. يضيف ملفات أو مجلدات بواسطة مسار مطلق أو نسبي. ستتم فهرسة المستندات من كافة المجلدات الفرعية.

```csharp
public void Add(string[] paths, IndexingOptions options)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| paths | String[] | المسارات إلى الملفات أو المجلدات المراد فهرستها. |
| options | IndexingOptions | خيارات الفهرسة. |

### أمثلة

يوضح المثال كيفية إضافة مستندات إلى فهرس بخيارات فهرسة معينة.

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // إنشاء الفهرس في المجلد المحدد

IndexingOptions options = new IndexingOptions();
options.Threads = 2; // تحديد عدد سلاسل الفهرسة
string[] paths = new string[] { folderPath, filePath };
index.Add(paths, options); // فهرسة المستندات في المسارات المحددة
```

### أنظر أيضا

* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* مساحة الاسم [GroupDocs.Search](../../index)
* المجسم [GroupDocs.Search](../../../)

---

## Add(Document[], IndexingOptions) {#add}

يقوم بعملية الفهرسة. يضيف المستندات من نظام الملفات أو الدفق أو الهيكل .

```csharp
public void Add(Document[] documents, IndexingOptions options)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| documents | Document[] | المستندات من نظام الملفات أو الدفق أو الهيكل. |
| options | IndexingOptions | خيارات الفهرسة. |

### أنظر أيضا

* class [Document](../../../groupdocs.search.common/document)
* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* مساحة الاسم [GroupDocs.Search](../../index)
* المجسم [GroupDocs.Search](../../../)

---

## Add(ExtractedData[], IndexingOptions) {#add_1}

يقوم بعملية الفهرسة . يضيف البيانات المستخرجة إلى الفهرس .

```csharp
public void Add(ExtractedData[] data, IndexingOptions options)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| data | ExtractedData[] | البيانات المستخرجة. |
| options | IndexingOptions | خيارات الفهرسة. |

### أنظر أيضا

* class [ExtractedData](../../../groupdocs.search.common/extracteddata)
* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* مساحة الاسم [GroupDocs.Search](../../index)
* المجسم [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
