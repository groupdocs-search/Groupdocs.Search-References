---
title: SearchDocumentFilter
second_title: GroupDocs.Suche nach .NET-API-Referenz
description: Enthält Methoden zum Erstellen von Suchdokumentfiltern.
type: docs
weight: 1030
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
| static [CreateAnd](../../groupdocs.search.options/searchdocumentfilter/createand)(params ISearchDocumentFilter[]) | Erstellt eine logische Verknüpfung der angegebenen Filter. |
| static [CreateAttribute](../../groupdocs.search.options/searchdocumentfilter/createattribute)(params string[]) | Erstellt einen Filter zum Überspringen von Dokumenten, die keinen Wert aus der angegebenen Liste zulässiger Attribute haben. |
| static [CreateFileExtension](../../groupdocs.search.options/searchdocumentfilter/createfileextension)(params string[]) | Erstellt einen Filter zum Überspringen von Dokumenten, die nicht in der angegebenen Liste möglicher Erweiterungen enthalten sind. |
| static [CreateFilePathRegularExpression](../../groupdocs.search.options/searchdocumentfilter/createfilepathregularexpression#createfilepathregularexpression)(string) | Erstellt einen Filter zum Überspringen von Dokumenten, die keinem regulären Ausdruck entsprechen. Der reguläre Ausdruck wird auf den vollständigen Pfad eines Dokuments angewendet. |
| static [CreateFilePathRegularExpression](../../groupdocs.search.options/searchdocumentfilter/createfilepathregularexpression#createfilepathregularexpression_1)(string, RegexOptions) | Erstellt einen Filter zum Überspringen von Dokumenten, die keinem regulären Ausdruck entsprechen. Der reguläre Ausdruck wird auf den vollständigen Pfad eines Dokuments angewendet. |
| static [CreateNot](../../groupdocs.search.options/searchdocumentfilter/createnot)(ISearchDocumentFilter) | Erstellt einen Filter mit inverser Logik in Bezug auf den angegebenen inneren Filter. |
| static [CreateOr](../../groupdocs.search.options/searchdocumentfilter/createor)(params ISearchDocumentFilter[]) | Erstellt eine logische Trennung der angegebenen Filter. |

### Bemerkungen

**Erfahren Sie mehr**

* [Dokumentenfilterung im Suchergebnis](https://docs.groupdocs.com/display/searchnet/Document+filtering+in+search+result)
* [Suchoptionen](https://docs.groupdocs.com/display/searchnet/Search+options)

### Siehe auch

* namensraum [GroupDocs.Search.Options](../../groupdocs.search.options)
* Montage [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
