---
title: Add
second_title: GroupDocs.Search for .NET API Reference
description: Performs an indexing operation. Adds a file or folder by an absolute or relative path. Documents from all subfolders will be indexed.
type: docs
weight: 80
url: /net/groupdocs.search/index/add/
---

## Add(string) {#add_2}

Performs an indexing operation. Adds a file or folder by an absolute or relative path. Documents from all subfolders will be indexed.

```csharp
public void Add(string path)
```

| Parameter | Type | Description |
| --- | --- | --- |
| path | String | The path to a file or folder to be indexed. |

### Exceptions

| exception | condition |
| --- | --- |
| ObjectDisposedException | The index is disposed. |

### Remarks

The links to folders inside an added folder, for example the symbolic links and the junctions, are not followed: add the folder that a link names to index its documents. An added path that is a link itself is followed.

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

Performs an indexing operation. Adds a file or folder by an absolute or relative path. Documents from all subfolders will be indexed.

```csharp
public void Add(string path, IndexingOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| path | String | The path to a file or folder to be indexed. |
| options | IndexingOptions | The indexing options. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | The indexing options are `null`. |
| ObjectDisposedException | The index is disposed. |

### Remarks

The links to folders inside an added folder, for example the symbolic links and the junctions, are not followed: add the folder that a link names to index its documents. An added path that is a link itself is followed.

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

Performs an indexing operation. Adds files or folders by an absolute or relative path. Documents from all subfolders will be indexed.

```csharp
public void Add(string[] paths)
```

| Parameter | Type | Description |
| --- | --- | --- |
| paths | String[] | The paths to files or folders to be indexed. |

### Exceptions

| exception | condition |
| --- | --- |
| ObjectDisposedException | The index is disposed. |

### Remarks

The links to folders inside an added folder, for example the symbolic links and the junctions, are not followed: add the folder that a link names to index its documents. An added path that is a link itself is followed.

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

Performs an indexing operation. Adds files or folders by an absolute or relative path. Documents from all subfolders will be indexed.

```csharp
public void Add(string[] paths, IndexingOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| paths | String[] | The paths to files or folders to be indexed. |
| options | IndexingOptions | The indexing options. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | The indexing options are `null`. |
| ObjectDisposedException | The index is disposed. |

### Remarks

The links to folders inside an added folder, for example the symbolic links and the junctions, are not followed: add the folder that a link names to index its documents. An added path that is a link itself is followed.

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

Performs an indexing operation. Adds documents from file system, stream or structure.

```csharp
public void Add(Document[] documents, IndexingOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| documents | Document[] | The documents from file system, stream or structure. |
| options | IndexingOptions | The indexing options. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | The indexing options are `null`. |
| ArgumentException | A document is `null`. |
| ObjectDisposedException | The index is disposed. |

### Remarks

A document of a file is indexed with its attributes and additional fields, and a lazy document of a file is loaded when the file is indexed and closed after it; the loader gives the document of the same file. The file is found by the key of the document, as a file that is added by its path: a file that does not exist, does not pass the document filter or is indexed already is not loaded.

An update indexes a changed file again by its path, with the attributes of its indexed version but without the additional fields of its document; the [`FileIndexing`](../../../groupdocs.search.events/eventhub/fileindexing) event sees the attributes and can replace them, and can give the additional fields.

### See Also

* class [Document](../../../groupdocs.search.common/document)
* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Add(ExtractedData[], IndexingOptions) {#add_1}

Performs an indexing operation. Adds the extracted data to the index.

```csharp
public void Add(ExtractedData[] data, IndexingOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| data | ExtractedData[] | The extracted data. |
| options | IndexingOptions | The indexing options. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | The extracted data or the indexing options are `null`. |
| ArgumentException | The extracted data of a document is `null`. |
| ObjectDisposedException | The index is disposed. |

### See Also

* class [ExtractedData](../../../groupdocs.search.common/extracteddata)
* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
