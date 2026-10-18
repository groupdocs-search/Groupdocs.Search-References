---
title: "Dokument"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Stellt die Basisklasse für Dokumente dar, die einem Index aus Dateisystem-Stream oder -Struktur hinzugefügt werden. Enthält statische Methoden zum Erstellen von Dokumenten aus verschiedenen Quelltypen."
type: docs
weight: 50
url: /de/net/groupdocs.search.common/document/
---
## Document class

Stellt die Basisklasse für Dokumente dar, die aus Dateisystem, Stream oder Struktur zu einem Index hinzugefügt werden. Enthält statische Methoden zum Erstellen von Dokumenten aus verschiedenen Quelltypen.

```csharp
public abstract class Document
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| virtual [AdditionalFields](../../groupdocs.search.common/document/additionalfields) { get; set; } | Liefert oder setzt die zusätzlichen Felder für das Dokument. |
| virtual [Attributes](../../groupdocs.search.common/document/attributes) { get; set; } | Liefert oder setzt die Attribute des Dokuments. |
| abstract [DocumentKey](../../groupdocs.search.common/document/documentkey) { get; } | Liefert den Dokumentschlüssel, der verwendet wird, um das Dokument innerhalb eines Index zu identifizieren. |
| abstract [DocumentSourceKind](../../groupdocs.search.common/document/documentsourcekind) { get; } | Liefert die Art der Dokumentquelle. |
| abstract [Extension](../../groupdocs.search.common/document/extension) { get; } | Liefert die für diesen Dokumenttyp verwendete Erweiterung. |
| abstract [IsLazy](../../groupdocs.search.common/document/islazy) { get; } | Liefert einen Wert, der angibt, ob das Dokument bei Bedarf geladen wird oder nicht. |
| abstract [ModificationDate](../../groupdocs.search.common/document/modificationdate) { get; } | Liefert das letzte Änderungsdatum des Dokuments. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| static [CreateFromFile](../../groupdocs.search.common/document/createfromfile)(string) | Erstellt ein Dokument aus einer Datei. |
| static [CreateFromStream](../../groupdocs.search.common/document/createfromstream)(string, DateTime, string, Stream) | Erstellt ein Dokument aus einem Stream. |
| static [CreateFromStructure](../../groupdocs.search.common/document/createfromstructure)(string, DateTime, DocumentField[]) | Erstellt ein Dokument aus einer Struktur, die ein Array von Textfeldern ist. |
| static [CreateLazy](../../groupdocs.search.common/document/createlazy)(DocumentSourceKind, string, IDocumentLoader) | Erstellt ein lazy-loaded Dokument. |
| override [ToString](../../groupdocs.search.common/document/tostring)() | Gibt einen String zurück, der das aktuelle [`Document`](../document) darstellt. |

### Hinweise

**Learn more**

* [Indexing from different sources](https://docs.groupdocs.com/search/net/indexing-from-different-sources/)

### Siehe auch

* namespace [GroupDocs.Search.Common](../../groupdocs.search.common)
* assembly [GroupDocs.Search](../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
