---
title: "Index"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Représente la classe principale pour l'indexation de documents et la recherche parmi ceux-ci."
type: docs
weight: 700
url: /fr/net/groupdocs.search/index/
---
## Index class

Représente la classe principale pour l'indexation de documents et la recherche parmi ceux-ci.

```csharp
public class Index : IDisposable
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [Index](index#constructor)() | Initialise une nouvelle instance de la classe [`Index`](../index) en mémoire. |
| [Index](index#constructor_1)(IndexSettings) | Initialise une nouvelle instance de la classe [`Index`](../index) en mémoire avec des paramètres d'index spécifiques. |
| [Index](index#constructor_2)(string) | Initialise une nouvelle instance de la classe [`Index`](../index). Crée un nouvel index ou ouvre un index existant sur le disque. |
| [Index](index#constructor_3)(string, bool) | Initialise une nouvelle instance de la classe [`Index`](../index). Charge un index existant depuis le disque si *overwriteIfExists* est `false`; crée un nouvel index sur le disque sinon. |
| [Index](index#constructor_4)(string, IndexSettings) | Initialise une nouvelle instance de la classe [`Index`](../index). Crée un nouvel index avec des paramètres particuliers ou ouvre un index existant sur le disque. |
| [Index](index#constructor_5)(string, IndexSettings, bool) | Initialise une nouvelle instance de la classe [`Index`](../index). Charge un index existant depuis le disque si *overwriteIfExists* est `false`; crée un nouvel index sur le disque avec des paramètres d'index spécifiques sinon. |

## Propriétés

| Nom | Description |
| --- | --- |
| [Dictionaries](../../groupdocs.search/index/dictionaries) { get; } | Obtient le référentiel du dictionnaire. |
| [Events](../../groupdocs.search/index/events) { get; } | Obtient le hub d'événements pour s'abonner aux événements. |
| [IndexInfo](../../groupdocs.search/index/indexinfo) { get; } | Obtient les informations de base sur l'index. |
| [IndexSettings](../../groupdocs.search/index/indexsettings) { get; } | Obtient les paramètres de l'index. |
| [Repository](../../groupdocs.search/index/repository) { get; } | Obtient l'objet du référentiel d'index si l'index y est contenu. |

## Méthodes

| Nom | Description |
| --- | --- |
| static [LoadIntoMemoryCompletely](../../groupdocs.search/index/loadintomemorycompletely#loadintomemorycompletely)(string) | Charge l'intégralité de l'index en mémoire. Toute modification de l'index n'est pas automatiquement enregistrée dans le dossier d'origine. |
| static [LoadIntoMemoryCompletely](../../groupdocs.search/index/loadintomemorycompletely#loadintomemorycompletely_1)(string, IndexSettings) | Charge l'intégralité de l'index en mémoire. Toute modification de l'index n'est pas automatiquement enregistrée dans le dossier d'origine. |
| [Add](../../groupdocs.search/index/add#add_2)(string) | Effectue une opération d'indexation. Ajoute un fichier ou un dossier via un chemin absolu ou relatif. Les documents de tous les sous‑dossiers seront indexés. |
| [Add](../../groupdocs.search/index/add#add_4)(string[]) | Effectue une opération d'indexation. Ajoute des fichiers ou des dossiers via un chemin absolu ou relatif. Les documents de tous les sous‑dossiers seront indexés. |
| [Add](../../groupdocs.search/index/add#add)(Document[], IndexingOptions) | Effectue une opération d'indexation. Ajoute des documents depuis le système de fichiers, un flux ou une structure. |
| [Add](../../groupdocs.search/index/add#add_1)(ExtractedData[], IndexingOptions) | Effectue une opération d'indexation. Ajoute les données extraites à l'index. |
| [Add](../../groupdocs.search/index/add#add_3)(string, IndexingOptions) | Effectue une opération d'indexation. Ajoute un fichier ou un dossier via un chemin absolu ou relatif. Les documents de tous les sous‑dossiers seront indexés. |
| [Add](../../groupdocs.search/index/add#add_5)(string[], IndexingOptions) | Effectue une opération d'indexation. Ajoute des fichiers ou des dossiers via un chemin absolu ou relatif. Les documents de tous les sous‑dossiers seront indexés. |
| [ChangeAttributes](../../groupdocs.search/index/changeattributes)(AttributeChangeBatch) | Applique le lot spécifié de modifications d'attributs aux documents indexés sans réindexation pendant l'opération de mise à jour. |
| [CheckSegments](../../groupdocs.search/index/checksegments)(bool) | Vérifie l'index à la recherche de fichiers de segments endommagés sur le disque. La méthode répare la fonctionnalité de l'index en présence de segments endommagés si *fixIndexFunctionality* est vrai; sinon, elle ne répare pas. |
| [Delete](../../groupdocs.search/index/delete#delete_1)(string[], UpdateOptions) | Supprime les fichiers ou dossiers indexés de l'index. Met ensuite à jour l'index sans les chemins supprimés. Notez qu'un document individuel ne peut pas être supprimé de l'index s'il a été ajouté à l'index en tant que partie d'un dossier. |
| [Delete](../../groupdocs.search/index/delete#delete)(UpdateOptions, string[]) | Supprime les documents indexés provenant de flux ou de structures. Met ensuite à jour l'index sans les documents supprimés. |
| [Dispose](../../groupdocs.search/index/dispose)() | Libère toutes les ressources utilisées par le [`Index`](../index). |
| [GetAttributes](../../groupdocs.search/index/getattributes)(string) | Obtient tous les attributs associés au document indexé spécifié. |
| [GetDocumentText](../../groupdocs.search/index/getdocumenttext#getdocumenttext)(DocumentInfo, OutputAdapter) | Génère le texte d'un document indexé et le transmet via un adaptateur de sortie. |
| [GetDocumentText](../../groupdocs.search/index/getdocumenttext#getdocumenttext_1)(DocumentInfo, OutputAdapter, TextOptions) | Génère du texte formaté en HTML pour le document indexé et le transfère via l'adaptateur de sortie. |
| [GetIndexedDocument](../../groupdocs.search/index/getindexeddocument)(string) | Obtient un document indexé par clé de document. |
| [GetIndexedDocumentItems](../../groupdocs.search/index/getindexeddocumentitems)(DocumentInfo) | Obtient un tableau d'éléments imbriqués du document spécifié (pour les documents conteneurs tels que ZIP, OST, PST). |
| [GetIndexedDocuments](../../groupdocs.search/index/getindexeddocuments)() | Obtient un tableau de tous les documents indexés. |
| [GetIndexedPaths](../../groupdocs.search/index/getindexedpaths)() | Obtient un tableau de chemins indexés - documents ou dossiers. |
| [GetIndexingReports](../../groupdocs.search/index/getindexingreports)() | Obtient les rapports sur les opérations d'indexation. |
| [GetSearchReports](../../groupdocs.search/index/getsearchreports)() | Obtient les rapports sur les opérations de recherche. |
| [Highlight](../../groupdocs.search/index/highlight#highlight)(FoundDocument, Highlighter) | Génère du texte formaté en HTML avec les termes trouvés mis en évidence. |
| [Highlight](../../groupdocs.search/index/highlight#highlight_1)(FoundDocument, Highlighter, HighlightOptions) | Génère du texte formaté en HTML avec les termes trouvés mis en évidence. |
| [Merge](../../groupdocs.search/index/merge#merge)(Index, MergeOptions) | Fusionne l'index spécifié dans l'index actuel. Notez que l'autre index ne sera pas modifié. |
| [Merge](../../groupdocs.search/index/merge#merge_1)(IndexRepository, MergeOptions) | Fusionne les index du référentiel d'index spécifié dans l'index actuel. Notez que les index du référentiel ne seront pas modifiés. |
| [Notify](../../groupdocs.search/index/notify)(Notification) | Transmet l'objet de notification spécifié à l'index pour effectuer la notification. |
| [Optimize](../../groupdocs.search/index/optimize#optimize)() | Réduit le nombre de segments d'index en les fusionnant les uns avec les autres. Cette opération améliore les performances de recherche. |
| [Optimize](../../groupdocs.search/index/optimize#optimize_1)(MergeOptions) | Réduit le nombre de segments d'index en les fusionnant les uns avec les autres. Cette opération améliore les performances de recherche. |
| [SaveTo](../../groupdocs.search/index/saveto)(string) | Enregistre l'index en mémoire sur le disque. Enregistre également l'index régulier dans un autre dossier. Ne modifie pas les paramètres de cet index. |
| [Search](../../groupdocs.search/index/search#search_1)(SearchQuery) | Recherche dans l'index. |
| [Search](../../groupdocs.search/index/search#search_3)(string) | Recherche dans l'index. |
| [Search](../../groupdocs.search/index/search#search)(SearchImage, ImageSearchOptions) | Effectue une recherche d'image inversée dans l'index. |
| [Search](../../groupdocs.search/index/search#search_2)(SearchQuery, SearchOptions) | Recherche dans l'index. |
| [Search](../../groupdocs.search/index/search#search_4)(string, SearchOptions) | Recherche dans l'index. |
| [SearchNext](../../groupdocs.search/index/searchnext#searchnext)(ChunkSearchToken) | Poursuit la recherche de fragments démarrée avec la méthode Search. |
| [SearchNext](../../groupdocs.search/index/searchnext#searchnext_1)(ChunkSearchToken, Cancellation) | Poursuit la recherche de fragments démarrée avec la méthode Search. |
| [Update](../../groupdocs.search/index/update#update)() | Ré-indexe les documents qui ont été modifiés ou supprimés depuis la dernière mise à jour. Ajoute les nouveaux fichiers qui ont été ajoutés aux dossiers indexés. |
| [Update](../../groupdocs.search/index/update#update_1)(UpdateOptions) | Ré-indexe les documents qui ont été modifiés ou supprimés depuis la dernière mise à jour. Ajoute les nouveaux fichiers qui ont été ajoutés aux dossiers indexés. |

### Remarques

**Learn more**

* [Creating an index](https://docs.groupdocs.com/display/searchnet/Creating+an+index)
* [Indexing](https://docs.groupdocs.com/display/searchnet/Indexing)
* [Searching](https://docs.groupdocs.com/display/searchnet/Searching)

### Exemples

L'exemple montre une utilisation typique de la classe.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

SearchResult result = index.Search(query); // Searching in index
```

### Voir aussi

* namespace [GroupDocs.Search](../../groupdocs.search)
* assembly [GroupDocs.Search](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
