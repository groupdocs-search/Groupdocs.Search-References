---
title: Add
second_title: GroupDocs.Search for .NET API Reference
description: Performs indexing operation. Indexing only from stream and structure is supported.
type: docs
weight: 10
url: /net/groupdocs.search.scaling/indexer/add/
---
## Add(Document[], string[], IndexingOptions) {#add}

Performs indexing operation. Indexing only from stream and structure is supported.

```csharp
public void Add(Document[] documents, string[] passwords, IndexingOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| documents | Document[] | The documents from stream or structure. |
| passwords | String[] | The document passwords. |
| options | IndexingOptions | The add options. |

### See Also

* class [Document](../../../groupdocs.search.common/document)
* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Indexer](../../indexer)
* namespace [GroupDocs.Search.Scaling](../../../groupdocs.search.scaling)
* assembly [GroupDocs.Search](../../../)

---

## Add(ExtractedData[], IndexingOptions) {#add_1}

Performs indexing operation. Adds the extracted data to the search network.

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
* class [Indexer](../../indexer)
* namespace [GroupDocs.Search.Scaling](../../../groupdocs.search.scaling)
* assembly [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.search.dll -->
