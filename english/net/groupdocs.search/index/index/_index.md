---
title: Index
second_title: GroupDocs.Search for .NET API Reference
description: Initializes a new instance of the Indexgroupdocs.search/index class in memory.
type: docs
weight: 10
url: /net/groupdocs.search/index/index/
---

## Index() {#constructor}

Initializes a new instance of the [`Index`](../../index) class in memory.

```csharp
public Index()
```

### Examples

The example demonstrates how to create an index in memory without saving files to disk.

```csharp
Index index = new Index(); 
```

### See Also

* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Index(IndexSettings) {#constructor_1}

Initializes a new instance of the [`Index`](../../index) class in memory with particular index settings.

```csharp
public Index(IndexSettings settings)
```

| Parameter | Type | Description |
| --- | --- | --- |
| settings | IndexSettings | The index settings object. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentException | A string of the document filter of the settings, such as a regular expression, has more than 65535 characters. |

### Examples

The example demonstrates how to create an index in memory without saving files to disk with particular index settings.

```csharp
IndexSettings settings = new IndexSettings();
settings.IndexType = IndexType.CompactIndex;
Index index = new Index(settings);
```

### See Also

* class [IndexSettings](../../indexsettings)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Index(string) {#constructor_2}

Initializes a new instance of the [`Index`](../../index) class. Creates a new or opens an existing index on disk.

```csharp
public Index(string indexFolder)
```

| Parameter | Type | Description |
| --- | --- | --- |
| indexFolder | String | The index folder path. |

### Exceptions

| exception | condition |
| --- | --- |
| InvalidOperationException | The folder contains an index of a previous version that must be updated with [`IndexUpdater`](../../indexupdater), an index of a version that cannot be updated, or an index created or changed by a newer version of the library; or it contains no index but files or subfolders that are not a part of an index. |
| IOException | Another [`Index`](../../index) object uses the folder, in this process or in another one, or an index is saved or updated into the folder at the moment. |
| InvalidDataException | The folder contains a damaged index: a file that the opening of the index reads is damaged, or the index has lost the files that record its changes. |
| FileNotFoundException | The folder contains a damaged index: a file that the opening of the index reads is missing. |

### Remarks

A new index is created in a folder that does not exist or is empty, or in a folder that holds only the files of an index that cannot be opened, for example of an index whose creation has failed: these files are deleted first. A folder that contains no index but other files or subfolders is refused, so that its content is not deleted: the folder of an index must not keep other data.

The errors that occur while an index is opened but do not prevent its opening, for example the damage of a dictionary that then gets its default content, are reported before a handler of the [`ErrorOccurred`](../../../groupdocs.search.events/eventhub/erroroccurred) event can be added: they are written to the log of the index (see [`Logger`](../../indexsettings/logger)) and are listed in the errors of the next indexing report (see [`Errors`](../../../groupdocs.search.common/indexingreport/errors)).

### Examples

The example demonstrates how to create an index on a disk or open an existing index.

```csharp
string indexFolder = @"c:\MyIndex\";
Index index = new Index(indexFolder); 
```

### See Also

* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Index(string, IndexSettings) {#constructor_4}

Initializes a new instance of the [`Index`](../../index) class. Creates a new index with particular settings or opens an existing index on disk.

```csharp
public Index(string indexFolder, IndexSettings settings)
```

| Parameter | Type | Description |
| --- | --- | --- |
| indexFolder | String | The index folder path. |
| settings | IndexSettings | The index settings object. |

### Exceptions

| exception | condition |
| --- | --- |
| InvalidOperationException | The folder contains an index of a previous version that must be updated with [`IndexUpdater`](../../indexupdater), an index of a version that cannot be updated, or an index created or changed by a newer version of the library; or it contains no index but files or subfolders that are not a part of an index. |
| ArgumentException | A new index is created, and a string of the document filter of the settings, such as a regular expression, has more than 65535 characters. |
| IOException | Another [`Index`](../../index) object uses the folder, in this process or in another one, or an index is saved or updated into the folder at the moment. |
| InvalidDataException | The folder contains a damaged index: a file that the opening of the index reads is damaged, or the index has lost the files that record its changes. |
| FileNotFoundException | The folder contains a damaged index: a file that the opening of the index reads is missing. |

### Remarks

A new index is created in a folder that does not exist or is empty, or in a folder that holds only the files of an index that cannot be opened, for example of an index whose creation has failed: these files are deleted first. A folder that contains no index but other files or subfolders is refused, so that its content is not deleted: the folder of an index must not keep other data.

The errors that occur while an index is opened but do not prevent its opening, for example the damage of a dictionary that then gets its default content, are reported before a handler of the [`ErrorOccurred`](../../../groupdocs.search.events/eventhub/erroroccurred) event can be added: they are written to the log of the index (see [`Logger`](../../indexsettings/logger)) and are listed in the errors of the next indexing report (see [`Errors`](../../../groupdocs.search.common/indexingreport/errors)).

### Examples

The example demonstrates how to create an index on a disk with particular index settings.

```csharp
string indexFolder = @"c:\MyIndex\";
IndexSettings settings = new IndexSettings();
settings.IndexType = IndexType.CompactIndex;
Index index = new Index(indexFolder, settings);
```

### See Also

* class [IndexSettings](../../indexsettings)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Index(string, bool) {#constructor_3}

Initializes a new instance of the [`Index`](../../index) class. Loads an existing index from disk if *overwriteIfExists* is `false`; creates a new index on disk otherwise.

```csharp
public Index(string indexFolder, bool overwriteIfExists)
```

| Parameter | Type | Description |
| --- | --- | --- |
| indexFolder | String | The index folder path. |
| overwriteIfExists | Boolean | The flag of overwriting the index folder. |

### Exceptions

| exception | condition |
| --- | --- |
| InvalidOperationException | *overwriteIfExists* is `false` and the folder contains an index of a previous version that must be updated with [`IndexUpdater`](../../indexupdater), an index of a version that cannot be updated, or an index created or changed by a newer version of the library; or it contains no index but files or subfolders that are not a part of an index. |
| IOException | Another [`Index`](../../index) object uses the folder, in this process or in another one, or an index is saved or updated into the folder at the moment. |
| InvalidDataException | *overwriteIfExists* is `false` and the folder contains a damaged index: a file that the opening of the index reads is damaged, or the index has lost the files that record its changes. |
| FileNotFoundException | *overwriteIfExists* is `false` and the folder contains a damaged index: a file that the opening of the index reads is missing. |

### Remarks

If *overwriteIfExists* is `true`, a new index is created in any folder, and all the files and the subfolders of the folder are deleted first. Otherwise a new index is created in a folder that does not exist or is empty, or in a folder that holds only the files of an index that cannot be opened, for example of an index whose creation has failed; a folder that contains no index but other files or subfolders is refused, so that its content is not deleted. The folder of an index must not keep other data.

The errors that occur while an index is opened but do not prevent its opening, for example the damage of a dictionary that then gets its default content, are reported before a handler of the [`ErrorOccurred`](../../../groupdocs.search.events/eventhub/erroroccurred) event can be added: they are written to the log of the index (see [`Logger`](../../indexsettings/logger)) and are listed in the errors of the next indexing report (see [`Errors`](../../../groupdocs.search.common/indexingreport/errors)).

### Examples

The example demonstrates how to create a new index in a folder that already contains another index.

```csharp
string indexFolder = @"c:\MyIndex\";
Index index = new Index(indexFolder, true);
```

### See Also

* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Index(string, IndexSettings, bool) {#constructor_5}

Initializes a new instance of the [`Index`](../../index) class. Loads an existing index from disk if *overwriteIfExists* is `false`; creates a new index on disk with particular index settings otherwise.

```csharp
public Index(string indexFolder, IndexSettings settings, bool overwriteIfExists)
```

| Parameter | Type | Description |
| --- | --- | --- |
| indexFolder | String | The index folder path. |
| settings | IndexSettings | The index settings object. |
| overwriteIfExists | Boolean | The flag of overwriting the index folder. |

### Exceptions

| exception | condition |
| --- | --- |
| InvalidOperationException | *overwriteIfExists* is `false` and the folder contains an index of a previous version that must be updated with [`IndexUpdater`](../../indexupdater), an index of a version that cannot be updated, or an index created or changed by a newer version of the library; or it contains no index but files or subfolders that are not a part of an index. |
| ArgumentException | A new index is created, and a string of the document filter of the settings, such as a regular expression, has more than 65535 characters. |
| IOException | Another [`Index`](../../index) object uses the folder, in this process or in another one, or an index is saved or updated into the folder at the moment. |
| InvalidDataException | *overwriteIfExists* is `false` and the folder contains a damaged index: a file that the opening of the index reads is damaged, or the index has lost the files that record its changes. |
| FileNotFoundException | *overwriteIfExists* is `false` and the folder contains a damaged index: a file that the opening of the index reads is missing. |

### Remarks

If *overwriteIfExists* is `true`, a new index is created in any folder, and all the files and the subfolders of the folder are deleted first. Otherwise a new index is created in a folder that does not exist or is empty, or in a folder that holds only the files of an index that cannot be opened, for example of an index whose creation has failed; a folder that contains no index but other files or subfolders is refused, so that its content is not deleted. The folder of an index must not keep other data.

The errors that occur while an index is opened but do not prevent its opening, for example the damage of a dictionary that then gets its default content, are reported before a handler of the [`ErrorOccurred`](../../../groupdocs.search.events/eventhub/erroroccurred) event can be added: they are written to the log of the index (see [`Logger`](../../indexsettings/logger)) and are listed in the errors of the next indexing report (see [`Errors`](../../../groupdocs.search.common/indexingreport/errors)).

### Examples

The example demonstrates how to create an index on a disk with particular index settings.

```csharp
string indexFolder = @"c:\MyIndex\";
IndexSettings settings = new IndexSettings();
settings.IndexType = IndexType.CompactIndex;
Index index = new Index(indexFolder, settings, true);
```

### See Also

* class [IndexSettings](../../indexsettings)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
