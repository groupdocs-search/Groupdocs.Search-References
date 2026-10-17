---
title: "FuzzyAlgorithm"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Représente la classe de base pour les algorithmes de recherche floue."
type: docs
weight: 20
url: /fr/java/com.groupdocs.search.options/fuzzyalgorithm/
---
**Inheritance:**
java.lang.Object
```
public abstract class FuzzyAlgorithm
```

Représente la classe de base pour les algorithmes de recherche floue.


**Learn more**

* [Fuzzy search](../https://docs.groupdocs.com/display/searchjava/Fuzzy+search)

## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getSimilarityLevel(int termLength)](#getSimilarityLevel-int-) | Obtient le niveau de similarité pour la longueur de terme spécifiée. |
|
|  | [getMaxMistakeCount(int termLength)](#getMaxMistakeCount-int-) | Obtient le nombre maximal d'erreurs autorisées pour la longueur de terme spécifiée. |
|
| [getCore()](#getCore--) |  |
### getSimilarityLevel(int termLength) {#getSimilarityLevel-int-}
```
public abstract double getSimilarityLevel(int termLength)
```


Obtient le niveau de similarité pour la longueur de terme spécifiée.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | termLength | int | La longueur du terme. |
|

**Returns:**
double - Le niveau de similarité.

### getMaxMistakeCount(int termLength) {#getMaxMistakeCount-int-}
```
public abstract int getMaxMistakeCount(int termLength)
```


Obtient le nombre maximal d'erreurs autorisées pour la longueur de terme spécifiée.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | termLength | int | La longueur du terme. |
|

**Returns:**
int - Le nombre maximal d'erreurs autorisées.

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
