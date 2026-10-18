---
title: "StopWordDictionary"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Stellt ein Wörterbuch von Stoppwörtern dar."
type: docs
weight: 500
url: /de/net/groupdocs.search.dictionaries/stopworddictionary/
---
## StopWordDictionary class

Stellt ein Wörterbuch von Stoppwörtern dar.

```csharp
public class StopWordDictionary : DictionaryBase, IEnumerable<string>
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Count](../../groupdocs.search.dictionaries/stopworddictionary/count) { get; } | Ermittelt die Anzahl der Stoppwörter, die im [`StopWordDictionary`](../stopworddictionary) enthalten sind. |
| override [DictionaryType](../../groupdocs.search.dictionaries/stopworddictionary/dictionarytype) { get; } | Ermittelt den Wörterbuchtyp. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [AddRange](../../groupdocs.search.dictionaries/stopworddictionary/addrange#addrange)(IEnumerable&lt;string&gt;) | Fügt die angegebene Sammlung von Wörtern zu dieser Instanz des [`StopWordDictionary`](../stopworddictionary) hinzu. |
| [AddRange](../../groupdocs.search.dictionaries/stopworddictionary/addrange#addrange_1)(string[]) | Fügt die angegebene Sammlung von Wörtern zu dieser Instanz des [`StopWordDictionary`](../stopworddictionary) hinzu. |
| override [Clear](../../groupdocs.search.dictionaries/stopworddictionary/clear)() | Entfernt alle Wörter aus einem [`StopWordDictionary`](../stopworddictionary)-Objekt. |
| [Contains](../../groupdocs.search.dictionaries/stopworddictionary/contains)(string) | Bestimmt, ob ein [`StopWordDictionary`](../stopworddictionary)-Objekt das angegebene Wort enthält. |
| [ExportDictionary](../../groupdocs.search.dictionaries/dictionarybase/exportdictionary)(string) | Exportiert das Wörterbuch in eine Datei mit dem angegebenen Namen. |
| [GetEnumerator](../../groupdocs.search.dictionaries/stopworddictionary/getenumerator)() | Gibt einen Enumerator zurück, der die Sammlung durchläuft. |
| [ImportDictionary](../../groupdocs.search.dictionaries/dictionarybase/importdictionary)(string) | Importiert ein Wörterbuch aus der angegebenen Datei. |
| [RemoveRange](../../groupdocs.search.dictionaries/stopworddictionary/removerange#removerange)(IEnumerable&lt;string&gt;) | Entfernt die angegebene Sammlung von Wörtern aus dieser Instanz des [`StopWordDictionary`](../stopworddictionary). |
| [RemoveRange](../../groupdocs.search.dictionaries/stopworddictionary/removerange#removerange_1)(string[]) | Entfernt die angegebene Sammlung von Wörtern aus dieser Instanz des [`StopWordDictionary`](../stopworddictionary). |

### Hinweise

**Learn more**

* [Indexing with stop words](https://docs.groupdocs.com/display/searchnet/Indexing+with+stop+words)
* [Managing stop word dictionary](https://docs.groupdocs.com/display/searchnet/Stop+word+dictionary)

### Siehe auch

* class [DictionaryBase](../dictionarybase)
* namespace [GroupDocs.Search.Dictionaries](../../groupdocs.search.dictionaries)
* assembly [GroupDocs.Search](../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
