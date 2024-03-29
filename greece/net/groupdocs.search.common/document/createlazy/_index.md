---
title: CreateLazy
second_title: GroupDocs.Αναζήτηση για αναφορά API .NET
description: Δημιουργεί ένα έγγραφο με αργή φόρτωση.
type: docs
weight: 40
url: /el/net/groupdocs.search.common/document/createlazy/
---
## Document.CreateLazy method

Δημιουργεί ένα έγγραφο με αργή φόρτωση.

```csharp
public static Document CreateLazy(DocumentSourceKind documentSourceKind, string documentKey, 
    IDocumentLoader documentLoader)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| documentSourceKind | DocumentSourceKind | Το είδος της πηγής εγγράφου. Αυτή η τιμή πρέπει να ταιριάζει με το είδος του φορτωμένου εγγράφου. |
| documentKey | String | Το κλειδί εγγράφου. Αυτή η τιμή πρέπει να ταιριάζει με το κλειδί του φορτωμένου εγγράφου. |
| documentLoader | IDocumentLoader | Το πρόγραμμα φόρτωσης εγγράφων. |

### Επιστρεφόμενη Αξία

Το έγγραφο που δημιουργήθηκε.

### Δείτε επίσης

* enum [DocumentSourceKind](../../documentsourcekind)
* interface [IDocumentLoader](../../idocumentloader)
* class [Document](../../document)
* χώρος ονομάτων [GroupDocs.Search.Common](../../document)
* συνέλευση [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
