---
title: "StopWordDictionary"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Représente un dictionnaire de mots vides."
type: docs
weight: 500
url: /fr/net/groupdocs.search.dictionaries/stopworddictionary/
---
## StopWordDictionary class

Représente un dictionnaire de mots vides.

```csharp
public class StopWordDictionary : DictionaryBase, IEnumerable<string>
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Count](../../groupdocs.search.dictionaries/stopworddictionary/count) { get; } | Obtient le nombre de mots vides contenus dans le [`StopWordDictionary`](../stopworddictionary). |
| override [DictionaryType](../../groupdocs.search.dictionaries/stopworddictionary/dictionarytype) { get; } | Obtient le type du dictionnaire. |

## Méthodes

| Nom | Description |
| --- | --- |
| [AddRange](../../groupdocs.search.dictionaries/stopworddictionary/addrange#addrange)(IEnumerable&lt;string&gt;) | Ajoute la collection spécifiée de mots à cette instance du [`StopWordDictionary`](../stopworddictionary). |
| [AddRange](../../groupdocs.search.dictionaries/stopworddictionary/addrange#addrange_1)(string[]) | Ajoute la collection spécifiée de mots à cette instance du [`StopWordDictionary`](../stopworddictionary). |
| override [Clear](../../groupdocs.search.dictionaries/stopworddictionary/clear)() | Supprime tous les mots d'un objet [`StopWordDictionary`](../stopworddictionary). |
| [Contains](../../groupdocs.search.dictionaries/stopworddictionary/contains)(string) | Détermine si un objet [`StopWordDictionary`](../stopworddictionary) contient le mot spécifié. |
| [ExportDictionary](../../groupdocs.search.dictionaries/dictionarybase/exportdictionary)(string) | Exporte le dictionnaire vers un fichier avec le nom spécifié. |
| [GetEnumerator](../../groupdocs.search.dictionaries/stopworddictionary/getenumerator)() | Renvoie un énumérateur qui parcourt la collection. |
| [ImportDictionary](../../groupdocs.search.dictionaries/dictionarybase/importdictionary)(string) | Importe un dictionnaire depuis le fichier spécifié. |
| [RemoveRange](../../groupdocs.search.dictionaries/stopworddictionary/removerange#removerange)(IEnumerable&lt;string&gt;) | Supprime la collection spécifiée de mots de cette instance du [`StopWordDictionary`](../stopworddictionary). |
| [RemoveRange](../../groupdocs.search.dictionaries/stopworddictionary/removerange#removerange_1)(string[]) | Supprime la collection spécifiée de mots de cette instance du [`StopWordDictionary`](../stopworddictionary). |

### Remarques

**Learn more**

* [Indexing with stop words](https://docs.groupdocs.com/display/searchnet/Indexing+with+stop+words)
* [Managing stop word dictionary](https://docs.groupdocs.com/display/searchnet/Stop+word+dictionary)

### Voir aussi

* class [DictionaryBase](../dictionarybase)
* namespace [GroupDocs.Search.Dictionaries](../../groupdocs.search.dictionaries)
* assembly [GroupDocs.Search](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
