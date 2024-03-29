---
title: MetadataIndexingOptions
second_title: GroupDocs.Search efter .NET API Reference
description: Ger alternativ för att indexera metadatafält.
type: docs
weight: 970
url: /sv/net/groupdocs.search.options/metadataindexingoptions/
---
## MetadataIndexingOptions class

Ger alternativ för att indexera metadatafält.

```csharp
public class MetadataIndexingOptions
```

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [DefaultFieldName](../../groupdocs.search.options/metadataindexingoptions/defaultfieldname) { get; set; } | Hämtar eller ställer in standardfältnamnet som används för att indexera tomma fältnamn. Standardvärdet är`"okänd"` . |
| [IndexingEmptyNames](../../groupdocs.search.options/metadataindexingoptions/indexingemptynames) { get; set; } | Hämtar eller ställer in ett värde som anger om tomma fältnamn ska indexeras eller inte. Standardvärdet är`Sann` . |
| [IndexingEmptyValues](../../groupdocs.search.options/metadataindexingoptions/indexingemptyvalues) { get; set; } | Hämtar eller ställer in ett värde som anger om tomma fältvärden ska indexeras eller inte. Standardvärdet är`Sann` . |
| [MaxBytesToIndexField](../../groupdocs.search.options/metadataindexingoptions/maxbytestoindexfield) { get; set; } | Hämtar eller ställer in det maximala antalet värden i en array av typen byte för att indexera fältet. Standardvärdet är`int.MaxValue` . |
| [MaxDoublesToIndexField](../../groupdocs.search.options/metadataindexingoptions/maxdoublestoindexfield) { get; set; } | Hämtar eller ställer in det maximala antalet värden i en matris av typen dubbelt för att indexera fältet. Standardvärdet är`int.MaxValue` . |
| [MaxIntsToIndexField](../../groupdocs.search.options/metadataindexingoptions/maxintstoindexfield) { get; set; } | Hämtar eller ställer in det maximala antalet värden i en array av typen int för att indexera fältet. Standardvärdet är`int.MaxValue` . |
| [MaxLongsToIndexField](../../groupdocs.search.options/metadataindexingoptions/maxlongstoindexfield) { get; set; } | Hämtar eller ställer in det maximala antalet värden i en array av typen long för att indexera fältet. Standardvärdet är`int.MaxValue` . |
| [SeparatorBetweenValues](../../groupdocs.search.options/metadataindexingoptions/separatorbetweenvalues) { get; set; } | Hämtar eller ställer in avgränsaren mellan värden i ett fält av typen array. Standardvärdet är mellanslagstecknet. |
| [SeparatorInCompoundName](../../groupdocs.search.options/metadataindexingoptions/separatorincompoundname) { get; set; } | Hämtar eller ställer in avgränsaren i det sammansatta namnet på ett fält. Standardvärdet är`"."` . |

### Anmärkningar

**Läs mer**

* [Indexeringsalternativ](https://docs.groupdocs.com/display/searchnet/Indexing+options)
* MetadataIndexingOptions används när du hämtar dokumenttext från ett index: [Få indexerade dokument](https://docs.groupdocs.com/display/searchnet/Getting+indexed+documents)
* MetadataIndexingOptions används när du markerar sökresultat: [Markera sökresultat](https://docs.groupdocs.com/display/searchnet/Highlighting+search+results)

### Se även

* namnutrymme [GroupDocs.Search.Options](../../groupdocs.search.options)
* hopsättning [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
