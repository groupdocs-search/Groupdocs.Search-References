---
title: "CharacterReplacementDictionary"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Représente un dictionnaire de remplacement de caractères utilisé pendant le processus d'indexation. Le remplacement de caractères peut être utilisé, par exemple, pour supprimer les accents des caractères accentués ou pour créer un index insensible à la casse."
type: docs
weight: 390
url: /fr/net/groupdocs.search.dictionaries/characterreplacementdictionary/
---
## CharacterReplacementDictionary class

Représente un dictionnaire de remplacement de caractères utilisé pendant le processus d'indexation. Le remplacement de caractères peut être utilisé, par exemple, pour supprimer les accents des caractères accentués ou pour créer un index insensible à la casse.

```csharp
public class CharacterReplacementDictionary : DictionaryBase, IEnumerable<int>
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Count](../../groupdocs.search.dictionaries/characterreplacementdictionary/count) { get; } | Obtient le nombre de points de code Unicode contenus dans ce [`CharacterReplacementDictionary`](../characterreplacementdictionary). |
| override [DictionaryType](../../groupdocs.search.dictionaries/characterreplacementdictionary/dictionarytype) { get; } | Obtient le type du dictionnaire. |

## Méthodes

| Nom | Description |
| --- | --- |
| [AddRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/addrange#addrange)(CharacterReplacementPair[]) | Ajoute la collection spécifiée de remplacements de caractères à cette instance de [`CharacterReplacementDictionary`](../characterreplacementdictionary). |
| [AddRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/addrange#addrange_1)(IEnumerable&lt;CharacterReplacementPair&gt;) | Ajoute la collection spécifiée de remplacements de caractères à cette instance de [`CharacterReplacementDictionary`](../characterreplacementdictionary). |
| [AddRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/addrange#addrange_2)(IEnumerable&lt;KeyValuePair&lt;char, char&gt;&gt;) | Ajoute la collection spécifiée de remplacements de caractères à cette instance de [`CharacterReplacementDictionary`](../characterreplacementdictionary). |
| [AddRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/addrange#addrange_3)(IEnumerable&lt;KeyValuePair&lt;int, int&gt;&gt;) | Ajoute la collection spécifiée de remplacements de points de code Unicode à cette instance de [`CharacterReplacementDictionary`](../characterreplacementdictionary). |
| override [Clear](../../groupdocs.search.dictionaries/characterreplacementdictionary/clear)() | Supprime tous les remplacements de caractères d'un objet [`CharacterReplacementDictionary`](../characterreplacementdictionary). |
| [Contains](../../groupdocs.search.dictionaries/characterreplacementdictionary/contains)(int) | Détermine si un objet [`CharacterReplacementDictionary`](../characterreplacementdictionary) contient un remplacement pour le point de code Unicode spécifié. |
| [ExportDictionary](../../groupdocs.search.dictionaries/dictionarybase/exportdictionary)(string) | Exporte le dictionnaire vers un fichier avec le nom spécifié. |
| [GetEnumerator](../../groupdocs.search.dictionaries/characterreplacementdictionary/getenumerator)() | Renvoie un énumérateur qui parcourt la collection. |
| [GetReplacement](../../groupdocs.search.dictionaries/characterreplacementdictionary/getreplacement)(int) | Obtient un remplacement pour le point de code Unicode spécifié. |
| [ImportDictionary](../../groupdocs.search.dictionaries/dictionarybase/importdictionary)(string) | Importe un dictionnaire depuis le fichier spécifié. |
| [RemoveRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/removerange#removerange)(char[]) | Supprime la collection spécifiée de remplacements de caractères de cette instance du [`CharacterReplacementDictionary`](../characterreplacementdictionary). |
| [RemoveRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/removerange#removerange_2)(IEnumerable&lt;char&gt;) | Supprime la collection spécifiée de remplacements de caractères de cette instance du [`CharacterReplacementDictionary`](../characterreplacementdictionary). |
| [RemoveRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/removerange#removerange_3)(IEnumerable&lt;int&gt;) | Supprime la collection spécifiée de remplacements de points de code Unicode de cette instance du [`CharacterReplacementDictionary`](../characterreplacementdictionary). |
| [RemoveRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/removerange#removerange_1)(int[]) | Supprime la collection spécifiée de remplacements de points de code Unicode de cette instance du [`CharacterReplacementDictionary`](../characterreplacementdictionary). |

### Remarques

**Learn more**

* [Character replacement during Indexing](https://docs.groupdocs.com/display/searchnet/Character+replacement+during+Indexing)
* [Managing character replacements](https://docs.groupdocs.com/display/searchnet/Character+replacements)

### Voir aussi

* class [DictionaryBase](../dictionarybase)
* namespace [GroupDocs.Search.Dictionaries](../../groupdocs.search.dictionaries)
* assembly [GroupDocs.Search](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
