---
title: "Index"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Représente la classe principale pour l'indexation de documents et la recherche parmi ceux-ci."
type: docs
weight: 17
url: /fr/java/com.groupdocs.search/index/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.io.Closeable
```
public class Index implements Closeable
```

Représente la classe principale pour l'indexation de documents et la recherche parmi ceux-ci.


**Learn more**

* [Creating an index](../https://docs.groupdocs.com/display/searchjava/Creating+an+index)
* [Indexing](../https://docs.groupdocs.com/display/searchjava/Indexing)
* [Searching](../https://docs.groupdocs.com/display/searchjava/Searching)


L'exemple montre une utilisation typique de la classe.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // Création de l'index dans le dossier spécifié
index.add(documentsFolder); // Indexation des documents depuis le dossier spécifié
SearchResult result = index.search(query); // Recherche dans l'index
 
```
 
````


## Constructeurs

| Constructeur | Description |
| --- | --- |
|  | [Index()](#Index--) | Initialise une nouvelle instance de la classe Index en mémoire. |
|
|  | [Index(IndexSettings settings)](#Index-com.groupdocs.search.IndexSettings-) | Initialise une nouvelle instance de la classe Index en mémoire avec des paramètres d'index spécifiques. |
|
|  | [Index(String indexFolder)](#Index-java.lang.String-) | Initialise une nouvelle instance de la classe Index. |
|
|  | [Index(String indexFolder, IndexSettings settings)](#Index-java.lang.String-com.groupdocs.search.IndexSettings-) | Initialise une nouvelle instance de la |
Index
classe.
|
|  | [Index(String indexFolder, boolean overwriteIfExists)](#Index-java.lang.String-boolean-) | Initialise une nouvelle instance de la |
Index
classe.
|
|  | [Index(String indexFolder, IndexSettings settings, boolean overwriteIfExists)](#Index-java.lang.String-com.groupdocs.search.IndexSettings-boolean-) | Initialise une nouvelle instance de la |
Index
classe.
|
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getEvents()](#getEvents--) | Obtient le hub d'événements pour s'abonner aux événements. |
|
|  | [getIndexInfo()](#getIndexInfo--) | Obtient les informations de base sur l'index. |
|
|  | [getRepository()](#getRepository--) | Obtient l'objet du référentiel d'index si l'index y est contenu. |
|
|  | [getIndexSettings()](#getIndexSettings--) | Obtient les paramètres de l'index. |
|
|  | [getDictionaries()](#getDictionaries--) | Obtient le référentiel du dictionnaire. |
|
|  | [close()](#close--) | Libère toutes les ressources utilisées par le |
Index
.
|
|  | [add(String path)](#add-java.lang.String-) | Effectue l'opération d'indexation. |
|
|  | [add(String path, IndexingOptions options)](#add-java.lang.String-com.groupdocs.search.options.IndexingOptions-) | Effectue l'opération d'indexation. |
|
|  | [add(String[] paths)](#add-java.lang.String---) | Effectue l'opération d'indexation. |
|
|  | [add(String[] paths, IndexingOptions options)](#add-java.lang.String---com.groupdocs.search.options.IndexingOptions-) | Effectue l'opération d'indexation. |
|
|  | [add(Document[] documents, IndexingOptions options)](#add-com.groupdocs.search.Document---com.groupdocs.search.options.IndexingOptions-) | Effectue l'opération d'indexation. |
|
|  | [add(ExtractedData[] data, IndexingOptions options)](#add-com.groupdocs.search.ExtractedData---com.groupdocs.search.options.IndexingOptions-) | Effectue l'opération d'indexation. |
|
|  | [update()](#update--) | Ré-indexe les documents qui ont été modifiés ou supprimés depuis la dernière mise à jour. |
|
|  | [update(UpdateOptions options)](#update-com.groupdocs.search.options.UpdateOptions-) | Ré-indexe les documents qui ont été modifiés ou supprimés depuis la dernière mise à jour. |
|
|  | [getIndexingReports()](#getIndexingReports--) | Obtient les rapports sur les opérations d'indexation. |
|
|  | [getSearchReports()](#getSearchReports--) | Obtient les rapports sur les opérations de recherche. |
|
|  | [search(String query)](#search-java.lang.String-) | Recherche dans l'index. |
|
|  | [search(String query, SearchOptions options)](#search-java.lang.String-com.groupdocs.search.options.SearchOptions-) | Recherche dans l'index. |
|
|  | [search(SearchQuery query)](#search-com.groupdocs.search.SearchQuery-) | Recherche dans l'index. |
|
|  | [search(SearchQuery query, SearchOptions options)](#search-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-) | Recherche dans l'index. |
|
|  | [search(SearchImage image, ImageSearchOptions options)](#search-com.groupdocs.search.common.SearchImage-com.groupdocs.search.options.ImageSearchOptions-) | Effectue une recherche d'image inversée dans l'index. |
|
|  | [searchNext(ChunkSearchToken chunkSearchToken)](#searchNext-com.groupdocs.search.common.ChunkSearchToken-) | Continue la recherche par morceaux commencée avec la méthode Search. |
|
|  | [searchNext(ChunkSearchToken chunkSearchToken, Cancellation cancellation)](#searchNext-com.groupdocs.search.common.ChunkSearchToken-com.groupdocs.search.common.Cancellation-) | Continue la recherche par morceaux commencée avec la méthode Search. |
|
|  | [optimize()](#optimize--) | Réduit le nombre de segments d'index en les fusionnant les uns avec les autres. |
|
|  | [optimize(MergeOptions options)](#optimize-com.groupdocs.search.options.MergeOptions-) | Réduit le nombre de segments d'index en les fusionnant les uns avec les autres. |
|
|  | [merge(Index index, MergeOptions options)](#merge-com.groupdocs.search.Index-com.groupdocs.search.options.MergeOptions-) | Fusionne l'index spécifié dans l'index actuel. |
|
|  | [merge(IndexRepository repository, MergeOptions options)](#merge-com.groupdocs.search.IndexRepository-com.groupdocs.search.options.MergeOptions-) | Fusionne les index du référentiel d'index spécifié dans l'index actuel. |
|
|  | [highlight(FoundDocument document, Highlighter highlighter)](#highlight-com.groupdocs.search.results.FoundDocument-com.groupdocs.search.highlighters.Highlighter-) | Génère du texte formaté en HTML avec les termes trouvés mis en évidence. |
|
|  | [highlight(FoundDocument document, Highlighter highlighter, HighlightOptions options)](#highlight-com.groupdocs.search.results.FoundDocument-com.groupdocs.search.highlighters.Highlighter-com.groupdocs.search.options.HighlightOptions-) | Génère du texte formaté en HTML avec les termes trouvés mis en évidence. |
|
|  | [getIndexedDocuments()](#getIndexedDocuments--) | Obtient un tableau de tous les documents indexés. |
|
|  | [getIndexedDocumentItems(DocumentInfo documentInfo)](#getIndexedDocumentItems-com.groupdocs.search.results.DocumentInfo-) | Obtient un tableau d'éléments de document. |
|
|  | [GetIndexedDocument(String documentKey)](#GetIndexedDocument-java.lang.String-) | Obtient un document indexé par clé de document. |
|
|  | [getDocumentText(DocumentInfo documentInfo, OutputAdapter adapter)](#getDocumentText-com.groupdocs.search.results.DocumentInfo-com.groupdocs.search.common.OutputAdapter-) | Génère le texte d'un document indexé et le transmet via un adaptateur de sortie. |
|
|  | [getDocumentText(DocumentInfo documentInfo, OutputAdapter adapter, TextOptions options)](#getDocumentText-com.groupdocs.search.results.DocumentInfo-com.groupdocs.search.common.OutputAdapter-com.groupdocs.search.options.TextOptions-) | Génère du texte formaté en HTML pour le document indexé et le transfère via l'adaptateur de sortie. |
|
|  | [getIndexedPaths()](#getIndexedPaths--) | Obtient un tableau de chemins indexés - documents ou dossiers. |
|
|  | [delete(String[] paths, UpdateOptions options)](#delete-java.lang.String---com.groupdocs.search.options.UpdateOptions-) | Supprime les fichiers ou dossiers indexés de l'index. |
|
|  | [delete(UpdateOptions options, String[] documentKeys)](#delete-com.groupdocs.search.options.UpdateOptions-java.lang.String---) | Supprime les documents indexés à partir de flux ou de structures. |
|
|  | [notifyIndex(Notification notification)](#notifyIndex-com.groupdocs.search.Notification-) | Transmet l'objet de notification spécifié à l'index pour effectuer la notification. |
|
|  | [changeAttributes(AttributeChangeBatch batch)](#changeAttributes-com.groupdocs.search.common.AttributeChangeBatch-) | Applique le lot spécifié de modifications d'attributs aux documents indexés sans réindexation pendant l'opération de mise à jour. |
|
|  | [getAttributes(String path)](#getAttributes-java.lang.String-) | Obtient tous les attributs associés au document indexé spécifié. |
|
|  | [loadIntoMemoryCompletely(String indexFolder)](#loadIntoMemoryCompletely-java.lang.String-) | Charge l'intégralité de l'index en mémoire. |
|
|  | [loadIntoMemoryCompletely(String indexFolder, IndexSettings settings)](#loadIntoMemoryCompletely-java.lang.String-com.groupdocs.search.IndexSettings-) | Charge l'intégralité de l'index en mémoire. |
|
### Index() {#Index--}
```
public Index()
```


Initialise une nouvelle instance de la classe Index en mémoire.


L'exemple montre comment créer un index en mémoire sans enregistrer les fichiers sur le disque.

````
 ```

Index index = new Index();
 
```
 
````



### Index(IndexSettings settings) {#Index-com.groupdocs.search.IndexSettings-}
```
public Index(IndexSettings settings)
```


Initialise une nouvelle instance de la classe Index en mémoire avec des paramètres d'index spécifiques.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | L'objet de paramètres d'index. |


L'exemple montre comment créer un index en mémoire sans enregistrer les fichiers sur le disque avec des paramètres d'index particuliers.

````
 ```

IndexSettings settings = new IndexSettings();
settings.setIndexType(IndexType.CompactIndex);
Index index = new Index(settings);
 
```
 
````

|

### Index(String indexFolder) {#Index-java.lang.String-}
```
public Index(String indexFolder)
```


Initialise une nouvelle instance de la classe Index. Crée un nouvel index ou ouvre un index existant sur le disque.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | indexFolder | java.lang.String | Le chemin du dossier d'index. |


L'exemple montre comment créer un index sur un disque ou ouvrir un index existant.

````
 ```

String indexFolder = "c:\\MyIndex\\";
Index index = new Index(indexFolder);
 
```
 
````

|

### Index(String indexFolder, IndexSettings settings) {#Index-java.lang.String-com.groupdocs.search.IndexSettings-}
```
public Index(String indexFolder, IndexSettings settings)
```


Initialise une nouvelle instance de la
Index
classe.
Crée un nouvel index avec des paramètres particuliers ou ouvre un index existant sur le disque.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | indexFolder | java.lang.String | Le chemin du dossier d'index. |
|
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | L'objet de paramètres d'index. |

L'exemple montre comment créer un index sur un disque avec des paramètres d'index spécifiques.

````
 ```

String indexFolder = "c:\\MyIndex\\";
IndexSettings settings = new IndexSettings();
settings.setIndexType(IndexType.CompactIndex);
Index index = new Index(indexFolder, settings);
 
```
 
````

|

### Index(String indexFolder, boolean overwriteIfExists) {#Index-java.lang.String-boolean-}
```
public Index(String indexFolder, boolean overwriteIfExists)
```


Initialise une nouvelle instance de la
Index
classe.
Charge un index existant depuis le disque si
overwriteIfExists
est
false
;
crée un nouvel index sur le disque sinon.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | indexFolder | java.lang.String | Le chemin du dossier d'index. |
|
|  | overwriteIfExists | boolean | Le drapeau de remplacement du dossier d'index. |

L'exemple montre comment créer un nouvel index dans un dossier qui contient déjà un autre index.

````
 ```

String indexFolder = "c:\\MyIndex\\";
Index index = new Index(indexFolder, true);
 
```
 
````

|

### Index(String indexFolder, IndexSettings settings, boolean overwriteIfExists) {#Index-java.lang.String-com.groupdocs.search.IndexSettings-boolean-}
```
public Index(String indexFolder, IndexSettings settings, boolean overwriteIfExists)
```


Initialise une nouvelle instance de la
Index
classe.
Charge un index existant depuis le disque si
overwriteIfExists
est
false
;
crée un nouvel index sur le disque avec des paramètres d'index spécifiques sinon.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | indexFolder | java.lang.String | Le chemin du dossier d'index. |
|
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | L'objet de paramètres d'index. |
|
|  | overwriteIfExists | boolean | Le drapeau de remplacement du dossier d'index. |

L'exemple montre comment créer un index sur un disque avec des paramètres d'index spécifiques.

````
 ```

String indexFolder = "c:\\MyIndex\\";
IndexSettings settings = new IndexSettings();
settings.setIndexType(IndexType.CompactIndex);
Index index = new Index(indexFolder, settings, true);
 
```
 
````

|

### getEvents() {#getEvents--}
```
public final EventHub getEvents()
```


Obtient le hub d'événements pour s'abonner aux événements.


**Returns:**
[EventHub](../../com.groupdocs.search.events/eventhub) - The event hub for subscribing to events.

### getIndexInfo() {#getIndexInfo--}
```
public final IndexInfo getIndexInfo()
```


Obtient les informations de base sur l'index.


**Returns:**
[IndexInfo](../../com.groupdocs.search.common/indexinfo) - The basic information on the index.

### getRepository() {#getRepository--}
```
public final IndexRepository getRepository()
```


Obtient l'objet du référentiel d'index si l'index y est contenu.


**Returns:**
[IndexRepository](../../com.groupdocs.search/indexrepository) - The index repository object.

### getIndexSettings() {#getIndexSettings--}
```
public final IndexSettings getIndexSettings()
```


Obtient les paramètres de l'index.


**Returns:**
[IndexSettings](../../com.groupdocs.search/indexsettings) - The index settings.

### getDictionaries() {#getDictionaries--}
```
public final DictionaryRepository getDictionaries()
```


Obtient le référentiel du dictionnaire.


**Returns:**
[DictionaryRepository](../../com.groupdocs.search.dictionaries/dictionaryrepository) - The dictionary repository.

### close() {#close--}
```
public final void close()
```


Libère toutes les ressources utilisées par le
Index
.


### add(String path) {#add-java.lang.String-}
```
public final void add(String path)
```


Effectue l'opération d'indexation.
Ajoute un fichier ou un dossier par un chemin absolu ou relatif.
Les documents de tous les sous-dossiers seront indexés.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | chemin | java.lang.String | Le chemin d'un fichier ou d'un dossier à indexer. |

L'exemple montre comment ajouter des documents à un index.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String folderPath = "c:\\MyDocuments\\";
String filePath = "c:\\Documents\\MyFile.txt";
Index index = new Index(indexFolder); // Création de l'index dans le dossier spécifié
index.add(folderPath); // Indexation des documents dans le dossier spécifié
index.add(filePath); // Indexation du document spécifié
 
```
 
````

|

### add(String path, IndexingOptions options) {#add-java.lang.String-com.groupdocs.search.options.IndexingOptions-}
```
public final void add(String path, IndexingOptions options)
```


Effectue l'opération d'indexation.
Ajoute un fichier ou un dossier par un chemin absolu ou relatif.
Les documents de tous les sous-dossiers seront indexés.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | chemin | java.lang.String | Le chemin d'un fichier ou d'un dossier à indexer. |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | Les options d'indexation. |

L'exemple montre comment ajouter des documents à un index avec des options d'indexation particulières.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String folderPath = "c:\\MyDocuments\\";
String filePath = "c:\\Documents\\MyFile.txt";
Index index = new Index(indexFolder); // Création de l'index dans le dossier spécifié
IndexingOptions options = new IndexingOptions();
options.setThreads(2); // Définition du nombre de threads d'indexation
index.add(folderPath, options); // Indexation des documents dans le dossier spécifié
index.add(filePath, options); // Indexation du document spécifié
 
```
 
````

|

### add(String[] paths) {#add-java.lang.String---}
```
public final void add(String[] paths)
```


Effectue l'opération d'indexation.
Ajoute des fichiers ou dossiers par un chemin absolu ou relatif.
Les documents de tous les sous-dossiers seront indexés.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | chemins | java.lang.String[] | Les chemins vers des fichiers ou dossiers à indexer. |

L'exemple montre comment ajouter des documents à un index.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String folderPath = "c:\\MyDocuments\\";
String filePath = "c:\\Documents\\MyFile.txt";
Index index = new Index(indexFolder); // Création de l'index dans le dossier spécifié
String[] paths = new String[] { folderPath, filePath };
index.add(paths); // Indexation des documents aux chemins spécifiés
 
```
 
````

|

### add(String[] paths, IndexingOptions options) {#add-java.lang.String---com.groupdocs.search.options.IndexingOptions-}
```
public final void add(String[] paths, IndexingOptions options)
```


Effectue l'opération d'indexation.
Ajoute des fichiers ou dossiers par un chemin absolu ou relatif.
Les documents de tous les sous-dossiers seront indexés.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | chemins | java.lang.String[] | Les chemins vers des fichiers ou dossiers à indexer. |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | Les options d'indexation. |

L'exemple montre comment ajouter des documents à un index avec des options d'indexation particulières.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String folderPath = "c:\\MyDocuments\\";
String filePath = "c:\\Documents\\MyFile.txt";
Index index = new Index(indexFolder); // Création de l'index dans le dossier spécifié
IndexingOptions options = new IndexingOptions();
options.setThreads(2); // Définition du nombre de threads d'indexation
String[] paths = new String[] { folderPath, filePath };
index.add(paths, options); // Indexation des documents aux chemins spécifiés
 
```
 
````

|

### add(Document[] documents, IndexingOptions options) {#add-com.groupdocs.search.Document---com.groupdocs.search.options.IndexingOptions-}
```
public final void add(Document[] documents, IndexingOptions options)
```


Effectue l'opération d'indexation.
Ajoute des documents depuis le système de fichiers, le flux ou la structure.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | documents | [Document\[\]](../../com.groupdocs.search/document) | Les documents provenant du système de fichiers, du flux ou de la structure. |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | Les options d'indexation. |
|

### add(ExtractedData[] data, IndexingOptions options) {#add-com.groupdocs.search.ExtractedData---com.groupdocs.search.options.IndexingOptions-}
```
public final void add(ExtractedData[] data, IndexingOptions options)
```


Effectue l'opération d'indexation.
Ajoute les données extraites à l'index.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | data | [ExtractedData\[\]](../../com.groupdocs.search/extracteddata) | Les données extraites. |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | Les options d'indexation. |
|

### update() {#update--}
```
public final void update()
```


Ré-indexe les documents qui ont été modifiés ou supprimés depuis la dernière mise à jour.
Ajoute de nouveaux fichiers qui ont été ajoutés aux dossiers indexés.

L'exemple montre comment mettre à jour un index.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Création de l'index dans le dossier spécifié
index.add(documentsFolder); // Indexation des documents depuis le dossier spécifié
// Supprimer les documents du dossier de documents ou les modifier ou ajouter de nouveaux documents au dossier
index.update(); // Mise à jour de l'index
 
```
 
````



### update(UpdateOptions options) {#update-com.groupdocs.search.options.UpdateOptions-}
```
public final void update(UpdateOptions options)
```


Ré-indexe les documents qui ont été modifiés ou supprimés depuis la dernière mise à jour.
Ajoute de nouveaux fichiers qui ont été ajoutés aux dossiers indexés.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | options | [UpdateOptions](../../com.groupdocs.search.options/updateoptions) | Les options de mise à jour. |

L'exemple montre comment mettre à jour un index avec des options de mise à jour particulières.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Création de l'index dans le dossier spécifié
index.add(documentsFolder); // Indexation des documents depuis le dossier spécifié
// Supprimer les documents du dossier de documents ou les modifier ou ajouter de nouveaux documents au dossier
UpdateOptions options = new UpdateOptions();
options.setThreads(2); // Définition du nombre de threads d'indexation
index.update(options); // Mise à jour de l'index
 
```
 
````

|

### getIndexingReports() {#getIndexingReports--}
```
public final IndexingReport[] getIndexingReports()
```


Obtient les rapports sur les opérations d'indexation.


**Returns:**
com.groupdocs.search.common.IndexingReport[] - Les rapports d'indexation.

L'exemple montre comment obtenir les rapports d'indexation.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Création de l'index dans le dossier spécifié
index.add(documentsFolder); // Indexation des documents depuis le dossier spécifié
IndexingReport[] reports = index.getIndexingReports(); // Obtention des rapports d'indexation
 
```
 
````


### getSearchReports() {#getSearchReports--}
```
public final SearchReport[] getSearchReports()
```


Obtient les rapports sur les opérations de recherche.


**Returns:**
com.groupdocs.search.common.SearchReport[] - Les rapports de recherche.

L'exemple montre comment obtenir les rapports de recherche.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query1 = \"Einstein\";
String query2 = \"Newton\";
Index index = new Index(indexFolder); // Création de l'index dans le dossier spécifié
index.add(documentsFolder); // Indexation des documents depuis le dossier spécifié
SearchResult result1 = index.search(query1); // Recherche
SearchResult result2 = index.search(query2);
SearchResult result3 = index.search(query1 + \" & \" + query2);
SearchReport[] reports = index.getSearchReports(); // Obtention des rapports de recherche
 
```
 
````


### search(String query) {#search-java.lang.String-}
```
public final SearchResult search(String query)
```


Recherche dans l'index.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | query | java.lang.String | La requête de recherche. |

L'exemple suivant montre comment effectuer une recherche simple.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // Création de l'index dans le dossier spécifié
index.add(documentsFolder); // Indexation des documents depuis le dossier spécifié
SearchResult result = index.search(query); // Recherche
 
```
 
````

L'exemple suivant montre comment effectuer une recherche Regex.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Création de l'index dans le dossier spécifié
index.add(documentsFolder); // Indexation des documents depuis le dossier spécifié
String query = \"^[0-9]{3,}\"; // Le symbole caret au début de la requête de recherche indique à l'index qu'il s'agit d'une requête Regex
SearchResult result = index.search(query); // Recherche
 
```
 
````

L'exemple suivant montre comment effectuer une recherche à facettes.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Création de l'index dans le dossier spécifié
index.add(documentsFolder); // Indexation des documents depuis le dossier spécifié
String query = \"content:Newton\"; // Le mot avant les deux-points dans la requête indique le nom du champ du document à rechercher
SearchResult result = index.search(query); // Recherche
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(String query, SearchOptions options) {#search-java.lang.String-com.groupdocs.search.options.SearchOptions-}
```
public final SearchResult search(String query, SearchOptions options)
```


Recherche dans l'index.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | query | java.lang.String | La requête de recherche. |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | Les options de recherche. |

L'exemple suivant montre comment effectuer une recherche floue.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Création de l'index dans le dossier spécifié
index.add(documentsFolder); // Indexation des documents depuis le dossier spécifié
SearchOptions options = new SearchOptions();
options.getFuzzySearch().setEnabled(true); // Activation de la recherche floue
options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(1)); // Définition du nombre de différences possibles pour chaque mot
// Les guillemets doubles au début et à la fin indiquent à l'index qu'il s'agit d'une requête de recherche de phrase
String query = \"\\\"The Pursuit of Happiness\\\"\";
SearchResult result = index.search(query, options); // Recherche
 
```
 
````

L'exemple suivant montre comment effectuer une recherche de synonymes.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Création de l'index dans le dossier spécifié
index.add(documentsFolder); // Indexation des documents depuis le dossier spécifié
SearchOptions options = new SearchOptions();
options.setUseSynonymSearch(true); // Activation de la recherche de synonymes
String query = \"cry\";
SearchResult result = index.search(query, options); // Recherche
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(SearchQuery query) {#search-com.groupdocs.search.SearchQuery-}
```
public final SearchResult search(SearchQuery query)
```


Recherche dans l'index.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | La requête de recherche. |

L'exemple suivant montre comment effectuer une recherche en utilisant la requête sous forme d'objet.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Création de l'index dans le dossier spécifié
index.add(documentsFolder); // Indexation des documents depuis le dossier spécifié
// Création de la sous-requête 1
SearchQuery subquery1 = SearchQuery.createWordQuery(\"accommodation\");
subquery1.setSearchOptions(new SearchOptions()); // Définition des options de recherche uniquement pour la sous-requête 1
subquery1.getSearchOptions().getFuzzySearch().setEnabled(true); // Activation de la recherche floue
subquery1.getSearchOptions().getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(3)); // Définition du nombre maximal de différences
// Création de la sous-requête 2
SearchQuery subquery2 = SearchQuery.createNumericRangeQuery(1, 1000000);
// Création de la sous-requête 3
SearchQuery subquery3 = SearchQuery.createRegexQuery("(.)\\1");
// Combinaison des sous-requêtes en une seule requête
SearchQuery query = SearchQuery.createPhraseSearchQuery(subquery1, subquery2, subquery3);
SearchResult result = index.search(query); // Recherche
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(SearchQuery query, SearchOptions options) {#search-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-}
```
public final SearchResult search(SearchQuery query, SearchOptions options)
```


Recherche dans l'index.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | La requête de recherche. |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | Les options de recherche. |

L'exemple suivant montre comment effectuer une recherche en utilisant la requête sous forme d'objet.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Création de l'index dans le dossier spécifié
index.add(documentsFolder); // Indexation des documents depuis le dossier spécifié
// Création d'une sous-requête de recherche de plage de dates
SearchQuery subquery1 = SearchQuery.createDateRangeQuery(new Date(2011, 6, 17), new Date(2013, 1, 1));
// Création d'une sous-requête de joker avec un nombre de mots manquants de 0 à 2
SearchQuery subquery2 = SearchQuery.createWildcardQuery(0, 2);
// Création d'une sous-requête de mot simple
SearchQuery subquery3 = SearchQuery.createWordQuery(\"birth\");
subquery3.setSearchOptions(new SearchOptions()); // Définition des options de recherche uniquement pour la sous-requête 3
subquery3.getSearchOptions().getFuzzySearch().setEnabled(true);
subquery3.getSearchOptions().getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(1));
// Combinaison des sous-requêtes en une seule requête
SearchQuery query = SearchQuery.createPhraseSearchQuery(subquery1, subquery2, subquery3);
// Création d'un objet d'options de recherche avec une capacité accrue des occurrences trouvées
SearchOptions options = new SearchOptions(); // Options de recherche globales
options.setMaxOccurrenceCountPerTerm(1000000);
options.setMaxTotalOccurrenceCount(10000000);
SearchResult result = index.search(query, options); // Recherche
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(SearchImage image, ImageSearchOptions options) {#search-com.groupdocs.search.common.SearchImage-com.groupdocs.search.options.ImageSearchOptions-}
```
public final ImageSearchResult search(SearchImage image, ImageSearchOptions options)
```


Effectue une recherche d'image inversée dans l'index.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | image | [SearchImage](../../com.groupdocs.search.common/searchimage) | L'image à rechercher. |
|
|  | options | [ImageSearchOptions](../../com.groupdocs.search.options/imagesearchoptions) | Les options de recherche d'image. |
|

**Returns:**
[ImageSearchResult](../../com.groupdocs.search.results/imagesearchresult) - The result of a reverse image search.

### searchNext(ChunkSearchToken chunkSearchToken) {#searchNext-com.groupdocs.search.common.ChunkSearchToken-}
```
public final SearchResult searchNext(ChunkSearchToken chunkSearchToken)
```


Continue la recherche par morceaux commencée avec la méthode Search.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | chunkSearchToken | [ChunkSearchToken](../../com.groupdocs.search.common/chunksearchtoken) | Le jeton de recherche de fragment. |

L'exemple montre comment effectuer une recherche de fragment.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // Création de l'index dans le dossier spécifié
index.add(documentsFolder); // Indexation des documents depuis le dossier spécifié
SearchOptions options = new SearchOptions();
options.setChunkSearch(true); // Activation de la recherche de fragment
SearchResult result = index.search(query, options); // Démarrage de la recherche de fragment
System.out.println("Nombre de documents : " + result.getDocumentCount());
System.out.println("Nombre d'occurrences : " + result.getOccurrenceCount());
while (result.getNextChunkSearchToken() != null) {
result = index.searchNext(result.getNextChunkSearchToken()); // Continuation de la recherche de fragment
System.out.println("Nombre de documents : " + result.getDocumentCount());
System.out.println("Nombre d'occurrences : " + result.getOccurrenceCount());
}
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### searchNext(ChunkSearchToken chunkSearchToken, Cancellation cancellation) {#searchNext-com.groupdocs.search.common.ChunkSearchToken-com.groupdocs.search.common.Cancellation-}
```
public final SearchResult searchNext(ChunkSearchToken chunkSearchToken, Cancellation cancellation)
```


Continue la recherche par morceaux commencée avec la méthode Search.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | chunkSearchToken | [ChunkSearchToken](../../com.groupdocs.search.common/chunksearchtoken) | Le jeton de recherche de fragment. |
|
|  | cancellation | [Cancellation](../../com.groupdocs.search.common/cancellation) | L'objet d'annulation. |

L'exemple montre comment effectuer une recherche en utilisant la requête sous forme d'objet.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // Création de l'index dans le dossier spécifié
index.add(documentsFolder); // Indexation des documents depuis le dossier spécifié
Cancellation cancellation = new Cancellation(); // Cet objet d'annulation interrompt toutes les continuations de recherche s'il est annulé
SearchOptions options = new SearchOptions();
options.setChunkSearch(true); // Activation de la recherche de fragment
options.setCancellation(cancellation);
SearchResult result = index.search(query, options); // Démarrage de la recherche de fragment
System.out.println("Nombre de documents : " + result.getDocumentCount());
System.out.println("Nombre d'occurrences : " + result.getOccurrenceCount());
while (result.getNextChunkSearchToken() != null) {
result = index.searchNext(result.getNextChunkSearchToken(), cancellation); // Continuation de la recherche de fragment
System.out.println("Nombre de documents : " + result.getDocumentCount());
System.out.println("Nombre d'occurrences : " + result.getOccurrenceCount());
}
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### optimize() {#optimize--}
```
public final void optimize()
```


Réduit le nombre de segments d'index en les fusionnant les uns avec les autres.
Cette opération améliore les performances de recherche.

L'exemple montre comment fusionner les segments d'un index.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder1 = "c:\\MyDocuments1\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
String documentsFolder3 = "c:\\MyDocuments3\\";
Index index = new Index(indexFolder); // Création de l'index dans le dossier spécifié
index.add(documentsFolder1); // Indexation des documents depuis le dossier spécifié
index.add(documentsFolder2); // Chaque appel à AddToIndex crée au moins un nouveau segment dans l'index
index.add(documentsFolder3);
// Fusion des segments de l'index
index.optimize();
 
```
 
````



### optimize(MergeOptions options) {#optimize-com.groupdocs.search.options.MergeOptions-}
```
public final void optimize(MergeOptions options)
```


Réduit le nombre de segments d'index en les fusionnant les uns avec les autres.
Cette opération améliore les performances de recherche.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | options | [MergeOptions](../../com.groupdocs.search.options/mergeoptions) | Les options de fusion. |

L'exemple montre comment fusionner les segments d'un index avec des options de fusion particulières.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder1 = "c:\\MyDocuments1\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
String documentsFolder3 = "c:\\MyDocuments3\\";
Index index = new Index(indexFolder); // Création de l'index dans le dossier spécifié
index.add(documentsFolder1); // Indexation des documents depuis le dossier spécifié
index.add(documentsFolder2); // Chaque appel à AddToIndex crée au moins un nouveau segment dans l'index
index.add(documentsFolder3);
MergeOptions options = new MergeOptions();
options.setAsync(true); // opération asynchrone
options.setCancellation(new Cancellation()); // Création de l'objet d'annulation
// Fusion des segments de l'index
index.optimize(options); // Cette méthode retournera avant que l'opération ne soit terminée
options.getCancellation().cancelAfter(10000); // Définition de la durée maximale de l'opération à 10 secondes
 
```
 
````

|

### merge(Index index, MergeOptions options) {#merge-com.groupdocs.search.Index-com.groupdocs.search.options.MergeOptions-}
```
public final void merge(Index index, MergeOptions options)
```


Fusionne l'index spécifié dans l'index actuel.
Notez que l'autre index ne sera pas modifié.


Si l'autre index possède une version précédente, il doit être mis à jour avant la fusion avec
IndexUpdater
.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | index | [Index](../../com.groupdocs.search/index) | L'index dans lequel fusionner. |
|
|  | options | [MergeOptions](../../com.groupdocs.search.options/mergeoptions) | Les options de fusion. |

L'exemple montre comment fusionner un index dans l'index actuel.

````
 ```

String indexFolder1 = "c:\\MyIndex1\\";
String indexFolder2 = "c:\\MyIndex2\\";
String documentsFolder1 = "c:\\MyDocuments1\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
Index index1 = new Index(indexFolder1); // Création de l'index1
index1.add(documentsFolder1); // Indexation des documents
Index index2 = new Index(indexFolder2); // Création de l'index2
index2.add(documentsFolder2); // Indexation des documents
MergeOptions options = new MergeOptions();
options.setCancellation(new Cancellation()); // Création de l'objet d'annulation
// Fusion de index2 dans index1. Notez que les fichiers de index2 ne seront pas modifiés.
index1.merge(index2, options);
 
```
 
````

|

### merge(IndexRepository repository, MergeOptions options) {#merge-com.groupdocs.search.IndexRepository-com.groupdocs.search.options.MergeOptions-}
```
public final void merge(IndexRepository repository, MergeOptions options)
```


Fusionne les index du référentiel d'index spécifié dans l'index actuel.
Notez que les index dans le référentiel ne seront pas modifiés.


Si d'autres index ont une version précédente, ils doivent être mis à jour avant de fusionner avec
IndexUpdater
.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | repository | [IndexRepository](../../com.groupdocs.search/indexrepository) | Le référentiel d'index dans lequel fusionner. |
|
|  | options | [MergeOptions](../../com.groupdocs.search.options/mergeoptions) | Les options de fusion. |

L'exemple montre comment fusionner un référentiel d'index dans l'index actuel.

````
 ```

String indexFolder1 = "c:\\MyIndex1\\";
String indexFolder2 = "c:\\MyIndex2\\";
String indexFolder3 = "c:\\MyIndex3\\";
String documentsFolder1 = "c:\\MyDocuments1\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
String documentsFolder3 = "c:\\MyDocuments3\\";
Index index1 = new Index(indexFolder1); // Création de l'index1
index1.add(documentsFolder1); // Indexation des documents
IndexRepository repository = new IndexRepository(); // Création du référentiel d'index
Index index2 = repository.create(indexFolder2); // Création de l'index2
index2.add(documentsFolder2); // Indexation des documents
Index index3 = repository.create(indexFolder3); // Création de l'index3
index3.add(documentsFolder3); // Indexation des documents
MergeOptions options = new MergeOptions();
options.setCancellation(new Cancellation()); // Création de l'objet d'annulation
// Fusion de tous les index du référentiel d'index dans index1. Notez que index2 et index3 ne seront pas modifiés.
index1.merge(repository, options);
 
```
 
````

|

### highlight(FoundDocument document, Highlighter highlighter) {#highlight-com.groupdocs.search.results.FoundDocument-com.groupdocs.search.highlighters.Highlighter-}
```
public final void highlight(FoundDocument document, Highlighter highlighter)
```


Génère du texte formaté en HTML avec les termes trouvés mis en évidence.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | document | [FoundDocument](../../com.groupdocs.search.results/founddocument) | Le document trouvé. |
|
|  | highlighter | [Highlighter](../../com.groupdocs.search.highlighters/highlighter) | Le surligneur de résultats de recherche. |

L'exemple montre comment mettre en évidence les occurrences dans du texte formaté en HTML.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentFolder = "c:\\MyDocuments\\";
// Création d'un index
Index index = new Index(indexFolder);
// Indexation des documents du dossier spécifié
index.add(documentFolder);
// Recherche du mot 'eternity'
SearchResult result = index.search("eternity");
// Mise en évidence des occurrences dans le texte
if (result.getDocumentCount() > 0) {
FoundDocument document = result.getFoundDocument(0); // Obtention du premier document trouvé
OutputAdapter outputAdapter = new FileOutputAdapter("c:\\Highlighted.html"); // Création d'un adaptateur de sortie vers le fichier
Highlighter highlighter = new HtmlHighlighter(outputAdapter); // Création de l'objet highlighter
index.highlight(document, highlighter); // Génération du texte formaté HTML avec les occurrences surlignées
}
 
```
 
````

|

### highlight(FoundDocument document, Highlighter highlighter, HighlightOptions options) {#highlight-com.groupdocs.search.results.FoundDocument-com.groupdocs.search.highlighters.Highlighter-com.groupdocs.search.options.HighlightOptions-}
```
public final void highlight(FoundDocument document, Highlighter highlighter, HighlightOptions options)
```


Génère du texte formaté en HTML avec les termes trouvés mis en évidence.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | document | [FoundDocument](../../com.groupdocs.search.results/founddocument) | Le document trouvé. |
|
|  | highlighter | [Highlighter](../../com.groupdocs.search.highlighters/highlighter) | Le surligneur de résultats de recherche. |
|
|  | options | [HighlightOptions](../../com.groupdocs.search.options/highlightoptions) | Les options de surlignage. |

L'exemple montre comment mettre en évidence les occurrences dans du texte formaté en HTML.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentFolder = "c:\\MyDocuments\\";
// Création d'un index
Index index = new Index(indexFolder);
// Indexation des documents du dossier spécifié
index.add(documentFolder);
// Recherche du mot 'eternity'
SearchResult result = index.search("eternity");
// Mise en évidence des occurrences dans le texte
if (result.getDocumentCount() > 0) {
FoundDocument document = result.getFoundDocument(0); // Obtention du premier document trouvé
OutputAdapter outputAdapter = new FileOutputAdapter("c:\\Highlighted.html"); // Création d'un adaptateur de sortie vers le fichier
Highlighter highlighter = new HtmlHighlighter(outputAdapter); // Création de l'objet highlighter
HighlightOptions options = new HighlightOptions(); // Création de l'objet d'options de surlignage
options.setTermsBefore(5);
options.setTermsAfter(5);
options.setTermsTotal(15);
index.highlight(document, highlighter, options); // Génération du texte formaté HTML avec les occurrences surlignées
}
 
```
 
````

|

### getIndexedDocuments() {#getIndexedDocuments--}
```
public final DocumentInfo[] getIndexedDocuments()
```


Obtient un tableau de tous les documents indexés.


**Returns:**
com.groupdocs.search.results.DocumentInfo[] - Un tableau de tous les documents indexés.

L'exemple montre comment obtenir une liste de documents indexés à partir d'un index.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Création d'un index dans le dossier spécifié
Index index = new Index(indexFolder);
// Indexation des documents du dossier spécifié
index.add(documentsFolder);
// Obtention de la liste des documents indexés
DocumentInfo[] documents = index.getIndexedDocuments();
 
```
 
````


### getIndexedDocumentItems(DocumentInfo documentInfo) {#getIndexedDocumentItems-com.groupdocs.search.results.DocumentInfo-}
```
public final DocumentInfo[] getIndexedDocumentItems(DocumentInfo documentInfo)
```


Obtient un tableau d'éléments de document.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | documentInfo | [DocumentInfo](../../com.groupdocs.search.results/documentinfo) | Une information de document. |

L'exemple montre comment obtenir une liste d'éléments d'un document indexé à partir d'un index.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Création d'un index dans le dossier spécifié
Index index = new Index(indexFolder);
// Indexation des documents du dossier spécifié
index.add(documentsFolder);
// Obtention de la liste des documents indexés
DocumentInfo[] documents = index.getIndexedDocuments();
for (int i = 0; i < documents.length; i++) {
DocumentInfo document = documents[i];
System.out.println(document.getFilePath());
DocumentInfo[] items = index.getIndexedDocumentItems(document); // Obtention de la liste des éléments du document
for (int j = 0; j < items.length; j++) {
DocumentInfo item = items[j];
System.out.println("\t" + item.getInnerPath());
}
}
 
```
 
````

|

**Returns:**
com.groupdocs.search.results.DocumentInfo[] - Un tableau d'éléments d'un document.

### GetIndexedDocument(String documentKey) {#GetIndexedDocument-java.lang.String-}
```
public DocumentInfo GetIndexedDocument(String documentKey)
```


Obtient un document indexé par clé de document.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | documentKey | java.lang.String | La clé du document. |
|

**Returns:**
[DocumentInfo](../../com.groupdocs.search.results/documentinfo) - The indexed document.

### getDocumentText(DocumentInfo documentInfo, OutputAdapter adapter) {#getDocumentText-com.groupdocs.search.results.DocumentInfo-com.groupdocs.search.common.OutputAdapter-}
```
public final void getDocumentText(DocumentInfo documentInfo, OutputAdapter adapter)
```


Génère le texte d'un document indexé et le transmet via un adaptateur de sortie.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | documentInfo | [DocumentInfo](../../com.groupdocs.search.results/documentinfo) | Les informations du document indexé. |
|
|  | adapter | [OutputAdapter](../../com.groupdocs.search.common/outputadapter) | L'adaptateur de sortie. |

L'exemple montre comment obtenir le texte d'un document indexé à partir d'un index.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Création d'un index dans le dossier spécifié
Index index = new Index(indexFolder);
// Indexation des documents du dossier spécifié
index.add(documentsFolder);
// Obtention de la liste des documents indexés
DocumentInfo[] documents = index.getIndexedDocuments();
// Obtention du texte d'un document
if (documents.length > 0) {
FileOutputAdapter outputAdapter = new FileOutputAdapter("C:\\Text.html");
index.getDocumentText(documents[0], outputAdapter);
}
 
```
 
````

|

### getDocumentText(DocumentInfo documentInfo, OutputAdapter adapter, TextOptions options) {#getDocumentText-com.groupdocs.search.results.DocumentInfo-com.groupdocs.search.common.OutputAdapter-com.groupdocs.search.options.TextOptions-}
```
public final void getDocumentText(DocumentInfo documentInfo, OutputAdapter adapter, TextOptions options)
```


Génère du texte formaté en HTML pour le document indexé et le transfère via l'adaptateur de sortie.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | documentInfo | [DocumentInfo](../../com.groupdocs.search.results/documentinfo) | Les informations du document indexé. |
|
|  | adapter | [OutputAdapter](../../com.groupdocs.search.common/outputadapter) | L'adaptateur de sortie. |
|
|  | options | [TextOptions](../../com.groupdocs.search.options/textoptions) | Les options de récupération du texte. |
|

### getIndexedPaths() {#getIndexedPaths--}
```
public final String[] getIndexedPaths()
```


Obtient un tableau de chemins indexés - documents ou dossiers.


**Returns:**
java.lang.String[] - Un tableau de chemins indexés.

### delete(String[] paths, UpdateOptions options) {#delete-java.lang.String---com.groupdocs.search.options.UpdateOptions-}
```
public final DeleteResult delete(String[] paths, UpdateOptions options)
```


Supprime les fichiers ou dossiers indexés de l'index. Met ensuite à jour l'index sans les chemins supprimés.
Notez qu'un document individuel ne peut pas être supprimé de l'index s'il a été ajouté à l'index dans le cadre d'un dossier.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | chemins | java.lang.String[] | Les chemins des fichiers ou dossiers à supprimer. |
|
|  | options | [UpdateOptions](../../com.groupdocs.search.options/updateoptions) | Les options de mise à jour. |

L'exemple montre comment supprimer des chemins indexés d'un index.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder1 = "c:\\MyDocuments\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
// Création d'un index dans le dossier spécifié
Index index = new Index(indexFolder);
// Indexation des documents à partir des dossiers spécifiés
index.add(documentsFolder1);
index.add(documentsFolder2);
// Obtention des chemins indexés depuis l'index
String[] indexedPaths1 = index.getIndexedPaths();
// Écriture des chemins indexés dans la console
System.out.println("Chemins indexés :");
for (String path : indexedPaths1) {
System.out.println("\t" + path);
}
// Suppression du chemin d'index de l'index
DeleteResult deleteResult = index.delete(new String[] { documentsFolder1 }, new UpdateOptions());
// Obtention des chemins indexés après suppression
String[] indexedPaths2 = index.getIndexedPaths();
System.out.println("\nChemins supprimés : " + deleteResult.getSuccessCount());
System.out.println("\nIndexed paths:");
for (String path : indexedPaths2) {
System.out.println("\t" + path);
}
 
```
 
````

|

**Returns:**
[DeleteResult](../../com.groupdocs.search.results/deleteresult) - An object describing the result of deleting files or folders from the index.

### delete(UpdateOptions options, String[] documentKeys) {#delete-com.groupdocs.search.options.UpdateOptions-java.lang.String---}
```
public final DeleteResult delete(UpdateOptions options, String[] documentKeys)
```


Supprime les documents indexés à partir de flux ou de structures. Puis met à jour l'index sans les documents supprimés.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | options | [UpdateOptions](../../com.groupdocs.search.options/updateoptions) | Les options de mise à jour. |
|
|  | documentKeys | java.lang.String[] | Les clés des documents ajoutés à partir de flux ou de structures. |
|

**Returns:**
[DeleteResult](../../com.groupdocs.search.results/deleteresult) - An object describing the result of deleting documents from the index.

### notifyIndex(Notification notification) {#notifyIndex-com.groupdocs.search.Notification-}
```
public final boolean notifyIndex(Notification notification)
```


Transmet l'objet de notification spécifié à l'index pour effectuer la notification.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | notification | [Notification](../../com.groupdocs.search/notification) | L'objet de notification. |
|

**Returns:**
boolean - Retourne  true  si la notification a été effectuée avec succès ; sinon  false .

### changeAttributes(AttributeChangeBatch batch) {#changeAttributes-com.groupdocs.search.common.AttributeChangeBatch-}
```
public final void changeAttributes(AttributeChangeBatch batch)
```


Applique le lot spécifié de modifications d'attributs aux documents indexés sans réindexation pendant l'opération de mise à jour.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | batch | [AttributeChangeBatch](../../com.groupdocs.search.common/attributechangebatch) | Le lot de modifications d'attributs. |
|

### getAttributes(String path) {#getAttributes-java.lang.String-}
```
public final String[] getAttributes(String path)
```


Obtient tous les attributs associés au document indexé spécifié.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | chemin | java.lang.String | Le chemin du document. |
|

**Returns:**
java.lang.String[] - Attributs associés au document.

### loadIntoMemoryCompletely(String indexFolder) {#loadIntoMemoryCompletely-java.lang.String-}
```
public static Index loadIntoMemoryCompletely(String indexFolder)
```


Charge l'intégralité de l'index en mémoire.
Toute modification de l'index n'est pas enregistrée automatiquement dans le dossier d'origine.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | indexFolder | java.lang.String | Le chemin du dossier d'index. |
|

**Returns:**
[Index](../../com.groupdocs.search/index) - The loaded in-memory index.

### loadIntoMemoryCompletely(String indexFolder, IndexSettings settings) {#loadIntoMemoryCompletely-java.lang.String-com.groupdocs.search.IndexSettings-}
```
public static Index loadIntoMemoryCompletely(String indexFolder, IndexSettings settings)
```


Charge l'intégralité de l'index en mémoire.
Toute modification de l'index n'est pas enregistrée automatiquement dans le dossier d'origine.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | indexFolder | java.lang.String | Le chemin du dossier d'index. |
|
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | L'objet de paramètres d'index. |
|

**Returns:**
[Index](../../com.groupdocs.search/index) - The loaded in-memory index.

