---
title: ImageSearchOptions
second_title: GroupDocs.Search for .NET API Reference
description: Provides options for reverse image search operation.
type: docs
weight: 950
url: /net/groupdocs.search.options/imagesearchoptions/
---
## ImageSearchOptions class

Provides options for reverse image search operation.

```csharp
public class ImageSearchOptions
```

## Constructors

| Name | Description |
| --- | --- |
| [ImageSearchOptions](imagesearchoptions)() | Initializes a new instance of the [`ImageSearchOptions`](../imagesearchoptions) class. |

## Properties

| Name | Description |
| --- | --- |
| [HashDifferences](../../groupdocs.search.options/imagesearchoptions/hashdifferences) { get; set; } | Gets or sets the maximum number of mismatched bits in the image hash. The default value is `5`. |
| [MaxResultCount](../../groupdocs.search.options/imagesearchoptions/maxresultcount) { get; set; } | Gets or sets the maximum number of found images for an image reverse search request. The default value is `1000`. |
| [SearchDocumentFilter](../../groupdocs.search.options/imagesearchoptions/searchdocumentfilter) { get; set; } | Gets or sets the search document filter. [`SearchDocumentFilter`](./searchdocumentfilter) works on the inclusion logic. Use [`SearchDocumentFilter`](../searchdocumentfilter) class for creation of a search document filter instances. The default value is `null`, which means that all found documents will be returned. |

### See Also

* namespace [GroupDocs.Search.Options](../../groupdocs.search.options)
* assembly [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.search.dll -->
