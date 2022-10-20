---
title: CreateLazy
second_title: GroupDocs.Search for .NET API Reference
description: Creates a lazyloaded document.
type: docs
weight: 40
url: /net/groupdocs.search.common/document/createlazy/
---
## Document.CreateLazy method

Creates a lazy-loaded document.

```csharp
public static Document CreateLazy(DocumentSourceKind documentSourceKind, string documentKey, 
    IDocumentLoader documentLoader)
```

| Parameter | Type | Description |
| --- | --- | --- |
| documentSourceKind | DocumentSourceKind | The document source kind. This value must match the kind of the loaded document. |
| documentKey | String | The document key. This value must match the key of the loaded document. |
| documentLoader | IDocumentLoader | The document loader. |

### Return Value

The created document.

### See Also

* enum [DocumentSourceKind](../../documentsourcekind)
* interface [IDocumentLoader](../../idocumentloader)
* class [Document](../../document)
* namespace [GroupDocs.Search.Common](../../document)
* assembly [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.search.dll -->