---
title: "TableDiscreteFunction"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Représente l'algorithme de recherche floue qui contient des correspondances entre la longueur des mots et le nombre d'erreurs autorisées."
type: docs
weight: 40
url: /fr/java/com.groupdocs.search.options/tablediscretefunction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.options.FuzzyAlgorithm](../../com.groupdocs.search.options/fuzzyalgorithm)
```
public class TableDiscreteFunction extends FuzzyAlgorithm
```

Représente l'algorithme de recherche floue qui contient des correspondances entre les longueurs de mots et le nombre d'erreurs autorisées. Cet algorithme peut être spécifié par une table de valeurs de sortie ou par une fonction d'étape.


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
options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(1, new Step(5, 2), new Step(8, 3))); // Création de l'algorithme de recherche floue
// Cette fonction spécifie 1 comme nombre maximal d'erreurs pour les mots de 1 à 4 caractères.
// Elle spécifie 2 comme nombre maximal d'erreurs pour les mots de 5 à 7 caractères.
// Elle spécifie 3 comme nombre maximal d'erreurs pour les mots de 8 caractères et plus.
SearchResult result = index.search(query, options); // Rechercher dans l'index
 
```
 
````


## Constructeurs

| Constructeur | Description |
| --- | --- |
|  | [TableDiscreteFunction(int offsetOfInputs, int[] tableOfOutputs)](#TableDiscreteFunction-int-int---) | Initialise une nouvelle instance de la classe  TableDiscreteFunction  . |
|
|  | [TableDiscreteFunction(int firstStepLevel, Step[] steps)](#TableDiscreteFunction-int-com.groupdocs.search.options.Step...-) | Initialise une nouvelle instance de la classe  TableDiscreteFunction  . |
|
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getSimilarityLevel(int termLength)](#getSimilarityLevel-int-) | Obtient un niveau de similarité pour la longueur de terme spécifiée. |
|
|  | [getMaxMistakeCount(int termLength)](#getMaxMistakeCount-int-) | Obtient le nombre maximal d'erreurs autorisées pour la longueur de terme spécifiée. |
|
### TableDiscreteFunction(int offsetOfInputs, int[] tableOfOutputs) {#TableDiscreteFunction-int-int---}
```
public TableDiscreteFunction(int offsetOfInputs, int[] tableOfOutputs)
```


Initialise une nouvelle instance de la classe  TableDiscreteFunction  .


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | offsetOfInputs | int | Le décalage des indices du tableau par rapport aux valeurs d'entrée. |
|
|  | tableOfOutputs | int[] | Le tableau des valeurs de sortie. |
|

### TableDiscreteFunction(int firstStepLevel, Step[] steps) {#TableDiscreteFunction-int-com.groupdocs.search.options.Step...-}
```
public TableDiscreteFunction(int firstStepLevel, Step[] steps)
```


Initialise une nouvelle instance de la classe  TableDiscreteFunction  .


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | firstStepLevel | int | Le niveau de la première étape de la fonction d'escalier. |
|
|  | steps | [Step\[\]](../../com.groupdocs.search.options/step) | Les étapes suivantes de la fonction d'escalier. |
|

### getSimilarityLevel(int termLength) {#getSimilarityLevel-int-}
```
public double getSimilarityLevel(int termLength)
```


Obtient un niveau de similarité pour la longueur de terme spécifiée.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | termLength | int | La longueur du terme. |
|

**Returns:**
double - Un niveau de similarité.

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
int - Un nombre maximal d'erreurs autorisées.

