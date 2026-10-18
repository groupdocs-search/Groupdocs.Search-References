---
title: "HomophoneDictionary"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Stellt ein Wörterbuch heterographischer Homophone dar."
type: docs
weight: 460
url: /de/net/groupdocs.search.dictionaries/homophonedictionary/
---
## HomophoneDictionary class

Stellt ein Wörterbuch heterographischer Homophone dar.

```csharp
public class HomophoneDictionary : DictionaryBase, IEnumerable<string>
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Count](../../groupdocs.search.dictionaries/homophonedictionary/count) { get; } | Ermittelt die Anzahl der Wörter, die in diesem [`HomophoneDictionary`](../homophonedictionary) enthalten sind. |
| override [DictionaryType](../../groupdocs.search.dictionaries/homophonedictionary/dictionarytype) { get; } | Ermittelt den Wörterbuchtyp. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [AddRange](../../groupdocs.search.dictionaries/homophonedictionary/addrange#addrange)(IEnumerable&lt;string[]&gt;) | Fügt die angegebene Sammlung von Homophon-Gruppen zu dieser Instanz des [`HomophoneDictionary`](../homophonedictionary) hinzu. |
| [AddRange](../../groupdocs.search.dictionaries/homophonedictionary/addrange#addrange_1)(string[][]) | Fügt die angegebene Sammlung von Homophon-Gruppen zu dieser Instanz des [`HomophoneDictionary`](../homophonedictionary) hinzu. |
| override [Clear](../../groupdocs.search.dictionaries/homophonedictionary/clear)() | Entfernt alle Wörter aus einem [`HomophoneDictionary`](../homophonedictionary)-Objekt. |
| [ExportDictionary](../../groupdocs.search.dictionaries/dictionarybase/exportdictionary)(string) | Exportiert das Wörterbuch in eine Datei mit dem angegebenen Namen. |
| [GetAllHomophoneGroups](../../groupdocs.search.dictionaries/homophonedictionary/getallhomophonegroups)() | Liefert alle Gruppen von Homophonen, die in diesem Wörterbuch enthalten sind. |
| [GetEnumerator](../../groupdocs.search.dictionaries/homophonedictionary/getenumerator)() | Gibt einen Enumerator zurück, der die Sammlung durchläuft. |
| [GetHomophoneGroups](../../groupdocs.search.dictionaries/homophonedictionary/gethomophonegroups)(string) | Liefert alle Gruppen von Homophonen, zu denen das angegebene Wort gehört. |
| [GetHomophones](../../groupdocs.search.dictionaries/homophonedictionary/gethomophones)(string) | Liefert die Homophone für das angegebene Wort. Das resultierende Array enthält das ursprüngliche Wort nicht. |
| [ImportDictionary](../../groupdocs.search.dictionaries/dictionarybase/importdictionary)(string) | Importiert ein Wörterbuch aus der angegebenen Datei. |

### Hinweise

**Learn more**

* [Homophone search](https://docs.groupdocs.com/display/searchnet/Homophone+search)
* [Managing homophone dictionary](https://docs.groupdocs.com/display/searchnet/Homophone+dictionary)

### Siehe auch

* class [DictionaryBase](../dictionarybase)
* namespace [GroupDocs.Search.Dictionaries](../../groupdocs.search.dictionaries)
* assembly [GroupDocs.Search](../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
