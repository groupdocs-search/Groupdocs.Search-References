---
title: "Add"
second_title: "GroupDocs.Search for .NET API Reference"
description: "ينفّذ عملية الفهرسة. يضيف ملفًا أو مجلدًا باستخدام مسار مطلق أو نسبي. سيتم فهرسة المستندات من جميع المجلدات الفرعية."
type: docs
weight: 80
url: /ar/net/groupdocs.search/index/add/
---
## Add(string) {#add_2}

ينفّذ عملية الفهرسة. يضيف ملفًا أو مجلدًا باستخدام مسار مطلق أو نسبي. سيتم فهرسة المستندات من جميع المجلدات الفرعية.

```csharp
public void Add(string path)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| المسار | سلسلة | المسار إلى ملف أو مجلد ليتم فهرسته. |

### أمثلة

يوضح المثال كيفية إضافة المستندات إلى الفهرس.

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(folderPath); // Indexing documents in the specified folder
index.Add(filePath); // Indexing the specified document
```

### انظر أيضًا

* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Add(string, IndexingOptions) {#add_3}

ينفّذ عملية الفهرسة. يضيف ملفًا أو مجلدًا باستخدام مسار مطلق أو نسبي. سيتم فهرسة المستندات من جميع المجلدات الفرعية.

```csharp
public void Add(string path, IndexingOptions options)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| المسار | سلسلة | المسار إلى ملف أو مجلد ليتم فهرسته. |
| الخيارات | IndexingOptions | خيارات الفهرسة. |

### أمثلة

يوضح المثال كيفية إضافة المستندات إلى الفهرس مع خيارات فهرسة معينة.

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // Creating index in the specified folder

IndexingOptions options = new IndexingOptions();
options.Threads = 2; // Setting the number of indexing threads
index.Add(folderPath, options); // Indexing documents in the specified folder
index.Add(filePath, options); // Indexing the specified document
```

### انظر أيضًا

* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Add(string[]) {#add_4}

ينفّذ عملية الفهرسة. يضيف ملفات أو مجلدات باستخدام مسار مطلق أو نسبي. سيتم فهرسة المستندات من جميع المجلدات الفرعية.

```csharp
public void Add(string[] paths)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| المسارات | String[] | المسارات إلى ملفات أو مجلدات ليتم فهرستها. |

### أمثلة

يوضح المثال كيفية إضافة المستندات إلى الفهرس.

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // Creating index in the specified folder

string[] paths = new string[] { folderPath, filePath };
index.Add(paths); // Indexing documents at the specified paths
```

### انظر أيضًا

* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Add(string[], IndexingOptions) {#add_5}

ينفّذ عملية الفهرسة. يضيف ملفات أو مجلدات باستخدام مسار مطلق أو نسبي. سيتم فهرسة المستندات من جميع المجلدات الفرعية.

```csharp
public void Add(string[] paths, IndexingOptions options)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| المسارات | String[] | المسارات إلى ملفات أو مجلدات ليتم فهرستها. |
| الخيارات | IndexingOptions | خيارات الفهرسة. |

### أمثلة

يوضح المثال كيفية إضافة المستندات إلى الفهرس مع خيارات فهرسة معينة.

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // Creating index in the specified folder

IndexingOptions options = new IndexingOptions();
options.Threads = 2; // Setting the number of indexing threads
string[] paths = new string[] { folderPath, filePath };
index.Add(paths, options); // Indexing documents at the specified paths
```

### انظر أيضًا

* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Add(Document[], IndexingOptions) {#add}

ينفّذ عملية الفهرسة. يضيف مستندات من نظام الملفات أو التدفق أو الهيكل.

```csharp
public void Add(Document[] documents, IndexingOptions options)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| المستندات | Document[] | المستندات من نظام الملفات أو الدفق أو الهيكل. |
| الخيارات | IndexingOptions | خيارات الفهرسة. |

### انظر أيضًا

* class [Document](../../../groupdocs.search.common/document)
* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Add(ExtractedData[], IndexingOptions) {#add_1}

ينفّذ عملية الفهرسة. يضيف البيانات المستخرجة إلى الفهرس.

```csharp
public void Add(ExtractedData[] data, IndexingOptions options)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| البيانات | ExtractedData[] | البيانات المستخرجة. |
| الخيارات | IndexingOptions | خيارات الفهرسة. |

### انظر أيضًا

* class [ExtractedData](../../../groupdocs.search.common/extracteddata)
* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.search.dll -->
