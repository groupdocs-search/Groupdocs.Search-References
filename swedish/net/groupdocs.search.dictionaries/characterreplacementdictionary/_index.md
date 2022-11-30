---
title: CharacterReplacementDictionary
second_title: GroupDocs.Search efter .NET API Reference
description: Representerar en ordbok för teckenersättning som används under indexeringsprocessen. Teckenersättning kan till exempel användas för att ta bort accenter från accenttecken eller för att göra indexokänsligt för skiftlägen.
type: docs
weight: 370
url: /sv/net/groupdocs.search.dictionaries/characterreplacementdictionary/
---
## CharacterReplacementDictionary class

Representerar en ordbok för teckenersättning som används under indexeringsprocessen. Teckenersättning kan till exempel användas för att ta bort accenter från accenttecken eller för att göra indexokänsligt för skiftlägen.

```csharp
public class CharacterReplacementDictionary : DictionaryBase, IEnumerable<char>
```

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [Count](../../groupdocs.search.dictionaries/characterreplacementdictionary/count) { get; } | Hämtar antalet tecken som ingår i detta[`CharacterReplacementDictionary`](../characterreplacementdictionary) . |

## Metoder

| namn | Beskrivning |
| --- | --- |
| [AddRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/addrange#addrange)(CharacterReplacementPair[]) | Lägger till den angivna samlingen av teckenersättningar till denna instans av[`CharacterReplacementDictionary`](../characterreplacementdictionary) . |
| [AddRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/addrange#addrange_1)(IEnumerable&lt;CharacterReplacementPair&gt;) | Lägger till den angivna samlingen av teckenersättningar till denna instans av[`CharacterReplacementDictionary`](../characterreplacementdictionary) . |
| [AddRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/addrange#addrange_2)(IEnumerable&lt;KeyValuePair&lt;char, char&gt;&gt;) | Lägger till den angivna samlingen av teckenersättningar till denna instans av[`CharacterReplacementDictionary`](../characterreplacementdictionary) . |
| [Clear](../../groupdocs.search.dictionaries/characterreplacementdictionary/clear)() | Tar bort alla teckenersättningar från en[`CharacterReplacementDictionary`](../characterreplacementdictionary) objekt. |
| [Contains](../../groupdocs.search.dictionaries/characterreplacementdictionary/contains)(char) | Bestämmer om en[`CharacterReplacementDictionary`](../characterreplacementdictionary) objektet innehåller en ersättning för det angivna tecknet. |
| [ExportDictionary](../../groupdocs.search.dictionaries/dictionarybase/exportdictionary)(string) | Exporterar ordboken till en fil med det angivna namnet. |
| [GetEnumerator](../../groupdocs.search.dictionaries/characterreplacementdictionary/getenumerator)() | Returnerar en uppräkning som itererar genom samlingen. |
| [GetReplacement](../../groupdocs.search.dictionaries/characterreplacementdictionary/getreplacement)(char) | Får en ersättning för det angivna tecknet. |
| [ImportDictionary](../../groupdocs.search.dictionaries/dictionarybase/importdictionary)(string) | Importerar en ordbok från den angivna filen. |
| [RemoveRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/removerange#removerange)(char[]) | Tar bort den angivna samlingen av teckenersättningar från denna instans av[`CharacterReplacementDictionary`](../characterreplacementdictionary) . |
| [RemoveRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/removerange#removerange_1)(IEnumerable&lt;char&gt;) | Tar bort den angivna samlingen av teckenersättningar från denna instans av[`CharacterReplacementDictionary`](../characterreplacementdictionary) . |

### Anmärkningar

**Läs mer**

* [Teckenbyte under indexering](https://docs.groupdocs.com/display/searchnet/Character+replacement+during+Indexing)
* [Hantera karaktärsersättningar](https://docs.groupdocs.com/display/searchnet/Character+replacements)

### Se även

* class [DictionaryBase](../dictionarybase)
* namnutrymme [GroupDocs.Search.Dictionaries](../../groupdocs.search.dictionaries)
* hopsättning [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->