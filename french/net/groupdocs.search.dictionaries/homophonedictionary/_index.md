---
title: "HomophoneDictionary"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Représente un dictionnaire d'homophones hétérographiques."
type: docs
weight: 460
url: /fr/net/groupdocs.search.dictionaries/homophonedictionary/
---
## HomophoneDictionary class

Représente un dictionnaire d'homophones hétérographiques.

```csharp
public class HomophoneDictionary : DictionaryBase, IEnumerable<string>
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Count](../../groupdocs.search.dictionaries/homophonedictionary/count) { get; } | Obtient le nombre de mots contenus dans ce [`HomophoneDictionary`](../homophonedictionary). |
| override [DictionaryType](../../groupdocs.search.dictionaries/homophonedictionary/dictionarytype) { get; } | Obtient le type du dictionnaire. |

## Méthodes

| Nom | Description |
| --- | --- |
| [AddRange](../../groupdocs.search.dictionaries/homophonedictionary/addrange#addrange)(IEnumerable&lt;string[]&gt;) | Ajoute la collection spécifiée de groupes d'homophones à cette instance du [`HomophoneDictionary`](../homophonedictionary). |
| [AddRange](../../groupdocs.search.dictionaries/homophonedictionary/addrange#addrange_1)(string[][]) | Ajoute la collection spécifiée de groupes d'homophones à cette instance du [`HomophoneDictionary`](../homophonedictionary). |
| override [Clear](../../groupdocs.search.dictionaries/homophonedictionary/clear)() | Supprime tous les mots d'un objet [`HomophoneDictionary`](../homophonedictionary). |
| [ExportDictionary](../../groupdocs.search.dictionaries/dictionarybase/exportdictionary)(string) | Exporte le dictionnaire vers un fichier avec le nom spécifié. |
| [GetAllHomophoneGroups](../../groupdocs.search.dictionaries/homophonedictionary/getallhomophonegroups)() | Obtient tous les groupes d'homophones contenus dans ce dictionnaire. |
| [GetEnumerator](../../groupdocs.search.dictionaries/homophonedictionary/getenumerator)() | Renvoie un énumérateur qui parcourt la collection. |
| [GetHomophoneGroups](../../groupdocs.search.dictionaries/homophonedictionary/gethomophonegroups)(string) | Obtient tous les groupes d'homophones auxquels le mot spécifié appartient. |
| [GetHomophones](../../groupdocs.search.dictionaries/homophonedictionary/gethomophones)(string) | Obtient les homophones du mot spécifié. Le tableau résultant ne contient pas le mot d'origine. |
| [ImportDictionary](../../groupdocs.search.dictionaries/dictionarybase/importdictionary)(string) | Importe un dictionnaire depuis le fichier spécifié. |

### Remarques

**Learn more**

* [Homophone search](https://docs.groupdocs.com/display/searchnet/Homophone+search)
* [Managing homophone dictionary](https://docs.groupdocs.com/display/searchnet/Homophone+dictionary)

### Voir aussi

* class [DictionaryBase](../dictionarybase)
* namespace [GroupDocs.Search.Dictionaries](../../groupdocs.search.dictionaries)
* assembly [GroupDocs.Search](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
