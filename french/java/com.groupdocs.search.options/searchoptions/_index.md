---
title: "SearchOptions"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Fournit des options pour l'opération de recherche."
type: docs
weight: 34
url: /fr/java/com.groupdocs.search.options/searchoptions/
---
**Inheritance:**
java.lang.Object
```
public class SearchOptions
```

Fournit des options pour l'opération de recherche.


**Learn more**

* [Search options](../https://docs.groupdocs.com/display/searchjava/Search+options)

## Constructeurs

| Constructeur | Description |
| --- | --- |
|  | [SearchOptions()](#SearchOptions--) | Initialise une nouvelle instance de la classe  SearchOptions . |
|
|  | [SearchOptions(Object data)](#SearchOptions-java.lang.Object-) | Initialise une nouvelle instance de la classe  SearchOptions . |
|
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getUseSynonymSearch()](#getUseSynonymSearch--) | Obtient le drapeau d'utilisation des synonymes dans la recherche. |
|
|  | [setUseSynonymSearch(boolean value)](#setUseSynonymSearch-boolean-) | Définit le drapeau d'utilisation des synonymes dans la recherche. |
|
|  | [getUseHomophoneSearch()](#getUseHomophoneSearch--) | Obtient le drapeau d'utilisation des homophones dans la recherche. |
|
|  | [setUseHomophoneSearch(boolean value)](#setUseHomophoneSearch-boolean-) | Définit le drapeau d'utilisation des homophones dans la recherche. |
|
|  | [getUseWordFormsSearch()](#getUseWordFormsSearch--) | Obtient le drapeau d'utilisation des différentes formes de mots dans la recherche. |
|
|  | [setUseWordFormsSearch(boolean value)](#setUseWordFormsSearch-boolean-) | Définit le drapeau d'utilisation des différentes formes de mots dans la recherche. |
|
|  | [getRetrieveAttributes()](#getRetrieveAttributes--) | Obtient le drapeau de récupération des attributs associés aux documents trouvés. |
|
|  | [setRetrieveAttributes(boolean value)](#setRetrieveAttributes-boolean-) | Définit le drapeau de récupération des attributs associés aux documents trouvés. |
|
|  | [getFuzzySearch()](#getFuzzySearch--) | Obtient les options de recherche floue. |
|
|  | [getSpellingCorrector()](#getSpellingCorrector--) | Obtient les options du correcteur orthographique. |
|
|  | [getKeyboardLayoutCorrector()](#getKeyboardLayoutCorrector--) | Obtient les options du correcteur de disposition du clavier. |
|
|  | [getUseCaseSensitiveSearch()](#getUseCaseSensitiveSearch--) | Obtient le drapeau de recherche sensible à la casse. |
|
|  | [setUseCaseSensitiveSearch(boolean value)](#setUseCaseSensitiveSearch-boolean-) | Définit le drapeau de recherche sensible à la casse. |
|
|  | [getMaxTotalOccurrenceCount()](#getMaxTotalOccurrenceCount--) | Obtient le nombre total maximal d'occurrences de tous les termes dans une requête de recherche. |
|
|  | [setMaxTotalOccurrenceCount(int value)](#setMaxTotalOccurrenceCount-int-) | Définit le nombre total maximal d'occurrences de tous les termes dans une requête de recherche. |
|
|  | [getMaxOccurrenceCountPerTerm()](#getMaxOccurrenceCountPerTerm--) | Obtient le nombre maximal d'occurrences de chaque terme dans une requête de recherche. |
|
|  | [setMaxOccurrenceCountPerTerm(int value)](#setMaxOccurrenceCountPerTerm-int-) | Définit le nombre maximal d'occurrences de chaque terme dans une requête de recherche. |
|
|  | [getDateFormats()](#getDateFormats--) | Obtient la collection de formats de date pour la recherche par intervalle de dates. |
|
|  | [isChunkSearch()](#isChunkSearch--) | Obtient le drapeau de recherche par morceaux. |
|
|  | [setChunkSearch(boolean value)](#setChunkSearch-boolean-) | Définit le drapeau de recherche par morceaux. |
|
|  | [getSearchDocumentFilter()](#getSearchDocumentFilter--) | Obtient le filtre de document de recherche. |
|
|  | [setSearchDocumentFilter(ISearchDocumentFilter value)](#setSearchDocumentFilter-com.groupdocs.search.options.ISearchDocumentFilter-) | Définit le filtre de documents de recherche. |
|
|  | [getCancellation()](#getCancellation--) | Obtient l'objet d'annulation de l'opération. |
|
|  | [setCancellation(Cancellation value)](#setCancellation-com.groupdocs.search.common.Cancellation-) | Définit l'objet d'annulation de l'opération. |
|
| [getCore()](#getCore--) |  |
### SearchOptions() {#SearchOptions--}
```
public SearchOptions()
```


Initialise une nouvelle instance de la classe  SearchOptions .


### SearchOptions(Object data) {#SearchOptions-java.lang.Object-}
```
public SearchOptions(Object data)
```


Initialise une nouvelle instance de la classe  SearchOptions .


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | données | java.lang.Object | Les données sérialisées. |
|

### getUseSynonymSearch() {#getUseSynonymSearch--}
```
public boolean getUseSynonymSearch()
```


Obtient le drapeau d'utilisation des synonymes dans la recherche. La valeur par défaut est false.


**Returns:**
boolean - Le drapeau d'utilisation des synonymes dans la recherche.

### setUseSynonymSearch(boolean value) {#setUseSynonymSearch-boolean-}
```
public void setUseSynonymSearch(boolean value)
```


Définit le drapeau d'utilisation des synonymes dans la recherche. La valeur par défaut est false.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | valeur | boolean | Le drapeau d'utilisation des synonymes dans la recherche. |
|

### getUseHomophoneSearch() {#getUseHomophoneSearch--}
```
public boolean getUseHomophoneSearch()
```


Obtient le drapeau d'utilisation des homophones dans la recherche. La valeur par défaut est false.


**Returns:**
boolean - Le drapeau d'utilisation des homophones dans la recherche.

### setUseHomophoneSearch(boolean value) {#setUseHomophoneSearch-boolean-}
```
public void setUseHomophoneSearch(boolean value)
```


Définit le drapeau d'utilisation des homophones dans la recherche. La valeur par défaut est false.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | valeur | boolean | Le drapeau d'utilisation des homophones dans la recherche. |
|

### getUseWordFormsSearch() {#getUseWordFormsSearch--}
```
public boolean getUseWordFormsSearch()
```


Obtient le drapeau d'utilisation des différentes formes de mots dans la recherche. La valeur par défaut est false.


**Returns:**
boolean - Le drapeau d'utilisation des différentes formes de mots dans la recherche.

### setUseWordFormsSearch(boolean value) {#setUseWordFormsSearch-boolean-}
```
public void setUseWordFormsSearch(boolean value)
```


Définit le drapeau d'utilisation des différentes formes de mots dans la recherche. La valeur par défaut est false.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | valeur | boolean | Le drapeau d'utiliser différentes formes de mots dans la recherche. |
|

### getRetrieveAttributes() {#getRetrieveAttributes--}
```
public boolean getRetrieveAttributes()
```


Obtient le drapeau de récupération des attributs associés aux documents trouvés. La valeur par défaut est false.


**Returns:**
booléen - Le drapeau de récupération des attributs associés aux documents trouvés.

### setRetrieveAttributes(boolean value) {#setRetrieveAttributes-boolean-}
```
public void setRetrieveAttributes(boolean value)
```


Définit le drapeau de récupération des attributs associés aux documents trouvés. La valeur par défaut est false.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | valeur | boolean | Le drapeau de récupération des attributs associés aux documents trouvés. |
|

### getFuzzySearch() {#getFuzzySearch--}
```
public FuzzySearchOptions getFuzzySearch()
```


Obtient les options de recherche floue.


**Returns:**
[FuzzySearchOptions](../../com.groupdocs.search.options/fuzzysearchoptions) - The fuzzy search options.

### getSpellingCorrector() {#getSpellingCorrector--}
```
public SpellingCorrectorOptions getSpellingCorrector()
```


Obtient les options du correcteur orthographique.


**Returns:**
[SpellingCorrectorOptions](../../com.groupdocs.search.options/spellingcorrectoroptions) - The spelling corrector options.

### getKeyboardLayoutCorrector() {#getKeyboardLayoutCorrector--}
```
public KeyboardLayoutCorrectorOptions getKeyboardLayoutCorrector()
```


Obtient les options du correcteur de disposition du clavier.


**Returns:**
[KeyboardLayoutCorrectorOptions](../../com.groupdocs.search.options/keyboardlayoutcorrectoroptions) - The keyboard layout corrector options.

### getUseCaseSensitiveSearch() {#getUseCaseSensitiveSearch--}
```
public boolean getUseCaseSensitiveSearch()
```


Obtient le drapeau de recherche sensible à la casse. La valeur par défaut est false.


**Returns:**
booléen - Le drapeau de recherche sensible à la casse.

### setUseCaseSensitiveSearch(boolean value) {#setUseCaseSensitiveSearch-boolean-}
```
public void setUseCaseSensitiveSearch(boolean value)
```


Définit le drapeau de recherche sensible à la casse. La valeur par défaut est false.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | valeur | boolean | Le drapeau de recherche sensible à la casse. |
|

### getMaxTotalOccurrenceCount() {#getMaxTotalOccurrenceCount--}
```
public int getMaxTotalOccurrenceCount()
```


Obtient le nombre total maximal d'occurrences de tous les termes dans une requête de recherche. La valeur par défaut est 500000.


**Returns:**
int - Le nombre total maximal d'occurrences.

### setMaxTotalOccurrenceCount(int value) {#setMaxTotalOccurrenceCount-int-}
```
public void setMaxTotalOccurrenceCount(int value)
```


Définit le nombre total maximal d'occurrences de tous les termes dans une requête de recherche. La valeur par défaut est 500000.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | valeur | int | Le nombre total maximal d'occurrences. |
|

### getMaxOccurrenceCountPerTerm() {#getMaxOccurrenceCountPerTerm--}
```
public int getMaxOccurrenceCountPerTerm()
```


Obtient le nombre maximal d'occurrences de chaque terme dans une requête de recherche. La valeur par défaut est 100000.


**Returns:**
int - Le nombre maximal d'occurrences de chaque terme dans une requête de recherche.

### setMaxOccurrenceCountPerTerm(int value) {#setMaxOccurrenceCountPerTerm-int-}
```
public void setMaxOccurrenceCountPerTerm(int value)
```


Définit le nombre maximal d'occurrences de chaque terme dans une requête de recherche. La valeur par défaut est 100000.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | valeur | int | Le nombre maximal d'occurrences de chaque terme dans une requête de recherche. |
|

### getDateFormats() {#getDateFormats--}
```
public DateFormatCollection getDateFormats()
```


Obtient la collection de formats de date pour la recherche par intervalle de dates. Les formats de date par défaut sont 'dd.MM.yyyy', 'MM/dd/yyyy' et 'yyyy-MM-dd'.


**Returns:**
[DateFormatCollection](../../com.groupdocs.search.options/dateformatcollection) - The collection of date formats for date range search.


L'exemple montre comment définir les formats de date pour la recherche.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // Création d'un index dans le dossier spécifié
index.add(documentsFolder); // Indexation des documents depuis le dossier spécifié
SearchOptions options = new SearchOptions();
options.getDateFormats().clear(); // Suppression des formats de date par défaut
DateFormatElement[] elements = new DateFormatElement[] {
DateFormatElement.getMonthTwoDigits(),
DateFormatElement.getDayOfMonthTwoDigits(),
DateFormatElement.getYearFourDigits(),
};
// Création d'un modèle de format de date 'MM/dd/yyyy'
com.groupdocs.search.DateFormat dateFormat = new com.groupdocs.search.DateFormat(elements, "/");
options.getDateFormats().addItem(dateFormat);
SearchResult result = index.search(query, options); // Rechercher dans l'index
 
```
 
````


### isChunkSearch() {#isChunkSearch--}
```
public boolean isChunkSearch()
```


Obtient le drapeau de recherche par morceaux. La valeur par défaut est false.


**Returns:**
booléen - Le drapeau de recherche par morceaux.

### setChunkSearch(boolean value) {#setChunkSearch-boolean-}
```
public void setChunkSearch(boolean value)
```


Définit le drapeau de recherche par morceaux. La valeur par défaut est false.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | valeur | boolean | Le drapeau de recherche par morceaux. |
|

### getSearchDocumentFilter() {#getSearchDocumentFilter--}
```
public ISearchDocumentFilter getSearchDocumentFilter()
```


Obtient le filtre de document de recherche.  SearchDocumentFilter  fonctionne selon la logique d'inclusion. Utilisez la classe  SearchDocumentFilter  pour créer des instances de filtre de document de recherche. La valeur par défaut est null, ce qui signifie que tous les documents trouvés seront retournés.


**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - The search document filter.


L'exemple montre comment définir le filtre de documents.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments1\\";
// Création d'un index dans le dossier spécifié
Index index = new Index(indexFolder);
// Indexation des documents
index.add(documentsFolder);
// Création d'un filtre de documents de recherche qui ignore les documents avec les extensions '.doc', '.docx', '.rtf'
SearchOptions options = new SearchOptions();
ISearchDocumentFilter fileExtensionFilter = SearchDocumentFilter.createFileExtension(".doc", ".docx", ".rtf"); // Création du filtre d'extension de fichier
ISearchDocumentFilter invertedFilter = SearchDocumentFilter.createNot(fileExtensionFilter); // Inversion du filtre d'extension de fichier
options.setSearchDocumentFilter(invertedFilter);
// Recherche dans l'index
SearchResult result = index.search("Einstein", options);
 
```
 
````


### setSearchDocumentFilter(ISearchDocumentFilter value) {#setSearchDocumentFilter-com.groupdocs.search.options.ISearchDocumentFilter-}
```
public void setSearchDocumentFilter(ISearchDocumentFilter value)
```


Définit le filtre de documents de recherche.  SearchDocumentFilter  fonctionne selon la logique d'inclusion. Utilisez la classe  SearchDocumentFilter  pour créer des instances de filtre de documents de recherche. La valeur par défaut est  null , ce qui signifie que tous les documents trouvés seront retournés.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | value | [ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) | Le filtre de document de recherche. |


L'exemple montre comment définir le filtre de documents.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments1\\";
// Création d'un index dans le dossier spécifié
Index index = new Index(indexFolder);
// Indexation des documents
index.add(documentsFolder);
// Création d'un filtre de documents de recherche qui ignore les documents avec les extensions '.doc', '.docx', '.rtf'
SearchOptions options = new SearchOptions();
ISearchDocumentFilter fileExtensionFilter = SearchDocumentFilter.createFileExtension(".doc", ".docx", ".rtf"); // Création du filtre d'extension de fichier
ISearchDocumentFilter invertedFilter = SearchDocumentFilter.createNot(fileExtensionFilter); // Inversion du filtre d'extension de fichier
options.setSearchDocumentFilter(invertedFilter);
// Recherche dans l'index
SearchResult result = index.search("Einstein", options);
 
```
 
````

|

### getCancellation() {#getCancellation--}
```
public Cancellation getCancellation()
```


Obtient l'objet d'annulation de l'opération. La valeur par défaut est null.


**Returns:**
[Cancellation](../../com.groupdocs.search.common/cancellation) - The operation cancellation object.

### setCancellation(Cancellation value) {#setCancellation-com.groupdocs.search.common.Cancellation-}
```
public void setCancellation(Cancellation value)
```


Définit l'objet d'annulation de l'opération. La valeur par défaut est null.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | value | [Cancellation](../../com.groupdocs.search.common/cancellation) | L'objet d'annulation de l'opération. |
|

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
