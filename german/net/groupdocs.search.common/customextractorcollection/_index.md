---
title: "CustomExtractorCollection"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Enthält eine Sammlung benutzerdefinierter Extraktoren. Wenn die Sammlung einen Extraktor für eine Dateierweiterung enthält, die von integrierten Extraktoren abgedeckt wird, wird dieser Extraktor anstelle des integrierten verwendet."
type: docs
weight: 40
url: /de/net/groupdocs.search.common/customextractorcollection/
---
## CustomExtractorCollection class

Enthält eine Sammlung benutzerdefinierter Extraktoren. Wenn die Sammlung einen Extraktor für eine Dateierweiterung enthält, die von integrierten Extraktoren abgedeckt wird, wird dieser Extraktor anstelle des integrierten verwendet.

```csharp
public class CustomExtractorCollection : ICollection<IFieldExtractor>
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Count](../../groupdocs.search.common/customextractorcollection/count) { get; } | Liefert die Anzahl der in der Sammlung enthaltenen Extraktoren. |
| [IsReadOnly](../../groupdocs.search.common/customextractorcollection/isreadonly) { get; } | Liefert einen Wert, der angibt, ob die Sammlung schreibgeschützt ist. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Add](../../groupdocs.search.common/customextractorcollection/add)(IFieldExtractor) | Fügt der Sammlung einen Extraktor hinzu. |
| [Clear](../../groupdocs.search.common/customextractorcollection/clear)() | Entfernt alle Extraktoren aus der Sammlung. |
| [Contains](../../groupdocs.search.common/customextractorcollection/contains)(IFieldExtractor) | Bestimmt, ob die Sammlung einen bestimmten Extraktor enthält. |
| [CopyTo](../../groupdocs.search.common/customextractorcollection/copyto)(IFieldExtractor[], int) | Kopiert die Elemente der Sammlung in ein Array, beginnend an einem bestimmten Array-Index. |
| [GetEnumerator](../../groupdocs.search.common/customextractorcollection/getenumerator)() | Gibt einen Enumerator für diese Sammlung zurück. |
| [Remove](../../groupdocs.search.common/customextractorcollection/remove)(IFieldExtractor) | Entfernt einen Extraktor aus der Sammlung. |

### Hinweise

**Learn more**

* [Custom text extractors](https://docs.groupdocs.com/display/searchnet/Custom+text+extractors)

### Siehe auch

* interface [IFieldExtractor](../ifieldextractor)
* namespace [GroupDocs.Search.Common](../../groupdocs.search.common)
* assembly [GroupDocs.Search](../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
