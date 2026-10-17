---
title: "FuzzySearchOptions"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Fournit des options de la recherche floue."
type: docs
weight: 21
url: /fr/java/com.groupdocs.search.options/fuzzysearchoptions/
---
**Inheritance:**
java.lang.Object
```
public abstract class FuzzySearchOptions
```

Fournit des options de la recherche floue.


**Learn more**

* [Fuzzy search](../https://docs.groupdocs.com/display/searchjava/Fuzzy+search)
* [Search options](../https://docs.groupdocs.com/display/searchjava/Search+options)

## Constructeurs

| Constructeur | Description |
| --- | --- |
| [FuzzySearchOptions()](#FuzzySearchOptions--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getEnabled()](#getEnabled--) | Obtient une valeur indiquant si la fonction de recherche floue est activée. |
|
|  | [setEnabled(boolean value)](#setEnabled-boolean-) | Définit une valeur indiquant si la fonction de recherche floue est activée. |
|
|  | [getFuzzyAlgorithm()](#getFuzzyAlgorithm--) | Obtient l'algorithme de recherche floue. |
|
|  | [setFuzzyAlgorithm(FuzzyAlgorithm value)](#setFuzzyAlgorithm-com.groupdocs.search.options.FuzzyAlgorithm-) | Définit l'algorithme de recherche floue. |
|
|  | [getOnlyBestResults()](#getOnlyBestResults--) | Obtient une valeur indiquant si seuls les meilleurs résultats seront retournés. |
|
|  | [setOnlyBestResults(boolean value)](#setOnlyBestResults-boolean-) | Définit une valeur indiquant si seuls les meilleurs résultats seront retournés. |
|
|  | [getOnlyBestResultsRange()](#getOnlyBestResultsRange--) | Obtient le dépassement maximal du nombre minimum d'erreurs trouvées. |
|
|  | [setOnlyBestResultsRange(byte value)](#setOnlyBestResultsRange-byte-) | Définit le dépassement maximal du nombre minimum d'erreurs trouvées. |
|
|  | [getConsiderTranspositions()](#getConsiderTranspositions--) | Obtient une valeur indiquant si l'algorithme de recherche floue doit considérer la transposition de deux caractères adjacents comme une seule erreur. |
|
|  | [setConsiderTranspositions(boolean value)](#setConsiderTranspositions-boolean-) | Définit une valeur indiquant si l'algorithme de recherche floue doit considérer la transposition de deux caractères adjacents comme une seule erreur. |
|
### FuzzySearchOptions() {#FuzzySearchOptions--}
```
public FuzzySearchOptions()
```


### getEnabled() {#getEnabled--}
```
public abstract boolean getEnabled()
```


Obtient une valeur indiquant si la fonction de recherche floue est activée. La valeur par défaut est false.


**Returns:**
booléen - Une valeur indiquant si la fonction de recherche floue est activée.

### setEnabled(boolean value) {#setEnabled-boolean-}
```
public abstract void setEnabled(boolean value)
```


Définit une valeur indiquant si la fonction de recherche floue est activée. La valeur par défaut est false.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | valeur | boolean | Une valeur indiquant si la fonction de recherche floue est activée. |
|

### getFuzzyAlgorithm() {#getFuzzyAlgorithm--}
```
public abstract FuzzyAlgorithm getFuzzyAlgorithm()
```


Obtient l'algorithme de recherche floue. Les algorithmes de recherche floue actuellement disponibles sont SimilarityLevel et TableDiscreteFunction. La valeur par défaut est une instance de SimilarityLevel avec une valeur de niveau de similarité de 0.5.


**Returns:**
[FuzzyAlgorithm](../../com.groupdocs.search.options/fuzzyalgorithm) - The fuzzy search algorithm.


L'exemple montre comment définir l'algorithme de recherche floue.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // Création d'un index dans le dossier spécifié
index.add(documentsFolder); // Indexation des documents depuis le dossier spécifié
SearchOptions options = new SearchOptions();
options.getFuzzySearch().setEnabled(true); // Activation de la recherche floue
options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(1, new Step(5, 2), new Step(8, 3))); // Création de l'algorithme de recherche floue
// Cette fonction spécifie 1 comme nombre maximal d'erreurs pour les mots de 1 à 4 caractères.
// Elle spécifie 2 comme nombre maximal d'erreurs pour les mots de 5 à 7 caractères.
// Elle spécifie 3 comme nombre maximal d'erreurs pour les mots de 8 caractères et plus.
SearchResult result = index.search(query, options); // Rechercher dans l'index
 
```
 
````


### setFuzzyAlgorithm(FuzzyAlgorithm value) {#setFuzzyAlgorithm-com.groupdocs.search.options.FuzzyAlgorithm-}
```
public abstract void setFuzzyAlgorithm(FuzzyAlgorithm value)
```


Définit l'algorithme de recherche floue. Les algorithmes de recherche floue actuellement disponibles sont SimilarityLevel et TableDiscreteFunction. La valeur par défaut est une instance de SimilarityLevel avec une valeur de niveau de similarité de 0.5.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | value | [FuzzyAlgorithm](../../com.groupdocs.search.options/fuzzyalgorithm) | L'algorithme de recherche floue. |


L'exemple montre comment définir l'algorithme de recherche floue.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // Création d'un index dans le dossier spécifié
index.add(documentsFolder); // Indexation des documents depuis le dossier spécifié
SearchOptions options = new SearchOptions();
options.getFuzzySearch().setEnabled(true); // Activation de la recherche floue
options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(1, new Step(5, 2), new Step(8, 3))); // Création de l'algorithme de recherche floue
// Cette fonction spécifie 1 comme nombre maximal d'erreurs pour les mots de 1 à 4 caractères.
// Elle spécifie 2 comme nombre maximal d'erreurs pour les mots de 5 à 7 caractères.
// Elle spécifie 3 comme nombre maximal d'erreurs pour les mots de 8 caractères et plus.
SearchResult result = index.search(query, options); // Rechercher dans l'index
 
```
 
````

|

### getOnlyBestResults() {#getOnlyBestResults--}
```
public abstract boolean getOnlyBestResults()
```


Obtient une valeur indiquant si seuls les meilleurs résultats seront retournés. La valeur par défaut est  false .


**Returns:**
boolean -  true  si seuls les meilleurs résultats seront retournés ; sinon  false .

### setOnlyBestResults(boolean value) {#setOnlyBestResults-boolean-}
```
public abstract void setOnlyBestResults(boolean value)
```


Définit une valeur indiquant si seuls les meilleurs résultats seront retournés. La valeur par défaut est  false .


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | valeur | boolean | true  si seuls les meilleurs résultats seront retournés ; sinon  false . |
|

### getOnlyBestResultsRange() {#getOnlyBestResultsRange--}
```
public abstract byte getOnlyBestResultsRange()
```


Obtient le dépassement maximal du nombre minimal d'erreurs trouvé. La valeur par défaut est  0 .


**Returns:**
byte - Le dépassement maximal du nombre minimal d'erreurs trouvé.

### setOnlyBestResultsRange(byte value) {#setOnlyBestResultsRange-byte-}
```
public abstract void setOnlyBestResultsRange(byte value)
```


Définit le dépassement maximal du nombre minimal d'erreurs trouvé. La valeur par défaut est  0 .


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | valeur | byte | Le dépassement maximal du nombre minimal d'erreurs trouvé. |
|

### getConsiderTranspositions() {#getConsiderTranspositions--}
```
public abstract boolean getConsiderTranspositions()
```


Obtient une valeur indiquant si l'algorithme de recherche floue doit considérer la transposition de deux caractères adjacents comme une seule erreur. La valeur par défaut est true.


**Returns:**
booléen - true si l'algorithme de recherche floue considère les transpositions ; sinon false.

### setConsiderTranspositions(boolean value) {#setConsiderTranspositions-boolean-}
```
public abstract void setConsiderTranspositions(boolean value)
```


Définit une valeur indiquant si l'algorithme de recherche floue doit considérer la transposition de deux caractères adjacents comme une seule erreur. La valeur par défaut est true.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | valeur | boolean | : true si l'algorithme de recherche floue considère les transpositions ; sinon false. |
|

