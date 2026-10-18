---
title: "Indexer"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Représente un service qui gère la distribution des documents indexés à travers les fragments du réseau de recherche."
type: docs
weight: 1480
url: /fr/net/groupdocs.search.scaling/indexer/
---
## Indexer class

Représente un service qui gère la distribution des documents indexés à travers les fragments du réseau de recherche.

```csharp
public sealed class Indexer
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Status](../../groupdocs.search.scaling/indexer/status) { get; } | Obtient le statut actuel du réseau de recherche. |

## Méthodes

| Nom | Description |
| --- | --- |
| [Add](../../groupdocs.search.scaling/indexer/add#add_1)(IList&lt;ExtractedData&gt;, IndexingOptions) | Effectue une opération d'indexation. Ajoute les données extraites au réseau de recherche. |
| [Add](../../groupdocs.search.scaling/indexer/add#add)(IList&lt;Document&gt;, IList&lt;string&gt;, IndexingOptions) | Effectue une opération d'indexation. L'indexation uniquement à partir du flux et de la structure est prise en charge. |
| [ChangeAttributes](../../groupdocs.search.scaling/indexer/changeattributes)(AttributeChangeBatch, ChangeAttributesOptions) | Applique le lot spécifié de modifications d'attributs aux documents indexés sans réindexation. |
| [Delete](../../groupdocs.search.scaling/indexer/delete)(string[], DeleteOptions) | Supprime les documents indexés. |
| [DeleteAllData](../../groupdocs.search.scaling/indexer/deletealldata)() | Supprime toutes les données indexées de toutes les partitions du réseau de recherche. |
| [Extract](../../groupdocs.search.scaling/indexer/extract)(IList&lt;Document&gt;, IList&lt;string&gt;, IndexingOptions) | Extrait les données des documents. |
| [GetAliasDictionary](../../groupdocs.search.scaling/indexer/getaliasdictionary)(int) | Obtient le dictionnaire d'alias. |
| [GetAlphabet](../../groupdocs.search.scaling/indexer/getalphabet)(int) | Obtient le dictionnaire de l'alphabet. |
| [GetAttributes](../../groupdocs.search.scaling/indexer/getattributes)(string) | Obtient tous les attributs associés au document indexé spécifié. |
| [GetCharacterReplacementDictionary](../../groupdocs.search.scaling/indexer/getcharacterreplacementdictionary)(int) | Obtient le dictionnaire de remplacement de caractères. |
| [GetDictionary](../../groupdocs.search.scaling/indexer/getdictionary)(DictionaryType, int) | Obtient un dictionnaire de la partition spécifiée. |
| [GetHomophoneDictionary](../../groupdocs.search.scaling/indexer/gethomophonedictionary)(int) | Obtient le dictionnaire des homophones. |
| [GetPasswordDictionary](../../groupdocs.search.scaling/indexer/getpassworddictionary)(int) | Obtient le dictionnaire des mots de passe. |
| [GetSpellingCorrector](../../groupdocs.search.scaling/indexer/getspellingcorrector)(int) | Obtient le dictionnaire du correcteur orthographique. |
| [GetStopWordDictionary](../../groupdocs.search.scaling/indexer/getstopworddictionary)(int) | Obtient le dictionnaire des mots vides. |
| [GetSynonymDictionary](../../groupdocs.search.scaling/indexer/getsynonymdictionary)(int) | Obtient le dictionnaire des synonymes. |
| [GetTokenizationDictionary](../../groupdocs.search.scaling/indexer/gettokenizationdictionary)(int) | Obtient le dictionnaire de tokenisation. |
| [Optimize](../../groupdocs.search.scaling/indexer/optimize)(OptimizeOptions) | Réduit le nombre de segments d'index en les fusionnant les uns avec les autres. Cette opération améliore les performances de recherche. |
| [SetDictionary](../../groupdocs.search.scaling/indexer/setdictionary#setdictionary)(DictionaryBase) | Définit un dictionnaire dans toutes les partitions. |
| [SetDictionary](../../groupdocs.search.scaling/indexer/setdictionary#setdictionary_1)(DictionaryBase, int) | Définit un dictionnaire dans la partition spécifiée. |
| [Synchronize](../../groupdocs.search.scaling/indexer/synchronize)(SynchronizeOptions) | Synchronise la liste des documents indexés avec ceux des partitions. Cette opération corrige les problèmes d'indexation et de suppression de documents qui résultaient de problèmes de communication avec les nœuds du réseau de recherche. |

### Voir aussi

* namespace [GroupDocs.Search.Scaling](../../groupdocs.search.scaling)
* assembly [GroupDocs.Search](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
