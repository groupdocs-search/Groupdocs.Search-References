---
title: "CreateLazy"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Crea un documento caricato in modo lazy."
type: docs
weight: 40
url: /it/net/groupdocs.search.common/document/createlazy/
---
## Document.CreateLazy method

Crea un documento caricato pigramente.

```csharp
public static Document CreateLazy(DocumentSourceKind documentSourceKind, string documentKey, 
    IDocumentLoader documentLoader)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| documentSourceKind | DocumentSourceKind | Il tipo di origine del documento. Questo valore deve corrispondere al tipo del documento caricato. |
| documentKey | String | La chiave del documento. Questo valore deve corrispondere alla chiave del documento caricato. |
| documentLoader | IDocumentLoader | Il caricatore del documento. |

### Valore di ritorno

Il documento creato.

### Vedi anche

* enum [DocumentSourceKind](../../documentsourcekind)
* interface [IDocumentLoader](../../idocumentloader)
* class [Document](../../document)
* namespace [GroupDocs.Search.Common](../../../groupdocs.search.common)
* assembly [GroupDocs.Search](../../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
