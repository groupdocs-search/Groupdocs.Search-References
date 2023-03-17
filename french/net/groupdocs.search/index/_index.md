---
title: Index
second_title: Référence de l'API GroupDocs.Search pour .NET
description: Représente la classe principale pour lindexation des documents et la recherche parmi eux.
type: docs
weight: 680
url: /fr/net/groupdocs.search/index/
---
## Index class

Représente la classe principale pour l'indexation des documents et la recherche parmi eux.

```csharp
public class Index : IDisposable
```

## Constructeurs

| Nom | La description |
| --- | --- |
| [Index](index#constructor)() | Initialise une nouvelle instance du[`Index`](../index) classe en mémoire. |
| [Index](index#constructor_1)(IndexSettings) | Initialise une nouvelle instance du[`Index`](../index) classe en mémoire avec des paramètres d'index particuliers. |
| [Index](index#constructor_2)(string) | Initialise une nouvelle instance du[`Index`](../index) class. Crée un nouvel index ou ouvre un index existant sur le disque. |
| [Index](index#constructor_3)(string, bool) | Initialise une nouvelle instance du[`Index`](../index) class. Charge un index existant à partir du disque si*overwriteIfExists* est`FAUX`; crée un nouvel index sur le disque sinon. |
| [Index](index#constructor_4)(string, IndexSettings) | Initialise une nouvelle instance du[`Index`](../index) class. Crée un nouvel index avec des paramètres particuliers ou ouvre un index existant sur le disque. |
| [Index](index#constructor_5)(string, IndexSettings, bool) | Initialise une nouvelle instance du[`Index`](../index) class. Charge un index existant à partir du disque si*overwriteIfExists* est`FAUX` ; crée un nouvel index sur le disque avec des paramètres d'index particuliers sinon. |

## Propriétés

| Nom | La description |
| --- | --- |
| [Dictionaries](../../groupdocs.search/index/dictionaries) { get; } | Obtient le référentiel de dictionnaires. |
| [Events](../../groupdocs.search/index/events) { get; } | Obtient le concentrateur d'événements pour s'abonner aux événements. |
| [IndexInfo](../../groupdocs.search/index/indexinfo) { get; } | Obtient les informations de base sur l'index. |
| [IndexSettings](../../groupdocs.search/index/indexsettings) { get; } | Obtient les paramètres d'index. |
| [Repository](../../groupdocs.search/index/repository) { get; } | Obtient l'objet de référentiel d'index si l'index y est contenu. |

## Méthodes

| Nom | La description |
| --- | --- |
| [Add](../../groupdocs.search/index/add#add_2)(string) | Effectue une opération d'indexation. Ajoute un fichier ou un dossier par un chemin absolu ou relatif. Les documents de tous les sous-dossiers seront indexés. |
| [Add](../../groupdocs.search/index/add#add_4)(string[]) | Effectue une opération d'indexation. Ajoute des fichiers ou des dossiers par un chemin absolu ou relatif. Les documents de tous les sous-dossiers seront indexés. |
| [Add](../../groupdocs.search/index/add#add)(Document[], IndexingOptions) | Effectue une opération d'indexation. Ajoute des documents à partir du système de fichiers, du flux ou de la structure. |
| [Add](../../groupdocs.search/index/add#add_1)(ExtractedData[], IndexingOptions) | Effectue l'opération d'indexation. Ajoute les données extraites à l'index. |
| [Add](../../groupdocs.search/index/add#add_3)(string, IndexingOptions) | Effectue une opération d'indexation. Ajoute un fichier ou un dossier par un chemin absolu ou relatif. Les documents de tous les sous-dossiers seront indexés. |
| [Add](../../groupdocs.search/index/add#add_5)(string[], IndexingOptions) | Effectue une opération d'indexation. Ajoute des fichiers ou des dossiers par un chemin absolu ou relatif. Les documents de tous les sous-dossiers seront indexés. |
| [ChangeAttributes](../../groupdocs.search/index/changeattributes)(AttributeChangeBatch) | Applique le lot spécifié de modifications d'attributs aux documents indexés sans réindexation pendant l'opération de mise à jour. |
| [Delete](../../groupdocs.search/index/delete#delete_1)(string[], UpdateOptions) | Supprime les fichiers ou dossiers indexés de l'index. Met ensuite à jour l'index sans supprimer les chemins. Notez qu'un document individuel ne peut pas être supprimé de l'index s'il a été ajouté à l'index dans le cadre d'un dossier. |
| [Delete](../../groupdocs.search/index/delete#delete)(UpdateOptions, string[]) | Supprime les documents indexés des flux ou des structures. Met ensuite à jour l'index sans documents supprimés. |
| [Dispose](../../groupdocs.search/index/dispose)() | Libère toutes les ressources utilisées par le[`Index`](../index) . |
| [GetAttributes](../../groupdocs.search/index/getattributes)(string) | Obtient tous les attributs associés au document indexé spécifié. |
| [GetDocumentText](../../groupdocs.search/index/getdocumenttext#getdocumenttext)(DocumentInfo, OutputAdapter) | Génère du texte au format HTML pour le document indexé et le transfère via l'adaptateur de sortie. |
| [GetDocumentText](../../groupdocs.search/index/getdocumenttext#getdocumenttext_1)(DocumentInfo, OutputAdapter, TextOptions) | Génère du texte au format HTML pour le document indexé et le transfère via l'adaptateur de sortie. |
| [GetIndexedDocumentItems](../../groupdocs.search/index/getindexeddocumentitems)(DocumentInfo) | Obtient un tableau d'éléments imbriqués du document spécifié (pour les documents conteneurs tels que ZIP, OST, PST). |
| [GetIndexedDocuments](../../groupdocs.search/index/getindexeddocuments)() | Obtient un tableau de tous les documents indexés. |
| [GetIndexedPaths](../../groupdocs.search/index/getindexedpaths)() | Obtient un tableau de chemins indexés - documents ou dossiers. |
| [GetIndexingReports](../../groupdocs.search/index/getindexingreports)() | Obtient les rapports sur les opérations d'indexation. |
| [GetSearchReports](../../groupdocs.search/index/getsearchreports)() | Obtient les rapports sur les opérations de recherche. |
| [Highlight](../../groupdocs.search/index/highlight#highlight)(FoundDocument, Highlighter) | Génère un texte au format HTML avec les termes trouvés en surbrillance. |
| [Highlight](../../groupdocs.search/index/highlight#highlight_1)(FoundDocument, Highlighter, HighlightOptions) | Génère un texte au format HTML avec les termes trouvés en surbrillance. |
| [Merge](../../groupdocs.search/index/merge#merge)(Index, MergeOptions) | Fusionne l'index spécifié dans l'index actuel. Notez que l'autre index ne sera pas modifié. |
| [Merge](../../groupdocs.search/index/merge#merge_1)(IndexRepository, MergeOptions) | Fusionne les index du référentiel d'index spécifié dans l'index actuel. Notez que les index du référentiel ne seront pas modifiés. |
| [Notify](../../groupdocs.search/index/notify)(Notification) | Passe l'objet de notification spécifié à l'index pour effectuer la notification. |
| [Optimize](../../groupdocs.search/index/optimize#optimize)() | Minimise le nombre de segments d'index en les fusionnant les uns avec les autres. Cette opération améliore les performances de recherche. |
| [Optimize](../../groupdocs.search/index/optimize#optimize_1)(MergeOptions) | Minimise le nombre de segments d'index en les fusionnant les uns avec les autres. Cette opération améliore les performances de recherche. |
| [Search](../../groupdocs.search/index/search#search_1)(SearchQuery) | Recherche dans l'index. |
| [Search](../../groupdocs.search/index/search#search_3)(string) | Recherche dans l'index. |
| [Search](../../groupdocs.search/index/search#search)(SearchImage, ImageSearchOptions) | Effectue une recherche d'image inversée dans l'index. |
| [Search](../../groupdocs.search/index/search#search_2)(SearchQuery, SearchOptions) | Recherche dans l'index. |
| [Search](../../groupdocs.search/index/search#search_4)(string, SearchOptions) | Recherche dans l'index. |
| [SearchNext](../../groupdocs.search/index/searchnext#searchnext)(ChunkSearchToken) | Continue la recherche de bloc commencée avec la méthode Search. |
| [SearchNext](../../groupdocs.search/index/searchnext#searchnext_1)(ChunkSearchToken, Cancellation) | Continue la recherche de bloc commencée avec la méthode Search. |
| [Update](../../groupdocs.search/index/update#update)() | Réindexe les documents qui ont été modifiés ou supprimés depuis la dernière mise à jour. Ajoute de nouveaux fichiers qui ont été ajoutés aux dossiers indexés. |
| [Update](../../groupdocs.search/index/update#update_1)(UpdateOptions) | Réindexe les documents qui ont été modifiés ou supprimés depuis la dernière mise à jour. Ajoute de nouveaux fichiers qui ont été ajoutés aux dossiers indexés. |

### Remarques

**Apprendre encore plus**

* [Création d'un index](https://docs.groupdocs.com/display/searchnet/Creating+an+index)
* [Indexage](https://docs.groupdocs.com/display/searchnet/Indexing)
* [Recherche](https://docs.groupdocs.com/display/searchnet/Searching)

### Exemples

L'exemple montre une utilisation typique de la classe.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

Index index = new Index(indexFolder); // Création d'un index dans le dossier spécifié
index.Add(documentsFolder); // Indexation des documents du dossier spécifié

SearchResult result = index.Search(query); // Recherche dans l'index
```

### Voir également

* espace de noms [GroupDocs.Search](../../groupdocs.search)
* Assemblée [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
