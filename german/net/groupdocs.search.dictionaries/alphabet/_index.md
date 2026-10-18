---
title: "Alphabet"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Stellt ein Zeichenwörterbuch dar, das beim Indexieren zur Erkennung des Zeichentyps verwendet wird. Jedes Zeichen kann als Trennzeichen, als Buchstabe oder als beides behandelt werden."
type: docs
weight: 380
url: /de/net/groupdocs.search.dictionaries/alphabet/
---
## Alphabet class

Stellt ein Zeichenwörterbuch dar, das beim Indexieren zur Erkennung des Zeichentyps verwendet wird. Jedes Zeichen kann als Trennzeichen, als Buchstabe oder beides behandelt werden.

```csharp
public class Alphabet : DictionaryBase, IEnumerable<int>
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Count](../../groupdocs.search.dictionaries/alphabet/count) { get; } | Liefert die Anzahl der Zeichen, die im [`Alphabet`](../alphabet) enthalten sind. |
| override [DictionaryType](../../groupdocs.search.dictionaries/alphabet/dictionarytype) { get; } | Ermittelt den Wörterbuchtyp. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| override [Clear](../../groupdocs.search.dictionaries/alphabet/clear)() | Setzt den Trennzeichen-Typ für alle Zeichen in diesem [`Alphabet`](../alphabet). |
| [ExportDictionary](../../groupdocs.search.dictionaries/dictionarybase/exportdictionary)(string) | Exportiert das Wörterbuch in eine Datei mit dem angegebenen Namen. |
| [GetCharacterType](../../groupdocs.search.dictionaries/alphabet/getcharactertype#getcharactertype)(char) | Liefert einen Typ eines Zeichens. |
| [GetCharacterType](../../groupdocs.search.dictionaries/alphabet/getcharactertype#getcharactertype_1)(int) | Liefert einen Typ eines Unicode-Codepunkts. |
| [GetCharacterType](../../groupdocs.search.dictionaries/alphabet/getcharactertype#getcharactertype_2)(string) | Liefert einen Typ eines Zeichens. Diese Methode kann verwendet werden, um den Typ eines Surrogatpaars zu erhalten. |
| [GetEnumerator](../../groupdocs.search.dictionaries/alphabet/getenumerator)() | Gibt einen Enumerator zurück, der die Sammlung durchläuft. |
| [ImportDictionary](../../groupdocs.search.dictionaries/dictionarybase/importdictionary)(string) | Importiert ein Wörterbuch aus der angegebenen Datei. |
| [SetRange](../../groupdocs.search.dictionaries/alphabet/setrange#setrange)(char[], CharacterType) | Setzt den Typ für jedes Zeichen der angegebenen Sammlung in dieser Instanz des [`Alphabet`](../alphabet). |
| [SetRange](../../groupdocs.search.dictionaries/alphabet/setrange#setrange_1)(int[], CharacterType) | Setzt den Typ für jedes Zeichen der angegebenen Sammlung in dieser Instanz des [`Alphabet`](../alphabet). |
| [SetRange](../../groupdocs.search.dictionaries/alphabet/setrange#setrange_2)(string[], CharacterType) | Setzt den Typ für jedes Zeichen der angegebenen Sammlung in dieser Instanz des [`Alphabet`](../alphabet). |

### Hinweise

**Learn more**

* [Character types](https://docs.groupdocs.com/display/searchnet/Character+types)
* [Managing alphabet](https://docs.groupdocs.com/display/searchnet/Alphabet)

### Siehe auch

* class [DictionaryBase](../dictionarybase)
* namespace [GroupDocs.Search.Dictionaries](../../groupdocs.search.dictionaries)
* assembly [GroupDocs.Search](../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
