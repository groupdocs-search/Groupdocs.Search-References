---
title: "MetadataIndexingOptions"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Stellt Optionen für die Indexierung von Metadatenfeldern bereit."
type: docs
weight: 1020
url: /de/net/groupdocs.search.options/metadataindexingoptions/
---
## MetadataIndexingOptions class

Stellt Optionen für die Indexierung von Metadatenfeldern bereit.

```csharp
public class MetadataIndexingOptions
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [DefaultFieldName](../../groupdocs.search.options/metadataindexingoptions/defaultfieldname) { get; set; } | Liest oder setzt den Standardfeldnamen, der zum Indizieren leerer Feldnamen verwendet wird. Der Standardwert ist `\"unknown\"`. |
| [IndexingEmptyNames](../../groupdocs.search.options/metadataindexingoptions/indexingemptynames) { get; set; } | Liest oder setzt einen Wert, der angibt, ob leere Feldnamen indiziert werden sollen oder nicht. Der Standardwert ist `true`. |
| [IndexingEmptyValues](../../groupdocs.search.options/metadataindexingoptions/indexingemptyvalues) { get; set; } | Liest oder setzt einen Wert, der angibt, ob leere Feldwerte indiziert werden sollen oder nicht. Der Standardwert ist `true`. |
| [MaxBytesToIndexField](../../groupdocs.search.options/metadataindexingoptions/maxbytestoindexfield) { get; set; } | Liest oder setzt die maximale Anzahl von Werten in einem Array vom Typ byte, die für das Indizieren des Feldes verwendet werden. Der Standardwert ist `int.MaxValue`. |
| [MaxDoublesToIndexField](../../groupdocs.search.options/metadataindexingoptions/maxdoublestoindexfield) { get; set; } | Liest oder setzt die maximale Anzahl von Werten in einem Array vom Typ double, die für das Indizieren des Feldes verwendet werden. Der Standardwert ist `int.MaxValue`. |
| [MaxIntsToIndexField](../../groupdocs.search.options/metadataindexingoptions/maxintstoindexfield) { get; set; } | Liest oder setzt die maximale Anzahl von Werten in einem Array vom Typ int, die für das Indizieren des Feldes verwendet werden. Der Standardwert ist `int.MaxValue`. |
| [MaxLongsToIndexField](../../groupdocs.search.options/metadataindexingoptions/maxlongstoindexfield) { get; set; } | Liest oder setzt die maximale Anzahl von Werten in einem Array vom Typ long, die für das Indizieren des Feldes verwendet werden. Der Standardwert ist `int.MaxValue`. |
| [SeparatorBetweenValues](../../groupdocs.search.options/metadataindexingoptions/separatorbetweenvalues) { get; set; } | Liest oder setzt das Trennzeichen zwischen Werten in einem Feld vom Typ Array. Der Standardwert ist das Leerzeichen. |
| [SeparatorInCompoundName](../../groupdocs.search.options/metadataindexingoptions/separatorincompoundname) { get; set; } | Liest oder setzt das Trennzeichen im zusammengesetzten Namen eines Feldes. Der Standardwert ist `\".\"`. |

### Hinweise

**Learn more**

* [Indexing options](https://docs.groupdocs.com/display/searchnet/Indexing+options)
* MetadataIndexingOptions are used when retrieving document text from an index: [Getting indexed documents](https://docs.groupdocs.com/display/searchnet/Getting+indexed+documents)
* MetadataIndexingOptions are used when highlighting search results: [Highlighting search results](https://docs.groupdocs.com/display/searchnet/Highlighting+search+results)

### Siehe auch

* namespace [GroupDocs.Search.Options](../../groupdocs.search.options)
* assembly [GroupDocs.Search](../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
