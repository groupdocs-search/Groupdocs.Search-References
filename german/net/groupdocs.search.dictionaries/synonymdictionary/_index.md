---
title: "SynonymDictionary"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Stellt ein Synonymwörterbuch dar."
type: docs
weight: 510
url: /de/net/groupdocs.search.dictionaries/synonymdictionary/
---
## SynonymDictionary class

Stellt ein Synonymwörterbuch dar.

```csharp
public class SynonymDictionary : DictionaryBase, IEnumerable<string>
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Count](../../groupdocs.search.dictionaries/synonymdictionary/count) { get; } | Ermittelt die Anzahl der Wörter, die in diesem [`SynonymDictionary`](../synonymdictionary) enthalten sind. |
| override [DictionaryType](../../groupdocs.search.dictionaries/synonymdictionary/dictionarytype) { get; } | Ermittelt den Wörterbuchtyp. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [AddRange](../../groupdocs.search.dictionaries/synonymdictionary/addrange#addrange)(IEnumerable&lt;string[]&gt;) | Fügt die angegebene Sammlung von Synonymgruppen zu dieser Instanz des [`SynonymDictionary`](../synonymdictionary) hinzu. |
| [AddRange](../../groupdocs.search.dictionaries/synonymdictionary/addrange#addrange_1)(string[][]) | Fügt die angegebene Sammlung von Synonymgruppen zu dieser Instanz des [`SynonymDictionary`](../synonymdictionary) hinzu. |
| override [Clear](../../groupdocs.search.dictionaries/synonymdictionary/clear)() | Entfernt alle Wörter aus diesem [`SynonymDictionary`](../synonymdictionary)-Objekt. |
| [ExportDictionary](../../groupdocs.search.dictionaries/dictionarybase/exportdictionary)(string) | Exportiert das Wörterbuch in eine Datei mit dem angegebenen Namen. |
| [GetAllSynonymGroups](../../groupdocs.search.dictionaries/synonymdictionary/getallsynonymgroups)() | Gibt alle Synonymgruppen zurück, die in diesem Wörterbuch enthalten sind. |
| [GetEnumerator](../../groupdocs.search.dictionaries/synonymdictionary/getenumerator)() | Gibt einen Enumerator zurück, der die Sammlung durchläuft. |
| [GetSynonymGroups](../../groupdocs.search.dictionaries/synonymdictionary/getsynonymgroups)(string) | Gibt alle Synonymgruppen zurück, zu denen das angegebene Wort gehört. |
| [GetSynonyms](../../groupdocs.search.dictionaries/synonymdictionary/getsynonyms)(string) | Gibt die Synonyme für das angegebene Wort zurück. Das resultierende Array enthält das ursprüngliche Wort nicht. |
| [ImportDictionary](../../groupdocs.search.dictionaries/dictionarybase/importdictionary)(string) | Importiert ein Wörterbuch aus der angegebenen Datei. |

### Hinweise

**Learn more**

* [Synonym search](https://docs.groupdocs.com/display/searchnet/Synonym+search)
* [Managing synonym dictionary](https://docs.groupdocs.com/display/searchnet/Synonym+dictionary)

### Siehe auch

* class [DictionaryBase](../dictionarybase)
* namespace [GroupDocs.Search.Dictionaries](../../groupdocs.search.dictionaries)
* assembly [GroupDocs.Search](../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
