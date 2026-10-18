---
title: "CreateLazy"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Crée un document chargé paresseusement."
type: docs
weight: 40
url: /fr/net/groupdocs.search.common/document/createlazy/
---
## Document.CreateLazy method

Crée un document chargé paresseusement.

```csharp
public static Document CreateLazy(DocumentSourceKind documentSourceKind, string documentKey, 
    IDocumentLoader documentLoader)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| documentSourceKind | DocumentSourceKind | Le type de source du document. Cette valeur doit correspondre au type du document chargé. |
| documentKey | String | La clé du document. Cette valeur doit correspondre à la clé du document chargé. |
| documentLoader | IDocumentLoader | Le chargeur de document. |

### Valeur de retour

Le document créé.

### Voir aussi

* enum [DocumentSourceKind](../../documentsourcekind)
* interface [IDocumentLoader](../../idocumentloader)
* class [Document](../../document)
* namespace [GroupDocs.Search.Common](../../../groupdocs.search.common)
* assembly [GroupDocs.Search](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
