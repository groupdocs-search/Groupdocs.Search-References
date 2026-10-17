---
title: "SimilarityLevel"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Représente un algorithme de recherche floue qui spécifie le niveau de similarité."
type: docs
weight: 35
url: /fr/java/com.groupdocs.search.options/similaritylevel/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.options.FuzzyAlgorithm](../../com.groupdocs.search.options/fuzzyalgorithm)
```
public class SimilarityLevel extends FuzzyAlgorithm
```

Représente un algorithme de recherche floue qui spécifie le niveau de similarité. L'algorithme de niveau de similarité calcule le nombre maximal d'erreurs pour un mot inversement proportionnel à la longueur du mot.


**Learn more**

* [Fuzzy search](../https://docs.groupdocs.com/display/searchjava/Fuzzy+search)


L'exemple montre une utilisation typique de la classe.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // Création d'un index dans le dossier spécifié
index.add(documentsFolder); // Indexation des documents depuis le dossier spécifié
SearchOptions options = new SearchOptions();
options.getFuzzySearch().setEnabled(true); // Activation de la recherche floue
options.getFuzzySearch().setFuzzyAlgorithm(new SimilarityLevel(0.8)); // Création de l'algorithme de recherche floue
// Cette fonction spécifie 0 comme nombre maximal d'erreurs pour les mots de 1 à 4 caractères.
// Elle spécifie 1 comme nombre maximal d'erreurs pour les mots de 5 à 9 caractères.
// Elle spécifie 2 comme nombre maximal d'erreurs pour les mots de 10 à 14 caractères. Et ainsi de suite.
SearchResult result = index.search(query, options); // Rechercher dans l'index
 
```
 
````


## Constructeurs

| Constructeur | Description |
| --- | --- |
|  | [SimilarityLevel(double value)](#SimilarityLevel-double-) | Initialise une nouvelle instance de la classe  SimilarityLevel . |
|
|  | [SimilarityLevel(Object data)](#SimilarityLevel-java.lang.Object-) | Initialise une nouvelle instance de la classe  SimilarityLevel . |
|
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getSimilarityLevel(int termLength)](#getSimilarityLevel-int-) | Obtient la valeur du niveau de similarité pour la longueur de terme spécifiée. |
|
|  | [getMaxMistakeCount(int termLength)](#getMaxMistakeCount-int-) | Obtient le nombre maximal d'erreurs autorisées pour la longueur de terme spécifiée. |
|
### SimilarityLevel(double value) {#SimilarityLevel-double-}
```
public SimilarityLevel(double value)
```


Initialise une nouvelle instance de la classe  SimilarityLevel .


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | valeur | double | La valeur du niveau de similarité. |
|

### SimilarityLevel(Object data) {#SimilarityLevel-java.lang.Object-}
```
public SimilarityLevel(Object data)
```


Initialise une nouvelle instance de la classe  SimilarityLevel .


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | données | java.lang.Object | Les données sérialisées. |
|

### getSimilarityLevel(int termLength) {#getSimilarityLevel-int-}
```
public double getSimilarityLevel(int termLength)
```


Obtient la valeur du niveau de similarité pour la longueur de terme spécifiée.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | termLength | int | La longueur du terme. |
|

**Returns:**
double - La valeur du niveau de similarité.

### getMaxMistakeCount(int termLength) {#getMaxMistakeCount-int-}
```
public int getMaxMistakeCount(int termLength)
```


Obtient le nombre maximal d'erreurs autorisées pour la longueur de terme spécifiée.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | termLength | int | La longueur du terme. |
|

**Returns:**
int - Le nombre maximal d'erreurs autorisées.

