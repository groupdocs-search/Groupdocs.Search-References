---
title: Alphabet
second_title: Référence de l'API GroupDocs.Search pour .NET
description: Représente un dictionnaire de caractères utilisé lors de lindexation pour détecter le type de caractère. Chaque caractère peut être traité comme séparateur comme lettre ou les deux.
type: docs
weight: 360
url: /fr/net/groupdocs.search.dictionaries/alphabet/
---
## Alphabet class

Représente un dictionnaire de caractères utilisé lors de l'indexation pour détecter le type de caractère. Chaque caractère peut être traité comme séparateur, comme lettre ou les deux.

```csharp
public class Alphabet : DictionaryBase, IEnumerable<char>
```

## Propriétés

| Nom | La description |
| --- | --- |
| [Count](../../groupdocs.search.dictionaries/alphabet/count) { get; } | Obtient le nombre de caractères contenus dans le[`Alphabet`](../alphabet) . |

## Méthodes

| Nom | La description |
| --- | --- |
| [Clear](../../groupdocs.search.dictionaries/alphabet/clear)() | Définit leSeparator tapez tous les caractères de ce[`Alphabet`](../alphabet) . |
| [ExportDictionary](../../groupdocs.search.dictionaries/dictionarybase/exportdictionary)(string) | Exporte le dictionnaire vers un fichier avec le nom spécifié. |
| [GetCharacterType](../../groupdocs.search.dictionaries/alphabet/getcharactertype)(char) | Obtient un type de caractère. |
| [GetEnumerator](../../groupdocs.search.dictionaries/alphabet/getenumerator)() | Renvoie un énumérateur qui parcourt la collection. |
| [ImportDictionary](../../groupdocs.search.dictionaries/dictionarybase/importdictionary)(string) | Importe un dictionnaire à partir du fichier spécifié. |
| [SetRange](../../groupdocs.search.dictionaries/alphabet/setrange)(char[], CharacterType) | Définit le type de chaque caractère de la collection spécifiée dans cette instance du[`Alphabet`](../alphabet) . |

### Remarques

**Apprendre encore plus**

* [Types de caractères](https://docs.groupdocs.com/display/searchnet/Character+types)
* [Gestion de l'alphabet](https://docs.groupdocs.com/display/searchnet/Alphabet)

### Voir également

* class [DictionaryBase](../dictionarybase)
* espace de noms [GroupDocs.Search.Dictionaries](../../groupdocs.search.dictionaries)
* Assemblée [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->