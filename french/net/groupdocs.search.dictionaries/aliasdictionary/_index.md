---
title: "AliasDictionary"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Représente un dictionnaire d'alias."
type: docs
weight: 360
url: /fr/net/groupdocs.search.dictionaries/aliasdictionary/
---
## AliasDictionary class

Représente un dictionnaire d'alias.

```csharp
public class AliasDictionary : DictionaryBase, IEnumerable<string>
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Count](../../groupdocs.search.dictionaries/aliasdictionary/count) { get; } | Obtient le nombre d'alias contenus dans le [`AliasDictionary`](../aliasdictionary). |
| override [DictionaryType](../../groupdocs.search.dictionaries/aliasdictionary/dictionarytype) { get; } | Obtient le type du dictionnaire. |

## Méthodes

| Nom | Description |
| --- | --- |
| [Add](../../groupdocs.search.dictionaries/aliasdictionary/add)(string, string) | Ajoute la paire spécifiée d'alias et de texte associé à cette instance du [`AliasDictionary`](../aliasdictionary). |
| [AddRange](../../groupdocs.search.dictionaries/aliasdictionary/addrange#addrange)(AliasReplacementPair[]) | Ajoute la collection spécifiée de paires alias/remplacement à cette instance du [`AliasDictionary`](../aliasdictionary). |
| [AddRange](../../groupdocs.search.dictionaries/aliasdictionary/addrange#addrange_1)(IEnumerable&lt;AliasReplacementPair&gt;) | Ajoute la collection spécifiée de paires alias/remplacement à cette instance du [`AliasDictionary`](../aliasdictionary). |
| [AddRange](../../groupdocs.search.dictionaries/aliasdictionary/addrange#addrange_2)(IEnumerable&lt;KeyValuePair&lt;string, string&gt;&gt;) | Ajoute la collection spécifiée de paires alias/remplacement à cette instance du [`AliasDictionary`](../aliasdictionary). |
| override [Clear](../../groupdocs.search.dictionaries/aliasdictionary/clear)() | Supprime tous les alias d'un objet [`AliasDictionary`](../aliasdictionary). |
| [Contains](../../groupdocs.search.dictionaries/aliasdictionary/contains)(string) | Détermine si un objet [`AliasDictionary`](../aliasdictionary) contient l'alias spécifié. |
| [ExportDictionary](../../groupdocs.search.dictionaries/dictionarybase/exportdictionary)(string) | Exporte le dictionnaire vers un fichier avec le nom spécifié. |
| [GetEnumerator](../../groupdocs.search.dictionaries/aliasdictionary/getenumerator)() | Renvoie un énumérateur qui parcourt la collection. |
| [GetText](../../groupdocs.search.dictionaries/aliasdictionary/gettext)(string) | Obtient le texte associé à l'alias spécifié. |
| [ImportDictionary](../../groupdocs.search.dictionaries/dictionarybase/importdictionary)(string) | Importe un dictionnaire depuis le fichier spécifié. |
| [Remove](../../groupdocs.search.dictionaries/aliasdictionary/remove)(string) | Supprime l'alias spécifié d'un objet [`AliasDictionary`](../aliasdictionary). |

### Remarques

**Learn more**

* [Using aliases](https://docs.groupdocs.com/display/searchnet/Using+aliases)
* [Managing alias dictionary](https://docs.groupdocs.com/display/searchnet/Alias+dictionary)

### Voir aussi

* class [DictionaryBase](../dictionarybase)
* namespace [GroupDocs.Search.Dictionaries](../../groupdocs.search.dictionaries)
* assembly [GroupDocs.Search](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
