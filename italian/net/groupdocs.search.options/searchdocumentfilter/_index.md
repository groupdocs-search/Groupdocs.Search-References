---
title: "SearchDocumentFilter"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Contiene metodi per creare filtri di ricerca per documenti."
type: docs
weight: 1090
url: /it/net/groupdocs.search.options/searchdocumentfilter/
---
## SearchDocumentFilter class

Contiene metodi per creare filtri di ricerca per documenti.

```csharp
public static class SearchDocumentFilter
```

## Metodi

| Nome | Descrizione |
| --- | --- |
| static [CreateAnd](../../groupdocs.search.options/searchdocumentfilter/createand)(params ISearchDocumentFilter[]) | Crea una congiunzione logica dei filtri specificati. |
| static [CreateAttribute](../../groupdocs.search.options/searchdocumentfilter/createattribute)(params string[]) | Crea un filtro per saltare i documenti che non hanno alcun valore dalla lista specificata di attributi consentiti. |
| static [CreateFileExtension](../../groupdocs.search.options/searchdocumentfilter/createfileextension)(params string[]) | Crea un filtro per saltare i documenti che non sono nella lista specificata di estensioni possibili. |
| static [CreateFilePathRegularExpression](../../groupdocs.search.options/searchdocumentfilter/createfilepathregularexpression#createfilepathregularexpression)(string) | Crea un filtro per saltare i documenti che non corrispondono a un'espressione regolare. L'espressione regolare è applicata al percorso completo di un documento. |
| static [CreateFilePathRegularExpression](../../groupdocs.search.options/searchdocumentfilter/createfilepathregularexpression#createfilepathregularexpression_1)(string, RegexOptions) | Crea un filtro per saltare i documenti che non corrispondono a un'espressione regolare. L'espressione regolare è applicata al percorso completo di un documento. |
| static [CreateNot](../../groupdocs.search.options/searchdocumentfilter/createnot)(ISearchDocumentFilter) | Crea un filtro che ha una logica inversa rispetto al filtro interno specificato. |
| static [CreateOr](../../groupdocs.search.options/searchdocumentfilter/createor)(params ISearchDocumentFilter[]) | Crea una disgiunzione logica dei filtri specificati. |

### Osservazioni

**Learn more**

* [Document filtering in search result](https://docs.groupdocs.com/display/searchnet/Document+filtering+in+search+result)
* [Search options](https://docs.groupdocs.com/display/searchnet/Search+options)

### Vedi anche

* namespace [GroupDocs.Search.Options](../../groupdocs.search.options)
* assembly [GroupDocs.Search](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
