---
title: "CreateLazy"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Erstellt ein lazygeladenes Dokument."
type: docs
weight: 40
url: /de/net/groupdocs.search.common/document/createlazy/
---
## Document.CreateLazy method

Erstellt ein lazy-loaded Dokument.

```csharp
public static Document CreateLazy(DocumentSourceKind documentSourceKind, string documentKey, 
    IDocumentLoader documentLoader)
```

| Parameter | Type | Beschreibung |
| --- | --- | --- |
| documentSourceKind | DocumentSourceKind | Der Dokumentquellentyp. Dieser Wert muss dem Typ des geladenen Dokuments entsprechen. |
| documentKey | String | Der Dokumentschlüssel. Dieser Wert muss dem Schlüssel des geladenen Dokuments entsprechen. |
| documentLoader | IDocumentLoader | Der Dokumentlader. |

### Rückgabewert

Das erstellte Dokument.

### Siehe auch

* enum [DocumentSourceKind](../../documentsourcekind)
* interface [IDocumentLoader](../../idocumentloader)
* class [Document](../../document)
* namespace [GroupDocs.Search.Common](../../../groupdocs.search.common)
* assembly [GroupDocs.Search](../../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
