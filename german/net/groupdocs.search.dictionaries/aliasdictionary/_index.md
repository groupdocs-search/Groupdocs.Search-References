---
title: "AliasDictionary"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Stellt ein Wörterbuch von Aliasen dar."
type: docs
weight: 360
url: /de/net/groupdocs.search.dictionaries/aliasdictionary/
---
## AliasDictionary class

Stellt ein Wörterbuch von Aliasen dar.

```csharp
public class AliasDictionary : DictionaryBase, IEnumerable<string>
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Count](../../groupdocs.search.dictionaries/aliasdictionary/count) { get; } | Ermittelt die Anzahl der Aliasse, die im [`AliasDictionary`](../aliasdictionary) enthalten sind. |
| override [DictionaryType](../../groupdocs.search.dictionaries/aliasdictionary/dictionarytype) { get; } | Ermittelt den Wörterbuchtyp. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Add](../../groupdocs.search.dictionaries/aliasdictionary/add)(string, string) | Fügt das angegebene Alias‑Text‑Paar zu dieser Instanz des [`AliasDictionary`](../aliasdictionary) hinzu. |
| [AddRange](../../groupdocs.search.dictionaries/aliasdictionary/addrange#addrange)(AliasReplacementPair[]) | Fügt die angegebene Sammlung von Alias‑Ersetzungs‑Paaren zu dieser Instanz des [`AliasDictionary`](../aliasdictionary) hinzu. |
| [AddRange](../../groupdocs.search.dictionaries/aliasdictionary/addrange#addrange_1)(IEnumerable&lt;AliasReplacementPair&gt;) | Fügt die angegebene Sammlung von Alias‑Ersetzungs‑Paaren zu dieser Instanz des [`AliasDictionary`](../aliasdictionary) hinzu. |
| [AddRange](../../groupdocs.search.dictionaries/aliasdictionary/addrange#addrange_2)(IEnumerable&lt;KeyValuePair&lt;string, string&gt;&gt;) | Fügt die angegebene Sammlung von Alias‑Ersetzungs‑Paaren zu dieser Instanz des [`AliasDictionary`](../aliasdictionary) hinzu. |
| override [Clear](../../groupdocs.search.dictionaries/aliasdictionary/clear)() | Entfernt alle Aliasse aus einem [`AliasDictionary`](../aliasdictionary)-Objekt. |
| [Contains](../../groupdocs.search.dictionaries/aliasdictionary/contains)(string) | Bestimmt, ob ein [`AliasDictionary`](../aliasdictionary)-Objekt das angegebene Alias enthält. |
| [ExportDictionary](../../groupdocs.search.dictionaries/dictionarybase/exportdictionary)(string) | Exportiert das Wörterbuch in eine Datei mit dem angegebenen Namen. |
| [GetEnumerator](../../groupdocs.search.dictionaries/aliasdictionary/getenumerator)() | Gibt einen Enumerator zurück, der die Sammlung durchläuft. |
| [GetText](../../groupdocs.search.dictionaries/aliasdictionary/gettext)(string) | Gibt einen Text zurück, der dem angegebenen Alias zugeordnet ist. |
| [ImportDictionary](../../groupdocs.search.dictionaries/dictionarybase/importdictionary)(string) | Importiert ein Wörterbuch aus der angegebenen Datei. |
| [Remove](../../groupdocs.search.dictionaries/aliasdictionary/remove)(string) | Entfernt das angegebene Alias aus einem [`AliasDictionary`](../aliasdictionary)-Objekt. |

### Hinweise

**Learn more**

* [Using aliases](https://docs.groupdocs.com/display/searchnet/Using+aliases)
* [Managing alias dictionary](https://docs.groupdocs.com/display/searchnet/Alias+dictionary)

### Siehe auch

* class [DictionaryBase](../dictionarybase)
* namespace [GroupDocs.Search.Dictionaries](../../groupdocs.search.dictionaries)
* assembly [GroupDocs.Search](../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
