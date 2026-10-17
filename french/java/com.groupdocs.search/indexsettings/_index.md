---
title: "IndexSettings"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Représente les paramètres d'index qui permettent de personnaliser les opérations d'indexation."
type: docs
weight: 19
url: /fr/java/com.groupdocs.search/indexsettings/
---
**Inheritance:**
java.lang.Object
```
public class IndexSettings
```

Représente les paramètres d'index qui permettent de personnaliser les opérations d'indexation.


**Learn more**

* [Search index settings](../https://docs.groupdocs.com/display/searchjava/Search+index+settings)


L'exemple montre une utilisation typique de la classe.

````
 ```

String indexFolder = "c:\\MyIndex\\";
IndexSettings settings = new IndexSettings();
settings.setIndexType(IndexType.CompactIndex); // Définition du type d'index
Index index = new Index(indexFolder, settings); // Création d'un index
 
```
 
````


## Constructeurs

| Constructeur | Description |
| --- | --- |
|  | [IndexSettings()](#IndexSettings--) | Initialise une nouvelle instance de la classe  IndexSettings  . |
|
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getInMemoryIndex()](#getInMemoryIndex--) | Obtient une valeur indiquant si l'index est stocké en mémoire ou sur le disque. |
|
|  | [getUseStopWords()](#getUseStopWords--) | Obtient une valeur indiquant s'il faut utiliser des mots vides ou non. |
|
|  | [setUseStopWords(boolean value)](#setUseStopWords-boolean-) | Définit une valeur indiquant s'il faut utiliser des mots vides ou non. |
|
|  | [getMaxIndexingReportCount()](#getMaxIndexingReportCount--) | Obtient le nombre maximal de rapports d'indexation. |
|
|  | [setMaxIndexingReportCount(int value)](#setMaxIndexingReportCount-int-) | Définit le nombre maximal de rapports d'indexation. |
|
|  | [getMaxSearchReportCount()](#getMaxSearchReportCount--) | Obtient le nombre maximal de rapports de recherche. |
|
|  | [setMaxSearchReportCount(int value)](#setMaxSearchReportCount-int-) | Définit le nombre maximal de rapports de recherche. |
|
|  | [getUseCharacterReplacements()](#getUseCharacterReplacements--) | Obtient une valeur indiquant s'il faut utiliser des remplacements de caractères ou non. |
|
|  | [setUseCharacterReplacements(boolean value)](#setUseCharacterReplacements-boolean-) | Définit une valeur indiquant s'il faut utiliser des remplacements de caractères ou non. |
|
|  | [getDocumentFilter()](#getDocumentFilter--) | Obtient un filtre de document. |
|
|  | [setDocumentFilter(DocumentFilter value)](#setDocumentFilter-com.groupdocs.search.DocumentFilter-) | Définit un filtre de document. |
|
|  | [getTextStorageSettings()](#getTextStorageSettings--) | Obtient les paramètres de stockage du texte. |
|
|  | [setTextStorageSettings(TextStorageSettings value)](#setTextStorageSettings-com.groupdocs.search.options.TextStorageSettings-) | Définit les paramètres de stockage du texte. |
|
|  | [getIndexType()](#getIndexType--) | Obtient le type d'index. |
|
|  | [setIndexType(IndexType value)](#setIndexType-com.groupdocs.search.options.IndexType-) | Définit le type d'index. |
|
|  | [getSearchThreads()](#getSearchThreads--) | Obtient le nombre de threads utilisés pour la recherche. |
|
|  | [setSearchThreads(NumberOfThreads value)](#setSearchThreads-com.groupdocs.search.options.NumberOfThreads-) | Définit le nombre de threads utilisés pour la recherche. |
|
|  | [getCustomExtractors()](#getCustomExtractors--) | Obtient la collection d'extracteurs personnalisés. |
|
|  | [getLogger()](#getLogger--) | Obtient un journaliseur utilisé pour consigner les événements et les erreurs dans l'index. |
|
|  | [setLogger(ILogger value)](#setLogger-com.groupdocs.search.common.ILogger-) | Définit un journaliseur utilisé pour consigner les événements et les erreurs dans l'index. |
|
### IndexSettings() {#IndexSettings--}
```
public IndexSettings()
```


Initialise une nouvelle instance de la classe  IndexSettings  .


### getInMemoryIndex() {#getInMemoryIndex--}
```
public final boolean getInMemoryIndex()
```


Obtient une valeur indiquant si l'index est stocké en mémoire ou sur le disque.


**Returns:**
boolean - Une valeur indiquant si l'index est stocké en mémoire ou sur disque.

### getUseStopWords() {#getUseStopWords--}
```
public final boolean getUseStopWords()
```


Obtient une valeur indiquant s'il faut utiliser des mots vides ou non. La valeur par défaut est  true .


**Returns:**
boolean - Une valeur indiquant s'il faut utiliser des mots vides ou non.

### setUseStopWords(boolean value) {#setUseStopWords-boolean-}
```
public final void setUseStopWords(boolean value)
```


Définit une valeur indiquant s'il faut utiliser des mots vides ou non. La valeur par défaut est  true .


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | valeur | boolean | Une valeur indiquant s'il faut utiliser des mots vides ou non. |
|

### getMaxIndexingReportCount() {#getMaxIndexingReportCount--}
```
public final int getMaxIndexingReportCount()
```


Obtient le nombre maximal de rapports d'indexation. La valeur par défaut est  5 .


**Returns:**
int - Le nombre maximal de rapports d'indexation.

### setMaxIndexingReportCount(int value) {#setMaxIndexingReportCount-int-}
```
public final void setMaxIndexingReportCount(int value)
```


Définit le nombre maximal de rapports d'indexation. La valeur par défaut est  5 .


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | valeur | int | Le nombre maximal de rapports d'indexation. |
|

### getMaxSearchReportCount() {#getMaxSearchReportCount--}
```
public final int getMaxSearchReportCount()
```


Obtient le nombre maximal de rapports de recherche. La valeur par défaut est  10 .


**Returns:**
int - Le nombre maximal de rapports de recherche.

### setMaxSearchReportCount(int value) {#setMaxSearchReportCount-int-}
```
public final void setMaxSearchReportCount(int value)
```


Définit le nombre maximal de rapports de recherche. La valeur par défaut est  10 .


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | valeur | int | Le nombre maximal de rapports de recherche. |
|

### getUseCharacterReplacements() {#getUseCharacterReplacements--}
```
public final boolean getUseCharacterReplacements()
```


Obtient une valeur indiquant s'il faut utiliser des remplacements de caractères ou non. La valeur par défaut est  false .


**Returns:**
boolean - Une valeur indiquant s'il faut utiliser des remplacements de caractères ou non.

### setUseCharacterReplacements(boolean value) {#setUseCharacterReplacements-boolean-}
```
public final void setUseCharacterReplacements(boolean value)
```


Définit une valeur indiquant s'il faut utiliser des remplacements de caractères ou non. La valeur par défaut est  false .


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | valeur | boolean | Une valeur indiquant s'il faut utiliser des remplacements de caractères ou non. |
|

### getDocumentFilter() {#getDocumentFilter--}
```
public final DocumentFilter getDocumentFilter()
```


Obtient un filtre de documents. Le  DocumentFilter  fonctionne selon la logique d'inclusion. Utilisez la classe  DocumentFilter  pour créer une instance de filtre de documents. La valeur par défaut est  null , ce qui signifie que tous les documents ajoutés sont indexés.


**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - The document filter.

L'exemple montre comment définir le filtre de documents.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Création d'un filtre qui ignore les documents avec les extensions '.doc', '.docx', '.rtf'
IndexSettings settings = new IndexSettings();
DocumentFilter fileExtensionFilter = DocumentFilter.createFileExtension(".doc", ".docx", ".rtf"); // Création du filtre d'extension de fichier
DocumentFilter invertedFilter = DocumentFilter.createNot(fileExtensionFilter); // Inversion du filtre d'extension de fichier
settings.setDocumentFilter(invertedFilter);
// Création d'un index dans le dossier spécifié
Index index = new Index(indexFolder, settings);
// Indexation des documents
index.add(documentsFolder);
// Recherche
SearchResult result = index.search("Einstein");
 
```
 
````


### setDocumentFilter(DocumentFilter value) {#setDocumentFilter-com.groupdocs.search.DocumentFilter-}
```
public final void setDocumentFilter(DocumentFilter value)
```


Définit un filtre de document. Le  DocumentFilter  fonctionne selon la logique d'inclusion. Utilisez la classe  GroupDocs.Search.Options.DocumentFilter  pour créer des instances de filtre de document. La valeur par défaut est  null , ce qui signifie que tous les documents ajoutés sont indexés.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | value | [DocumentFilter](../../com.groupdocs.search/documentfilter) | Le filtre de document. |

L'exemple montre comment définir le filtre de documents.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Création d'un filtre qui ignore les documents avec les extensions '.doc', '.docx', '.rtf'
IndexSettings settings = new IndexSettings();
DocumentFilter fileExtensionFilter = DocumentFilter.createFileExtension(".doc", ".docx", ".rtf"); // Création du filtre d'extension de fichier
DocumentFilter invertedFilter = DocumentFilter.createNot(fileExtensionFilter); // Inversion du filtre d'extension de fichier
settings.setDocumentFilter(invertedFilter);
// Création d'un index dans le dossier spécifié
Index index = new Index(indexFolder, settings);
// Indexation des documents
index.add(documentsFolder);
// Recherche
SearchResult result = index.search("Einstein");
 
```
 
````

|

### getTextStorageSettings() {#getTextStorageSettings--}
```
public final TextStorageSettings getTextStorageSettings()
```


Obtient les paramètres de stockage du texte. La valeur par défaut est  null , ce qui signifie que les textes des documents ne sont pas stockés.


**Returns:**
[TextStorageSettings](../../com.groupdocs.search.options/textstoragesettings) - The text storage settings.

L'exemple montre comment définir les paramètres de stockage du texte.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Création d'une instance de paramètres d'index
IndexSettings settings = new IndexSettings();
settings.setTextStorageSettings(new TextStorageSettings(Compression.High)); // Définition d'un niveau de compression élevé pour le stockage du texte de l'index
// Création d'un index dans le dossier spécifié
Index index = new Index(indexFolder, settings);
// Indexation des documents
index.add(documentsFolder);
// Recherche
SearchResult result = index.search("Einstein");
 
```
 
````


### setTextStorageSettings(TextStorageSettings value) {#setTextStorageSettings-com.groupdocs.search.options.TextStorageSettings-}
```
public final void setTextStorageSettings(TextStorageSettings value)
```


Définit les paramètres de stockage du texte. La valeur par défaut est  null , ce qui signifie que les textes des documents ne sont pas stockés.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | value | [TextStorageSettings](../../com.groupdocs.search.options/textstoragesettings) | Les paramètres de stockage du texte. |

L'exemple montre comment définir les paramètres de stockage du texte.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Création d'une instance de paramètres d'index
IndexSettings settings = new IndexSettings();
settings.setTextStorageSettings(new TextStorageSettings(Compression.High)); // Définition d'un niveau de compression élevé pour le stockage du texte de l'index
// Création d'un index dans le dossier spécifié
Index index = new Index(indexFolder, settings);
// Indexation des documents
index.add(documentsFolder);
// Recherche
SearchResult result = index.search("Einstein");
 
```
 
````

|

### getIndexType() {#getIndexType--}
```
public final IndexType getIndexType()
```


Obtient le type d'index. La valeur par défaut est  GroupDocs.Search.Options.IndexType.NormalIndex .


**Returns:**
[IndexType](../../com.groupdocs.search.options/indextype) - The index type.

### setIndexType(IndexType value) {#setIndexType-com.groupdocs.search.options.IndexType-}
```
public final void setIndexType(IndexType value)
```


Définit le type d'index. La valeur par défaut est  GroupDocs.Search.Options.IndexType.NormalIndex .


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | value | [IndexType](../../com.groupdocs.search.options/indextype) | Le type d'index. |
|

### getSearchThreads() {#getSearchThreads--}
```
public final NumberOfThreads getSearchThreads()
```


Obtient le nombre de threads utilisés pour la recherche. La valeur par défaut est  GroupDocs.Search.Options.NumberOfThreads.Default , ce qui signifie que la recherche sera effectuée en utilisant un nombre de threads égal au nombre de cœurs du processeur.


**Returns:**
[NumberOfThreads](../../com.groupdocs.search.options/numberofthreads) - The number of threads used for the search.

### setSearchThreads(NumberOfThreads value) {#setSearchThreads-com.groupdocs.search.options.NumberOfThreads-}
```
public final void setSearchThreads(NumberOfThreads value)
```


Définit le nombre de threads utilisés pour la recherche. La valeur par défaut est  GroupDocs.Search.Options.NumberOfThreads.Default , ce qui signifie que la recherche sera effectuée en utilisant un nombre de threads égal au nombre de cœurs du processeur.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | value | [NumberOfThreads](../../com.groupdocs.search.options/numberofthreads) | Le nombre de threads utilisés pour la recherche. |
|

### getCustomExtractors() {#getCustomExtractors--}
```
public final CustomExtractorCollection getCustomExtractors()
```


Obtient la collection d'extracteurs personnalisés. L'exemple complet d'implémentation d'un extracteur personnalisé est présenté dans la documentation de l'interface  GroupDocs.Search.Common.IFieldExtractor .


**Returns:**
[CustomExtractorCollection](../../com.groupdocs.search.common/customextractorcollection) - The custom extractor collection.

### getLogger() {#getLogger--}
```
public final ILogger getLogger()
```


Obtient un logger utilisé pour consigner les événements et les erreurs dans l'index. Notez que le logger n'est pas sauvegardé et doit être créé et assigné chaque fois que l'index est créé ou chargé.


**Returns:**
[ILogger](../../com.groupdocs.search.common/ilogger) - A logger that is used for logging events and errors in the index.

### setLogger(ILogger value) {#setLogger-com.groupdocs.search.common.ILogger-}
```
public final void setLogger(ILogger value)
```


Définit un journaliseur utilisé pour consigner les événements et les erreurs dans l'index. Notez que le journaliseur n'est pas enregistré et doit être créé et attribué chaque fois que l'index est créé ou chargé.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | value | [ILogger](../../com.groupdocs.search.common/ilogger) | Un journaliseur utilisé pour consigner les événements et les erreurs dans l'index. |
|

