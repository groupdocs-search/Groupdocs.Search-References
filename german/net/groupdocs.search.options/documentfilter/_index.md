---
title: "DocumentFilter"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Stellt die Basisklasse für Dokumentfilter dar. Enthält Methoden zur Erstellung von Dokumentfilter-Instanzen."
type: docs
weight: 850
url: /de/net/groupdocs.search.options/documentfilter/
---
## DocumentFilter class

Stellt die Basisklasse für Dokumentfilter dar. Enthält Methoden zur Erstellung von Dokumentfilter-Instanzen.

```csharp
public abstract class DocumentFilter
```

## Methoden

| Name | Beschreibung |
| --- | --- |
| static [CreateAnd](../../groupdocs.search.options/documentfilter/createand)(params DocumentFilter[]) | Erstellt eine logische Konjunktion der angegebenen Filter. |
| static [CreateCreationTimeLowerBound](../../groupdocs.search.options/documentfilter/createcreationtimelowerbound)(DateTime) | Erstellt einen Filter zum Überspringen von Dokumenten mit Erstellungsdatum, das vor der Untergrenze liegt. |
| static [CreateCreationTimeRange](../../groupdocs.search.options/documentfilter/createcreationtimerange)(DateTime, DateTime) | Erstellt einen Filter zum Überspringen von Dokumenten mit Erstellungsdatum außerhalb des angegebenen Bereichs. |
| static [CreateCreationTimeUpperBound](../../groupdocs.search.options/documentfilter/createcreationtimeupperbound)(DateTime) | Erstellt einen Filter zum Überspringen von Dokumenten mit Erstellungsdatum, das nach der Obergrenze liegt. |
| static [CreateFileExtension](../../groupdocs.search.options/documentfilter/createfileextension)(params string[]) | Erstellt einen Filter zum Überspringen von Dokumenten, die keine zulässige Erweiterung besitzen. |
| static [CreateFileLengthLowerBound](../../groupdocs.search.options/documentfilter/createfilelengthlowerbound)(long) | Erstellt einen Filter zum Überspringen von Dokumenten mit einer Länge, die kleiner als die Untergrenze ist. |
| static [CreateFileLengthRange](../../groupdocs.search.options/documentfilter/createfilelengthrange)(long, long) | Erstellt einen Filter zum Überspringen von Dokumenten außerhalb des angegebenen Längenbereichs. |
| static [CreateFileLengthUpperBound](../../groupdocs.search.options/documentfilter/createfilelengthupperbound)(long) | Erstellt einen Filter zum Überspringen von Dokumenten mit einer Länge, die größer als die Obergrenze ist. |
| static [CreateFilePathRegularExpression](../../groupdocs.search.options/documentfilter/createfilepathregularexpression#createfilepathregularexpression)(string) | Erstellt einen Filter, um Dokumente zu überspringen, die nicht einem regulären Ausdruck entsprechen. Der reguläre Ausdruck wird auf den vollständigen Pfad eines Dokuments angewendet. |
| static [CreateFilePathRegularExpression](../../groupdocs.search.options/documentfilter/createfilepathregularexpression#createfilepathregularexpression_1)(string, RegexOptions) | Erstellt einen Filter, um Dokumente zu überspringen, die nicht einem regulären Ausdruck entsprechen. Der reguläre Ausdruck wird auf den vollständigen Pfad eines Dokuments angewendet. |
| static [CreateModificationTimeLowerBound](../../groupdocs.search.options/documentfilter/createmodificationtimelowerbound)(DateTime) | Erstellt einen Filter zum Überspringen von Dokumenten mit Änderungsdatum, das vor der Untergrenze liegt. |
| static [CreateModificationTimeRange](../../groupdocs.search.options/documentfilter/createmodificationtimerange)(DateTime, DateTime) | Erstellt einen Filter zum Überspringen von Dokumenten mit Änderungsdatum außerhalb des angegebenen Bereichs. |
| static [CreateModificationTimeUpperBound](../../groupdocs.search.options/documentfilter/createmodificationtimeupperbound)(DateTime) | Erstellt einen Filter zum Überspringen von Dokumenten mit Änderungsdatum, das nach der Obergrenze liegt. |
| static [CreateNot](../../groupdocs.search.options/documentfilter/createnot)(DocumentFilter) | Erstellt einen Filter, der eine inverse Logik in Bezug auf den angegebenen inneren Filter hat. |
| static [CreateOr](../../groupdocs.search.options/documentfilter/createor)(params DocumentFilter[]) | Erstellt eine logische Disjunktion der angegebenen Filter. |
| abstract [ToString](../../groupdocs.search.options/documentfilter/tostring)() | Gibt die Zeichenkettenrepräsentation eines Dokumentfilters zurück. |

### Hinweise

**Learn more**

* [Document filtering during indexing](https://docs.groupdocs.com/display/searchnet/Document+filtering+during+indexing)

### Siehe auch

* namespace [GroupDocs.Search.Options](../../groupdocs.search.options)
* assembly [GroupDocs.Search](../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
