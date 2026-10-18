---
title: "Alphabet"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Représente un dictionnaire de caractères utilisé lors de l'indexation pour détecter le type de caractère. Chaque caractère peut être traité comme séparateur, comme lettre ou les deux."
type: docs
weight: 380
url: /fr/net/groupdocs.search.dictionaries/alphabet/
---
## Alphabet class

Représente un dictionnaire de caractères utilisé lors de l'indexation pour détecter le type de caractère. Chaque caractère peut être traité comme séparateur, comme lettre, ou les deux.

```csharp
public class Alphabet : DictionaryBase, IEnumerable<int>
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Count](../../groupdocs.search.dictionaries/alphabet/count) { get; } | Obtient le nombre de caractères contenus dans le [`Alphabet`](../alphabet). |
| override [DictionaryType](../../groupdocs.search.dictionaries/alphabet/dictionarytype) { get; } | Obtient le type du dictionnaire. |

## Méthodes

| Nom | Description |
| --- | --- |
| override [Clear](../../groupdocs.search.dictionaries/alphabet/clear)() | Définit le type de séparateur pour tous les caractères de ce [`Alphabet`](../alphabet). |
| [ExportDictionary](../../groupdocs.search.dictionaries/dictionarybase/exportdictionary)(string) | Exporte le dictionnaire vers un fichier avec le nom spécifié. |
| [GetCharacterType](../../groupdocs.search.dictionaries/alphabet/getcharactertype#getcharactertype)(char) | Obtient le type d'un caractère. |
| [GetCharacterType](../../groupdocs.search.dictionaries/alphabet/getcharactertype#getcharactertype_1)(int) | Obtient le type d'un point de code Unicode. |
| [GetCharacterType](../../groupdocs.search.dictionaries/alphabet/getcharactertype#getcharactertype_2)(string) | Obtient le type d'un caractère. Cette méthode peut être utilisée pour obtenir le type d'une paire de caractères de substitution. |
| [GetEnumerator](../../groupdocs.search.dictionaries/alphabet/getenumerator)() | Renvoie un énumérateur qui parcourt la collection. |
| [ImportDictionary](../../groupdocs.search.dictionaries/dictionarybase/importdictionary)(string) | Importe un dictionnaire depuis le fichier spécifié. |
| [SetRange](../../groupdocs.search.dictionaries/alphabet/setrange#setrange)(char[], CharacterType) | Définit le type pour chaque caractère de la collection spécifiée dans cette instance du [`Alphabet`](../alphabet). |
| [SetRange](../../groupdocs.search.dictionaries/alphabet/setrange#setrange_1)(int[], CharacterType) | Définit le type pour chaque caractère de la collection spécifiée dans cette instance du [`Alphabet`](../alphabet). |
| [SetRange](../../groupdocs.search.dictionaries/alphabet/setrange#setrange_2)(string[], CharacterType) | Définit le type pour chaque caractère de la collection spécifiée dans cette instance du [`Alphabet`](../alphabet). |

### Remarques

**Learn more**

* [Character types](https://docs.groupdocs.com/display/searchnet/Character+types)
* [Managing alphabet](https://docs.groupdocs.com/display/searchnet/Alphabet)

### Voir aussi

* class [DictionaryBase](../dictionarybase)
* namespace [GroupDocs.Search.Dictionaries](../../groupdocs.search.dictionaries)
* assembly [GroupDocs.Search](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
