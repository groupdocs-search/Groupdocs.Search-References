---
title: CreateLazy
second_title: .NET API Başvurusu için GroupDocs.Search
description: Geç yüklenmiş bir belge oluşturur.
type: docs
weight: 40
url: /tr/net/groupdocs.search.common/document/createlazy/
---
## Document.CreateLazy method

Geç yüklenmiş bir belge oluşturur.

```csharp
public static Document CreateLazy(DocumentSourceKind documentSourceKind, string documentKey, 
    IDocumentLoader documentLoader)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| documentSourceKind | DocumentSourceKind | Belge kaynağı türü. Bu değer, yüklenen belgenin türüyle eşleşmelidir. |
| documentKey | String | Belge anahtarı. Bu değer, yüklenen belgenin anahtarıyla eşleşmelidir. |
| documentLoader | IDocumentLoader | Belge yükleyici. |

### Geri dönüş değeri

Oluşturulan belge.

### Ayrıca bakınız

* enum [DocumentSourceKind](../../documentsourcekind)
* interface [IDocumentLoader](../../idocumentloader)
* class [Document](../../document)
* ad alanı [GroupDocs.Search.Common](../../document)
* toplantı [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->