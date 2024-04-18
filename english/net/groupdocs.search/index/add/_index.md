---
title: Add
second_title: GroupDocs.Search for .NET API Reference
description: Performs indexing operation. Adds a file or folder by an absolute or relative path. Documents from all subfolders will be indexed.
type: docs
weight: 70
url: /net/groupdocs.search/index/add/
---
## Add(string) {#add_2}

Performs indexing operation. Adds a file or folder by an absolute or relative path. Documents from all subfolders will be indexed.

```csharp
public void Add(string path)
```

| Parameter | Type | Description |
| --- | --- | --- |
| path | String | The path to a file or folder to be indexed. |

### Examples

The example demonstrates how to add documents to an index.

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(folderPath); // Indexing documents in the specified folder
index.Add(filePath); // Indexing the specified document
```

### See Also

* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Add(string, IndexingOptions) {#add_3}

Performs indexing operation. Adds a file or folder by an absolute or relative path. Documents from all subfolders will be indexed.

```csharp
public void Add(string path, IndexingOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| path | String | The path to a file or folder to be indexed. |
| options | IndexingOptions | The indexing options. |

### Examples

The example demonstrates how to add documents to an index with particular indexing options.

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

### See Also

* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Add(string[]) {#add_4}

Performs indexing operation. Adds files or folders by an absolute or relative path. Documents from all subfolders will be indexed.

```csharp
public void Add(string[] paths)
```

| Parameter | Type | Description |
| --- | --- | --- |
| paths | String[] | The paths to a files or folders to be indexed. |

### Examples

The example demonstrates how to add documents to an index.

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // Creating index in the specified folder

string[] paths = new string[] { folderPath, filePath };
index.Add(paths); // Indexing documents at the specified paths
```

### See Also

* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Add(string[], IndexingOptions) {#add_5}

Performs indexing operation. Adds files or folders by an absolute or relative path. Documents from all subfolders will be indexed.

```csharp
public void Add(string[] paths, IndexingOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| paths | String[] | The paths to a files or folders to be indexed. |
| options | IndexingOptions | The indexing options. |

### Examples

The example demonstrates how to add documents to an index with particular indexing options.

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

### See Also

* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Add(Document[], IndexingOptions) {#add}

Performs indexing operation. Adds documents from file system, stream or structure.

```csharp
public void Add(Document[] documents, IndexingOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| documents | Document[] | The documents from file system, stream or structure. |
| options | IndexingOptions | The indexing options. |

### See Also

* class [Document](../../../groupdocs.search.common/document)
* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Add(ExtractedData[], IndexingOptions) {#add_1}

Performs indexing operation. Adds the extracted data to the index.

```csharp
public void Add(ExtractedData[] data, IndexingOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| data | ExtractedData[] | The extracted data. |
| options | IndexingOptions | The indexing options. |

### See Also

* class [ExtractedData](../../../groupdocs.search.common/extracteddata)
* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.search.dll -->
