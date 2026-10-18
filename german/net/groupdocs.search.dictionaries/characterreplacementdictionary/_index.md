---
title: "CharacterReplacementDictionary"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Stellt ein Zeichenersetzungswörterbuch dar, das während des Indexierungsprozesses verwendet wird. Zeichenersetzung kann beispielsweise verwendet werden, um Akzente von Zeichen zu entfernen oder einen case‑insensitiven Index zu erstellen."
type: docs
weight: 390
url: /de/net/groupdocs.search.dictionaries/characterreplacementdictionary/
---
## CharacterReplacementDictionary class

Stellt ein Zeichenersetzungswörterbuch dar, das während des Indexierungsvorgangs verwendet wird. Zeichenersetzung kann beispielsweise dazu genutzt werden, Akzente von Zeichen zu entfernen oder einen case‑insensitiven Index zu erstellen.

```csharp
public class CharacterReplacementDictionary : DictionaryBase, IEnumerable<int>
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Count](../../groupdocs.search.dictionaries/characterreplacementdictionary/count) { get; } | Ermittelt die Anzahl der Unicode-Codepunkte, die in diesem [`CharacterReplacementDictionary`](../characterreplacementdictionary) enthalten sind. |
| override [DictionaryType](../../groupdocs.search.dictionaries/characterreplacementdictionary/dictionarytype) { get; } | Ermittelt den Wörterbuchtyp. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [AddRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/addrange#addrange)(CharacterReplacementPair[]) | Fügt die angegebene Sammlung von Zeichenersetzungen zu dieser Instanz des [`CharacterReplacementDictionary`](../characterreplacementdictionary) hinzu. |
| [AddRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/addrange#addrange_1)(IEnumerable&lt;CharacterReplacementPair&gt;) | Fügt die angegebene Sammlung von Zeichenersetzungen zu dieser Instanz des [`CharacterReplacementDictionary`](../characterreplacementdictionary) hinzu. |
| [AddRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/addrange#addrange_2)(IEnumerable&lt;KeyValuePair&lt;char, char&gt;&gt;) | Fügt die angegebene Sammlung von Zeichenersetzungen zu dieser Instanz des [`CharacterReplacementDictionary`](../characterreplacementdictionary) hinzu. |
| [AddRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/addrange#addrange_3)(IEnumerable&lt;KeyValuePair&lt;int, int&gt;&gt;) | Fügt die angegebene Sammlung von Unicode-Codepunkt‑Ersetzungen zu dieser Instanz des [`CharacterReplacementDictionary`](../characterreplacementdictionary) hinzu. |
| override [Clear](../../groupdocs.search.dictionaries/characterreplacementdictionary/clear)() | Entfernt alle Zeichenersetzungen aus einem [`CharacterReplacementDictionary`](../characterreplacementdictionary)-Objekt. |
| [Contains](../../groupdocs.search.dictionaries/characterreplacementdictionary/contains)(int) | Bestimmt, ob ein [`CharacterReplacementDictionary`](../characterreplacementdictionary)-Objekt eine Ersetzung für den angegebenen Unicode-Codepunkt enthält. |
| [ExportDictionary](../../groupdocs.search.dictionaries/dictionarybase/exportdictionary)(string) | Exportiert das Wörterbuch in eine Datei mit dem angegebenen Namen. |
| [GetEnumerator](../../groupdocs.search.dictionaries/characterreplacementdictionary/getenumerator)() | Gibt einen Enumerator zurück, der die Sammlung durchläuft. |
| [GetReplacement](../../groupdocs.search.dictionaries/characterreplacementdictionary/getreplacement)(int) | Liefert eine Ersetzung für den angegebenen Unicode-Codepunkt. |
| [ImportDictionary](../../groupdocs.search.dictionaries/dictionarybase/importdictionary)(string) | Importiert ein Wörterbuch aus der angegebenen Datei. |
| [RemoveRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/removerange#removerange)(char[]) | Entfernt die angegebene Sammlung von Zeichenersetzungen aus dieser Instanz des [`CharacterReplacementDictionary`](../characterreplacementdictionary). |
| [RemoveRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/removerange#removerange_2)(IEnumerable&lt;char&gt;) | Entfernt die angegebene Sammlung von Zeichenersetzungen aus dieser Instanz des [`CharacterReplacementDictionary`](../characterreplacementdictionary). |
| [RemoveRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/removerange#removerange_3)(IEnumerable&lt;int&gt;) | Entfernt die angegebene Sammlung von Unicode‑Codepunkt‑Ersetzungen aus dieser Instanz des [`CharacterReplacementDictionary`](../characterreplacementdictionary). |
| [RemoveRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/removerange#removerange_1)(int[]) | Entfernt die angegebene Sammlung von Unicode‑Codepunkt‑Ersetzungen aus dieser Instanz des [`CharacterReplacementDictionary`](../characterreplacementdictionary). |

### Hinweise

**Learn more**

* [Character replacement during Indexing](https://docs.groupdocs.com/display/searchnet/Character+replacement+during+Indexing)
* [Managing character replacements](https://docs.groupdocs.com/display/searchnet/Character+replacements)

### Siehe auch

* class [DictionaryBase](../dictionarybase)
* namespace [GroupDocs.Search.Dictionaries](../../groupdocs.search.dictionaries)
* assembly [GroupDocs.Search](../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
