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

The example demonstrates how to create index in memory without saving files to disk.

```csharp
Index index = new Index(); 
```

### See Also

* class [Index](../../index)
* namespace [GroupDocs.Search](../../index)
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

### Examples

The example demonstrates how to create index in memory without saving files to disk with particular index settings.

```csharp
IndexSettings settings = new IndexSettings();
settings.IndexType = IndexType.CompactIndex;
Index index = new Index(settings);
```

### See Also

* class [IndexSettings](../../indexsettings)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../index)
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

### Examples

The example demonstrates how to create an index on a disk or open an existing index.

```csharp
string indexFolder = @"c:\MyIndex\";
Index index = new Index(indexFolder); 
```

### See Also

* class [Index](../../index)
* namespace [GroupDocs.Search](../../index)
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
* namespace [GroupDocs.Search](../../index)
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

### Examples

The example demonstrates how to create a new index in a folder that already contains another index.

```csharp
string indexFolder = @"c:\MyIndex\";
Index index = new Index(indexFolder, true);
```

### See Also

* class [Index](../../index)
* namespace [GroupDocs.Search](../../index)
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
* namespace [GroupDocs.Search](../../index)
* assembly [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.search.dll -->