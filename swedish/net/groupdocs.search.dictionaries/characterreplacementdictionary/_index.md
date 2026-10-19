---
title: "CharacterReplacementDictionary"
second_title: "GroupDocs.Search för .NET API-referens"
description: "Representerar en teckenersättningsordlista som används under indexeringsprocessen. Teckenersättning kan till exempel användas för att ta bort accenter från accentuerade tecken eller för att skapa ett skiftlägesokänsligt index."
type: docs
weight: 390
url: /sv/net/groupdocs.search.dictionaries/characterreplacementdictionary/
---
## CharacterReplacementDictionary class

Representerar en teckenersättningsdictionary som används under indexeringsprocessen. Teckenersättning kan exempelvis användas för att ta bort accenter från accentuerade tecken eller för att skapa ett skiftlägesokänsligt index.

```csharp
public class CharacterReplacementDictionary : DictionaryBase, IEnumerable<int>
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Count](../../groupdocs.search.dictionaries/characterreplacementdictionary/count) { get; } | Hämtar antalet Unicode-kodpunkter som finns i denna [`CharacterReplacementDictionary`](../characterreplacementdictionary). |
| override [DictionaryType](../../groupdocs.search.dictionaries/characterreplacementdictionary/dictionarytype) { get; } | Hämtar ordbokstypen. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [AddRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/addrange#addrange)(CharacterReplacementPair[]) | Lägger till den angivna samlingen av teckenersättningar till denna instans av [`CharacterReplacementDictionary`](../characterreplacementdictionary). |
| [AddRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/addrange#addrange_1)(IEnumerable&lt;CharacterReplacementPair&gt;) | Lägger till den angivna samlingen av teckenersättningar till denna instans av [`CharacterReplacementDictionary`](../characterreplacementdictionary). |
| [AddRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/addrange#addrange_2)(IEnumerable&lt;KeyValuePair&lt;char, char&gt;&gt;) | Lägger till den angivna samlingen av teckenersättningar till denna instans av [`CharacterReplacementDictionary`](../characterreplacementdictionary). |
| [AddRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/addrange#addrange_3)(IEnumerable&lt;KeyValuePair&lt;int, int&gt;&gt;) | Lägger till den angivna samlingen av Unicode-kodpunktsersättningar till denna instans av [`CharacterReplacementDictionary`](../characterreplacementdictionary). |
| override [Clear](../../groupdocs.search.dictionaries/characterreplacementdictionary/clear)() | Tar bort alla teckenersättningar från ett [`CharacterReplacementDictionary`](../characterreplacementdictionary)-objekt. |
| [Contains](../../groupdocs.search.dictionaries/characterreplacementdictionary/contains)(int) | Bestämmer om ett [`CharacterReplacementDictionary`](../characterreplacementdictionary)-objekt innehåller en ersättning för den angivna Unicode-kodpunkten. |
| [ExportDictionary](../../groupdocs.search.dictionaries/dictionarybase/exportdictionary)(string) | Exporterar ordboken till en fil med det angivna namnet. |
| [GetEnumerator](../../groupdocs.search.dictionaries/characterreplacementdictionary/getenumerator)() | Returnerar en enumerator som itererar genom samlingen. |
| [GetReplacement](../../groupdocs.search.dictionaries/characterreplacementdictionary/getreplacement)(int) | Hämtar en ersättning för den angivna Unicode-kodpunkten. |
| [ImportDictionary](../../groupdocs.search.dictionaries/dictionarybase/importdictionary)(string) | Importerar en ordbok från den angivna filen. |
| [RemoveRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/removerange#removerange)(char[]) | Tar bort den angivna samlingen av teckenersättningar från den här instansen av [`CharacterReplacementDictionary`](../characterreplacementdictionary). |
| [RemoveRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/removerange#removerange_2)(IEnumerable&lt;char&gt;) | Tar bort den angivna samlingen av teckenersättningar från den här instansen av [`CharacterReplacementDictionary`](../characterreplacementdictionary). |
| [RemoveRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/removerange#removerange_3)(IEnumerable&lt;int&gt;) | Tar bort den angivna samlingen av Unicode-kodpunkters ersättningar från den här instansen av [`CharacterReplacementDictionary`](../characterreplacementdictionary). |
| [RemoveRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/removerange#removerange_1)(int[]) | Tar bort den angivna samlingen av Unicode-kodpunkters ersättningar från den här instansen av [`CharacterReplacementDictionary`](../characterreplacementdictionary). |

### Anmärkningar

**Learn more**

* [Character replacement during Indexing](https://docs.groupdocs.com/display/searchnet/Character+replacement+during+Indexing)
* [Managing character replacements](https://docs.groupdocs.com/display/searchnet/Character+replacements)

### Se även

* class [DictionaryBase](../dictionarybase)
* namespace [GroupDocs.Search.Dictionaries](../../groupdocs.search.dictionaries)
* assembly [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.search.dll -->
