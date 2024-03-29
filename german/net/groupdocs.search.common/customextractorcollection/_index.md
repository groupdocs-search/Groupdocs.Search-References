---
title: CustomExtractorCollection
second_title: GroupDocs.Suche nach .NET-API-Referenz
description: Enthält eine Sammlung benutzerdefinierter Extraktoren. Wenn die Sammlung einen Extraktor für eine Dateierweiterung enthält die von integrierten Extraktoren abgedeckt wird wird dieser Extraktor anstelle des integrierten Extraktors verwendet.
type: docs
weight: 40
url: /de/net/groupdocs.search.common/customextractorcollection/
---
## CustomExtractorCollection class

Enthält eine Sammlung benutzerdefinierter Extraktoren. Wenn die Sammlung einen Extraktor für eine Dateierweiterung enthält, die von integrierten Extraktoren abgedeckt wird, wird dieser Extraktor anstelle des integrierten Extraktors verwendet.

```csharp
public class CustomExtractorCollection : ICollection<IFieldExtractor>
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Count](../../groupdocs.search.common/customextractorcollection/count) { get; } | Ruft die Anzahl der in der Sammlung enthaltenen Extraktoren ab. |
| [IsReadOnly](../../groupdocs.search.common/customextractorcollection/isreadonly) { get; } | Ruft einen Wert ab, der angibt, ob die Sammlung schreibgeschützt ist. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Add](../../groupdocs.search.common/customextractorcollection/add)(IFieldExtractor) | Fügt der Sammlung einen Extraktor hinzu. |
| [Clear](../../groupdocs.search.common/customextractorcollection/clear)() | Entfernt alle Extraktoren aus der Sammlung. |
| [Contains](../../groupdocs.search.common/customextractorcollection/contains)(IFieldExtractor) | Bestimmt, ob die Sammlung einen bestimmten Extraktor enthält. |
| [CopyTo](../../groupdocs.search.common/customextractorcollection/copyto)(IFieldExtractor[], int) | Kopiert die Elemente der Sammlung in ein Array, beginnend bei einem bestimmten Array-Index. |
| [GetEnumerator](../../groupdocs.search.common/customextractorcollection/getenumerator)() | Gibt einen Enumerator für diese Sammlung zurück. |
| [Remove](../../groupdocs.search.common/customextractorcollection/remove)(IFieldExtractor) | Entfernt einen Extraktor aus der Sammlung. |

### Bemerkungen

**Erfahren Sie mehr**

* [Benutzerdefinierte Textextraktoren](https://docs.groupdocs.com/display/searchnet/Custom+text+extractors)

### Siehe auch

* interface [IFieldExtractor](../ifieldextractor)
* namensraum [GroupDocs.Search.Common](../../groupdocs.search.common)
* Montage [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
