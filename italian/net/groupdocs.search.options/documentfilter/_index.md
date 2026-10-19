---
title: "DocumentFilter"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Rappresenta la classe base per i filtri di documento. Contiene metodi per la creazione di istanze di filtri di documento."
type: docs
weight: 850
url: /it/net/groupdocs.search.options/documentfilter/
---
## DocumentFilter class

Rappresenta la classe base per i filtri di documento. Contiene metodi per la creazione di istanze di filtri di documento.

```csharp
public abstract class DocumentFilter
```

## Metodi

| Nome | Descrizione |
| --- | --- |
| static [CreateAnd](../../groupdocs.search.options/documentfilter/createand)(params DocumentFilter[]) | Crea una congiunzione logica dei filtri specificati. |
| static [CreateCreationTimeLowerBound](../../groupdocs.search.options/documentfilter/createcreationtimelowerbound)(DateTime) | Crea un filtro per saltare i documenti con data di creazione precedente al limite inferiore. |
| static [CreateCreationTimeRange](../../groupdocs.search.options/documentfilter/createcreationtimerange)(DateTime, DateTime) | Crea un filtro per saltare i documenti con data di creazione fuori dall'intervallo specificato. |
| static [CreateCreationTimeUpperBound](../../groupdocs.search.options/documentfilter/createcreationtimeupperbound)(DateTime) | Crea un filtro per saltare i documenti con data di creazione successiva al limite superiore. |
| static [CreateFileExtension](../../groupdocs.search.options/documentfilter/createfileextension)(params string[]) | Crea un filtro per saltare i documenti che non hanno un'estensione consentita. |
| static [CreateFileLengthLowerBound](../../groupdocs.search.options/documentfilter/createfilelengthlowerbound)(long) | Crea un filtro per saltare i documenti con lunghezza inferiore al limite inferiore. |
| static [CreateFileLengthRange](../../groupdocs.search.options/documentfilter/createfilelengthrange)(long, long) | Crea un filtro per saltare i documenti fuori dall'intervallo di lunghezza specificato. |
| static [CreateFileLengthUpperBound](../../groupdocs.search.options/documentfilter/createfilelengthupperbound)(long) | Crea un filtro per saltare i documenti con lunghezza superiore al limite superiore. |
| static [CreateFilePathRegularExpression](../../groupdocs.search.options/documentfilter/createfilepathregularexpression#createfilepathregularexpression)(string) | Crea un filtro per saltare i documenti che non corrispondono a un'espressione regolare. L'espressione regolare è applicata al percorso completo di un documento. |
| static [CreateFilePathRegularExpression](../../groupdocs.search.options/documentfilter/createfilepathregularexpression#createfilepathregularexpression_1)(string, RegexOptions) | Crea un filtro per saltare i documenti che non corrispondono a un'espressione regolare. L'espressione regolare è applicata al percorso completo di un documento. |
| static [CreateModificationTimeLowerBound](../../groupdocs.search.options/documentfilter/createmodificationtimelowerbound)(DateTime) | Crea un filtro per saltare i documenti con data di modifica precedente al limite inferiore. |
| static [CreateModificationTimeRange](../../groupdocs.search.options/documentfilter/createmodificationtimerange)(DateTime, DateTime) | Crea un filtro per saltare i documenti con data di modifica fuori dall'intervallo specificato. |
| static [CreateModificationTimeUpperBound](../../groupdocs.search.options/documentfilter/createmodificationtimeupperbound)(DateTime) | Crea un filtro per saltare i documenti con data di modifica successiva al limite superiore. |
| static [CreateNot](../../groupdocs.search.options/documentfilter/createnot)(DocumentFilter) | Crea un filtro che ha una logica inversa rispetto al filtro interno specificato. |
| static [CreateOr](../../groupdocs.search.options/documentfilter/createor)(params DocumentFilter[]) | Crea una disgiunzione logica dei filtri specificati. |
| abstract [ToString](../../groupdocs.search.options/documentfilter/tostring)() | Restituisce la rappresentazione stringa di un filtro di documento. |

### Osservazioni

**Learn more**

* [Document filtering during indexing](https://docs.groupdocs.com/display/searchnet/Document+filtering+during+indexing)

### Vedi anche

* namespace [GroupDocs.Search.Options](../../groupdocs.search.options)
* assembly [GroupDocs.Search](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
