---
title: "CharacterReplacementDictionary"
second_title: "GroupDocs.Search voor .NET API-referentie"
description: "Stelt een tekensvervangingswoordenlijst voor die wordt gebruikt tijdens het indexeerproces. Tekensvervanging kan bijvoorbeeld worden gebruikt om accenten van geaccentueerde tekens te verwijderen of om een hoofdletterongevoelige index te maken."
type: docs
weight: 390
url: /nl/net/groupdocs.search.dictionaries/characterreplacementdictionary/
---
## CharacterReplacementDictionary class

Stelt een tekenvervangingswoordenboek voor dat wordt gebruikt tijdens het indexeerproces. Tekenvervanging kan bijvoorbeeld worden gebruikt om accenten van geaccentueerde tekens te verwijderen of om een hoofdletterongevoelige index te maken.

```csharp
public class CharacterReplacementDictionary : DictionaryBase, IEnumerable<int>
```

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Count](../../groupdocs.search.dictionaries/characterreplacementdictionary/count) { get; } | Haalt het aantal Unicode-codepunten op dat in deze [`CharacterReplacementDictionary`](../characterreplacementdictionary) zit. |
| override [DictionaryType](../../groupdocs.search.dictionaries/characterreplacementdictionary/dictionarytype) { get; } | Haalt het type van het woordenboek op. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| [AddRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/addrange#addrange)(CharacterReplacementPair[]) | Voegt de opgegeven collectie van tekensvervangingen toe aan dit exemplaar van de [`CharacterReplacementDictionary`](../characterreplacementdictionary). |
| [AddRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/addrange#addrange_1)(IEnumerable&lt;CharacterReplacementPair&gt;) | Voegt de opgegeven collectie van tekensvervangingen toe aan dit exemplaar van de [`CharacterReplacementDictionary`](../characterreplacementdictionary). |
| [AddRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/addrange#addrange_2)(IEnumerable&lt;KeyValuePair&lt;char, char&gt;&gt;) | Voegt de opgegeven collectie van tekensvervangingen toe aan dit exemplaar van de [`CharacterReplacementDictionary`](../characterreplacementdictionary). |
| [AddRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/addrange#addrange_3)(IEnumerable&lt;KeyValuePair&lt;int, int&gt;&gt;) | Voegt de opgegeven collectie van Unicode-codepuntvervangingen toe aan dit exemplaar van de [`CharacterReplacementDictionary`](../characterreplacementdictionary). |
| override [Clear](../../groupdocs.search.dictionaries/characterreplacementdictionary/clear)() | Verwijdert alle tekensvervangingen uit een [`CharacterReplacementDictionary`](../characterreplacementdictionary)-object. |
| [Contains](../../groupdocs.search.dictionaries/characterreplacementdictionary/contains)(int) | Bepaalt of een [`CharacterReplacementDictionary`](../characterreplacementdictionary)-object een vervanging bevat voor het opgegeven Unicode-codepunt. |
| [ExportDictionary](../../groupdocs.search.dictionaries/dictionarybase/exportdictionary)(string) | Exporteert het woordenboek naar een bestand met de opgegeven naam. |
| [GetEnumerator](../../groupdocs.search.dictionaries/characterreplacementdictionary/getenumerator)() | Retourneert een enumerator die door de collectie iterereert. |
| [GetReplacement](../../groupdocs.search.dictionaries/characterreplacementdictionary/getreplacement)(int) | Haalt een vervanging op voor het opgegeven Unicode-codepunt. |
| [ImportDictionary](../../groupdocs.search.dictionaries/dictionarybase/importdictionary)(string) | Importeert een woordenboek uit het opgegeven bestand. |
| [RemoveRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/removerange#removerange)(char[]) | Verwijdert de opgegeven collectie van tekenvervangingen uit deze instantie van de [`CharacterReplacementDictionary`](../characterreplacementdictionary). |
| [RemoveRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/removerange#removerange_2)(IEnumerable&lt;char&gt;) | Verwijdert de opgegeven collectie van tekenvervangingen uit deze instantie van de [`CharacterReplacementDictionary`](../characterreplacementdictionary). |
| [RemoveRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/removerange#removerange_3)(IEnumerable&lt;int&gt;) | Verwijdert de opgegeven collectie van Unicode-codepuntvervangingen uit deze instantie van de [`CharacterReplacementDictionary`](../characterreplacementdictionary). |
| [RemoveRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/removerange#removerange_1)(int[]) | Verwijdert de opgegeven collectie van Unicode-codepuntvervangingen uit deze instantie van de [`CharacterReplacementDictionary`](../characterreplacementdictionary). |

### Opmerkingen

**Learn more**

* [Character replacement during Indexing](https://docs.groupdocs.com/display/searchnet/Character+replacement+during+Indexing)
* [Managing character replacements](https://docs.groupdocs.com/display/searchnet/Character+replacements)

### Zie ook

* class [DictionaryBase](../dictionarybase)
* namespace [GroupDocs.Search.Dictionaries](../../groupdocs.search.dictionaries)
* assembly [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.search.dll -->
