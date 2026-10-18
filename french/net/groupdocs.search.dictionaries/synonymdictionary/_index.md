---
title: "SynonymDictionary"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Représente un dictionnaire de synonymes."
type: docs
weight: 510
url: /fr/net/groupdocs.search.dictionaries/synonymdictionary/
---
## SynonymDictionary class

Représente un dictionnaire de synonymes.

```csharp
public class SynonymDictionary : DictionaryBase, IEnumerable<string>
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Count](../../groupdocs.search.dictionaries/synonymdictionary/count) { get; } | Obtient le nombre de mots contenus dans ce [`SynonymDictionary`](../synonymdictionary). |
| override [DictionaryType](../../groupdocs.search.dictionaries/synonymdictionary/dictionarytype) { get; } | Obtient le type du dictionnaire. |

## Méthodes

| Nom | Description |
| --- | --- |
| [AddRange](../../groupdocs.search.dictionaries/synonymdictionary/addrange#addrange)(IEnumerable&lt;string[]&gt;) | Ajoute la collection spécifiée de groupes de synonymes à cette instance du [`SynonymDictionary`](../synonymdictionary). |
| [AddRange](../../groupdocs.search.dictionaries/synonymdictionary/addrange#addrange_1)(string[][]) | Ajoute la collection spécifiée de groupes de synonymes à cette instance du [`SynonymDictionary`](../synonymdictionary). |
| override [Clear](../../groupdocs.search.dictionaries/synonymdictionary/clear)() | Supprime tous les mots de cet objet [`SynonymDictionary`](../synonymdictionary). |
| [ExportDictionary](../../groupdocs.search.dictionaries/dictionarybase/exportdictionary)(string) | Exporte le dictionnaire vers un fichier avec le nom spécifié. |
| [GetAllSynonymGroups](../../groupdocs.search.dictionaries/synonymdictionary/getallsynonymgroups)() | Obtient tous les groupes de synonymes contenus dans ce dictionnaire. |
| [GetEnumerator](../../groupdocs.search.dictionaries/synonymdictionary/getenumerator)() | Renvoie un énumérateur qui parcourt la collection. |
| [GetSynonymGroups](../../groupdocs.search.dictionaries/synonymdictionary/getsynonymgroups)(string) | Obtient tous les groupes de synonymes auxquels le mot spécifié appartient. |
| [GetSynonyms](../../groupdocs.search.dictionaries/synonymdictionary/getsynonyms)(string) | Obtient les synonymes du mot spécifié. Le tableau résultant ne contient pas le mot original. |
| [ImportDictionary](../../groupdocs.search.dictionaries/dictionarybase/importdictionary)(string) | Importe un dictionnaire depuis le fichier spécifié. |

### Remarques

**Learn more**

* [Synonym search](https://docs.groupdocs.com/display/searchnet/Synonym+search)
* [Managing synonym dictionary](https://docs.groupdocs.com/display/searchnet/Synonym+dictionary)

### Voir aussi

* class [DictionaryBase](../dictionarybase)
* namespace [GroupDocs.Search.Dictionaries](../../groupdocs.search.dictionaries)
* assembly [GroupDocs.Search](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
