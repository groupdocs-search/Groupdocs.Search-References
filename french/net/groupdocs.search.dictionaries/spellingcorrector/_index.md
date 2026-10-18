---
title: "SpellingCorrector"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Représente un correcteur orthographique pour les termes d'une requête."
type: docs
weight: 490
url: /fr/net/groupdocs.search.dictionaries/spellingcorrector/
---
## SpellingCorrector class

Représente un correcteur orthographique pour les termes d'une requête.

```csharp
public class SpellingCorrector : DictionaryBase
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Count](../../groupdocs.search.dictionaries/spellingcorrector/count) { get; } | Obtient le nombre de mots contenus dans ce [`SpellingCorrector`](../spellingcorrector). |
| override [DictionaryType](../../groupdocs.search.dictionaries/spellingcorrector/dictionarytype) { get; } | Obtient le type du dictionnaire. |

## Méthodes

| Nom | Description |
| --- | --- |
| [AddRange](../../groupdocs.search.dictionaries/spellingcorrector/addrange#addrange)(IEnumerable&lt;string&gt;) | Ajoute la collection spécifiée de mots à cette instance du [`SpellingCorrector`](../spellingcorrector). |
| [AddRange](../../groupdocs.search.dictionaries/spellingcorrector/addrange#addrange_1)(string[]) | Ajoute la collection spécifiée de mots à cette instance du [`SpellingCorrector`](../spellingcorrector). |
| override [Clear](../../groupdocs.search.dictionaries/spellingcorrector/clear)() | Supprime tous les mots d'un objet [`SpellingCorrector`](../spellingcorrector). |
| [ExportDictionary](../../groupdocs.search.dictionaries/dictionarybase/exportdictionary)(string) | Exporte le dictionnaire vers un fichier avec le nom spécifié. |
| [GetWords](../../groupdocs.search.dictionaries/spellingcorrector/getwords)() | Obtient la collection de mots actuellement contenue dans ce [`SpellingCorrector`](../spellingcorrector). |
| [ImportDictionary](../../groupdocs.search.dictionaries/dictionarybase/importdictionary)(string) | Importe un dictionnaire depuis le fichier spécifié. |

### Remarques

**Learn more**

* [Spell checking](https://docs.groupdocs.com/display/searchnet/Spell+checking)
* [Managing spelling corrector](https://docs.groupdocs.com/display/searchnet/Spelling+corrector)

### Voir aussi

* class [DictionaryBase](../dictionarybase)
* namespace [GroupDocs.Search.Dictionaries](../../groupdocs.search.dictionaries)
* assembly [GroupDocs.Search](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
