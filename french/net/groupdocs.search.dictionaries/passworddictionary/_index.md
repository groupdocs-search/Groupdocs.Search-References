---
title: "PasswordDictionary"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Représente un dictionnaire de mots de passe de documents."
type: docs
weight: 480
url: /fr/net/groupdocs.search.dictionaries/passworddictionary/
---
## PasswordDictionary class

Représente un dictionnaire de mots de passe de documents.

```csharp
public class PasswordDictionary : DictionaryBase, IEnumerable<string>
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Count](../../groupdocs.search.dictionaries/passworddictionary/count) { get; } | Obtient le nombre d'éléments contenus dans le dictionnaire. |
| override [DictionaryType](../../groupdocs.search.dictionaries/passworddictionary/dictionarytype) { get; } | Obtient le type du dictionnaire. |

## Méthodes

| Nom | Description |
| --- | --- |
| [Add](../../groupdocs.search.dictionaries/passworddictionary/add)(string, string) | Ajoute un mot de passe pour un document au dictionnaire. |
| override [Clear](../../groupdocs.search.dictionaries/passworddictionary/clear)() | Supprime tous les mots de passe de cet objet [`PasswordDictionary`](../passworddictionary). |
| [Contains](../../groupdocs.search.dictionaries/passworddictionary/contains)(string) | Détermine si le dictionnaire contient un mot de passe pour le document spécifié. |
| [ExportDictionary](../../groupdocs.search.dictionaries/dictionarybase/exportdictionary)(string) | Exporte le dictionnaire vers un fichier avec le nom spécifié. |
| [GetEnumerator](../../groupdocs.search.dictionaries/passworddictionary/getenumerator)() | Renvoie un énumérateur qui parcourt la collection. |
| [GetPassword](../../groupdocs.search.dictionaries/passworddictionary/getpassword)(string) | Obtient le mot de passe du fichier. |
| [ImportDictionary](../../groupdocs.search.dictionaries/dictionarybase/importdictionary)(string) | Importe un dictionnaire depuis le fichier spécifié. |
| [Remove](../../groupdocs.search.dictionaries/passworddictionary/remove)(string) | Supprime le mot de passe du document spécifié du dictionnaire. |

### Remarques

**Learn more**

* [Indexing password protected documents](https://docs.groupdocs.com/display/searchnet/Indexing+password+protected+documents)
* [Managing document passwords](https://docs.groupdocs.com/display/searchnet/Document+passwords)

### Voir aussi

* class [DictionaryBase](../dictionarybase)
* namespace [GroupDocs.Search.Dictionaries](../../groupdocs.search.dictionaries)
* assembly [GroupDocs.Search](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
