---
title: SearchDocumentFilter
second_title: GroupDocs.Search efter .NET API Reference
description: Innehåller metoder för att skapa sökdokumentfilter.
type: docs
weight: 1030
url: /sv/net/groupdocs.search.options/searchdocumentfilter/
---
## SearchDocumentFilter class

Innehåller metoder för att skapa sökdokumentfilter.

```csharp
public static class SearchDocumentFilter
```

## Metoder

| namn | Beskrivning |
| --- | --- |
| static [CreateAnd](../../groupdocs.search.options/searchdocumentfilter/createand)(params ISearchDocumentFilter[]) | Skapar en logisk konjunktion av de angivna filtren. |
| static [CreateAttribute](../../groupdocs.search.options/searchdocumentfilter/createattribute)(params string[]) | Skapar ett filter för att hoppa över dokument som inte har något värde från den angivna listan över tillåtna attribut. |
| static [CreateFileExtension](../../groupdocs.search.options/searchdocumentfilter/createfileextension)(params string[]) | Skapar ett filter för att hoppa över dokument som inte finns i den angivna listan över möjliga tillägg. |
| static [CreateFilePathRegularExpression](../../groupdocs.search.options/searchdocumentfilter/createfilepathregularexpression#createfilepathregularexpression)(string) | Skapar ett filter för att hoppa över dokument som inte matchar ett reguljärt uttryck. Det reguljära uttrycket tillämpas på hela sökvägen till ett dokument. |
| static [CreateFilePathRegularExpression](../../groupdocs.search.options/searchdocumentfilter/createfilepathregularexpression#createfilepathregularexpression_1)(string, RegexOptions) | Skapar ett filter för att hoppa över dokument som inte matchar ett reguljärt uttryck. Det reguljära uttrycket tillämpas på hela sökvägen till ett dokument. |
| static [CreateNot](../../groupdocs.search.options/searchdocumentfilter/createnot)(ISearchDocumentFilter) | Skapar ett filter som har invers logik i förhållande till det angivna inre filtret. |
| static [CreateOr](../../groupdocs.search.options/searchdocumentfilter/createor)(params ISearchDocumentFilter[]) | Skapar en logisk disjunktion av de angivna filtren. |

### Anmärkningar

**Läs mer**

* [Dokumentfiltrering i sökresultat](https://docs.groupdocs.com/display/searchnet/Document+filtering+in+search+result)
* [sökmöjligheter](https://docs.groupdocs.com/display/searchnet/Search+options)

### Se även

* namnutrymme [GroupDocs.Search.Options](../../groupdocs.search.options)
* hopsättning [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
