---
title: "SearchDocumentFilter"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Enthält Methoden zum Erstellen von Suchdokumentfiltern."
type: docs
weight: 1090
url: /de/net/groupdocs.search.options/searchdocumentfilter/
---
## SearchDocumentFilter class

Enthält Methoden zum Erstellen von Suchdokumentfiltern.

```csharp
public static class SearchDocumentFilter
```

## Methoden

| Name | Beschreibung |
| --- | --- |
| static [CreateAnd](../../groupdocs.search.options/searchdocumentfilter/createand)(params ISearchDocumentFilter[]) | Erstellt eine logische Konjunktion der angegebenen Filter. |
| static [CreateAttribute](../../groupdocs.search.options/searchdocumentfilter/createattribute)(params string[]) | Erstellt einen Filter, um Dokumente zu überspringen, die keinen Wert aus der angegebenen Liste zulässiger Attribute haben. |
| static [CreateFileExtension](../../groupdocs.search.options/searchdocumentfilter/createfileextension)(params string[]) | Erstellt einen Filter, um Dokumente zu überspringen, die nicht in der angegebenen Liste möglicher Erweiterungen enthalten sind. |
| static [CreateFilePathRegularExpression](../../groupdocs.search.options/searchdocumentfilter/createfilepathregularexpression#createfilepathregularexpression)(string) | Erstellt einen Filter, um Dokumente zu überspringen, die nicht einem regulären Ausdruck entsprechen. Der reguläre Ausdruck wird auf den vollständigen Pfad eines Dokuments angewendet. |
| static [CreateFilePathRegularExpression](../../groupdocs.search.options/searchdocumentfilter/createfilepathregularexpression#createfilepathregularexpression_1)(string, RegexOptions) | Erstellt einen Filter, um Dokumente zu überspringen, die nicht einem regulären Ausdruck entsprechen. Der reguläre Ausdruck wird auf den vollständigen Pfad eines Dokuments angewendet. |
| static [CreateNot](../../groupdocs.search.options/searchdocumentfilter/createnot)(ISearchDocumentFilter) | Erstellt einen Filter, der eine inverse Logik in Bezug auf den angegebenen inneren Filter hat. |
| static [CreateOr](../../groupdocs.search.options/searchdocumentfilter/createor)(params ISearchDocumentFilter[]) | Erstellt eine logische Disjunktion der angegebenen Filter. |

### Hinweise

**Learn more**

* [Document filtering in search result](https://docs.groupdocs.com/display/searchnet/Document+filtering+in+search+result)
* [Search options](https://docs.groupdocs.com/display/searchnet/Search+options)

### Siehe auch

* namespace [GroupDocs.Search.Options](../../groupdocs.search.options)
* assembly [GroupDocs.Search](../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
