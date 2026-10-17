---
title: "SpellingCorrectorOptions"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Fournit des options pour le correcteur orthographique."
type: docs
weight: 36
url: /fr/java/com.groupdocs.search.options/spellingcorrectoroptions/
---
**Inheritance:**
java.lang.Object
```
public abstract class SpellingCorrectorOptions
```

Fournit des options pour le correcteur orthographique.


**Learn more**

* [Spell checking](../https://docs.groupdocs.com/display/searchjava/Spell+checking)
* [Search options](../https://docs.groupdocs.com/display/searchjava/Search+options)

## Constructeurs

| Constructeur | Description |
| --- | --- |
| [SpellingCorrectorOptions()](#SpellingCorrectorOptions--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getEnabled()](#getEnabled--) | Obtient une valeur indiquant si le correcteur orthographique est activé. |
|
|  | [setEnabled(boolean value)](#setEnabled-boolean-) | Définit une valeur indiquant si le correcteur orthographique est activé. |
|
|  | [getMaxMistakeCount()](#getMaxMistakeCount--) | Obtient le nombre maximal d'erreurs. |
|
|  | [setMaxMistakeCount(int value)](#setMaxMistakeCount-int-) | Définit le nombre maximal d'erreurs. |
|
|  | [getOnlyBestResults()](#getOnlyBestResults--) | Obtient une valeur indiquant si seuls les meilleurs résultats seront retournés. |
|
|  | [setOnlyBestResults(boolean value)](#setOnlyBestResults-boolean-) | Définit une valeur indiquant si seuls les meilleurs résultats seront retournés. |
|
|  | [getOnlyBestResultsRange()](#getOnlyBestResultsRange--) | Obtient le dépassement maximal du nombre minimum d'erreurs trouvées. |
|
|  | [setOnlyBestResultsRange(byte value)](#setOnlyBestResultsRange-byte-) | Définit le dépassement maximal du nombre minimum d'erreurs trouvées. |
|
|  | [getConsiderTranspositions()](#getConsiderTranspositions--) | Obtient une valeur indiquant si l'algorithme doit considérer la transposition de deux caractères adjacents comme une seule erreur. |
|
|  | [setConsiderTranspositions(boolean value)](#setConsiderTranspositions-boolean-) | Définit une valeur indiquant si l'algorithme doit considérer la transposition de deux caractères adjacents comme une seule erreur. |
|
### SpellingCorrectorOptions() {#SpellingCorrectorOptions--}
```
public SpellingCorrectorOptions()
```


### getEnabled() {#getEnabled--}
```
public abstract boolean getEnabled()
```


Obtient une valeur indiquant si le correcteur orthographique est activé. La valeur par défaut est false.


**Returns:**
boolean - Une valeur indiquant si le correcteur orthographique est activé.

### setEnabled(boolean value) {#setEnabled-boolean-}
```
public abstract void setEnabled(boolean value)
```


Définit une valeur indiquant si le correcteur orthographique est activé. La valeur par défaut est false.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | valeur | boolean | Une valeur indiquant si le correcteur orthographique est activé. |
|

### getMaxMistakeCount() {#getMaxMistakeCount--}
```
public abstract int getMaxMistakeCount()
```


Obtient le nombre maximal d'erreurs. La valeur par défaut est 2.


**Returns:**
int - Le nombre maximal d'erreurs.

### setMaxMistakeCount(int value) {#setMaxMistakeCount-int-}
```
public abstract void setMaxMistakeCount(int value)
```


Définit le nombre maximal d'erreurs. La valeur par défaut est  2 .


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | valeur | int | Le nombre maximal d'erreurs. |
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


Obtient une valeur indiquant si l'algorithme doit considérer la transposition de deux caractères adjacents comme une seule erreur. La valeur par défaut est  true .


**Returns:**
boolean -  true  si l'algorithme de correction orthographique considère les transpositions ; sinon  false .

### setConsiderTranspositions(boolean value) {#setConsiderTranspositions-boolean-}
```
public abstract void setConsiderTranspositions(boolean value)
```


Définit une valeur indiquant si l'algorithme doit considérer la transposition de deux caractères adjacents comme une seule erreur. La valeur par défaut est  true .


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | valeur | boolean | true  si l'algorithme de correction orthographique considère les transpositions ; sinon  false . |
|

