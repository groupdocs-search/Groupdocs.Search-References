---
title: "SpellingCorrectorOptions"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Fornisce opzioni per il correttore ortografico."
type: docs
weight: 36
url: /it/java/com.groupdocs.search.options/spellingcorrectoroptions/
---
**Inheritance:**
java.lang.Object
```
public abstract class SpellingCorrectorOptions
```

Fornisce opzioni per il correttore ortografico.


**Learn more**

* [Spell checking](../https://docs.groupdocs.com/display/searchjava/Spell+checking)
* [Search options](../https://docs.groupdocs.com/display/searchjava/Search+options)

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [SpellingCorrectorOptions()](#SpellingCorrectorOptions--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getEnabled()](#getEnabled--) | Restituisce un valore che indica se il correttore ortografico è abilitato. |
|
|  | [setEnabled(boolean value)](#setEnabled-boolean-) | Imposta un valore che indica se il correttore ortografico è abilitato. |
|
|  | [getMaxMistakeCount()](#getMaxMistakeCount--) | Restituisce il numero massimo di errori. |
|
|  | [setMaxMistakeCount(int value)](#setMaxMistakeCount-int-) | Imposta il numero massimo di errori. |
|
|  | [getOnlyBestResults()](#getOnlyBestResults--) | Restituisce un valore che indica se verranno restituiti solo i risultati migliori. |
|
|  | [setOnlyBestResults(boolean value)](#setOnlyBestResults-boolean-) | Imposta un valore che indica se verranno restituiti solo i risultati migliori. |
|
|  | [getOnlyBestResultsRange()](#getOnlyBestResultsRange--) | Restituisce il superamento massimo del numero minimo di errori trovati. |
|
|  | [setOnlyBestResultsRange(byte value)](#setOnlyBestResultsRange-byte-) | Imposta il superamento massimo del numero minimo di errori trovati. |
|
|  | [getConsiderTranspositions()](#getConsiderTranspositions--) | Restituisce un valore che indica se l'algoritmo deve considerare la trasposizione di due caratteri adiacenti come un singolo errore. |
|
|  | [setConsiderTranspositions(boolean value)](#setConsiderTranspositions-boolean-) | Imposta un valore che indica se l'algoritmo deve considerare la trasposizione di due caratteri adiacenti come un singolo errore. |
|
### SpellingCorrectorOptions() {#SpellingCorrectorOptions--}
```
public SpellingCorrectorOptions()
```


### getEnabled() {#getEnabled--}
```
public abstract boolean getEnabled()
```


Restituisce un valore che indica se il correttore ortografico è abilitato. Il valore predefinito è false.


**Returns:**
boolean - Un valore che indica se il correttore ortografico è abilitato.

### setEnabled(boolean value) {#setEnabled-boolean-}
```
public abstract void setEnabled(boolean value)
```


Imposta un valore che indica se il correttore ortografico è abilitato. Il valore predefinito è false.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | boolean | Un valore che indica se il correttore ortografico è abilitato. |
|

### getMaxMistakeCount() {#getMaxMistakeCount--}
```
public abstract int getMaxMistakeCount()
```


Restituisce il numero massimo di errori. Il valore predefinito è 2.


**Returns:**
int - Il numero massimo di errori.

### setMaxMistakeCount(int value) {#setMaxMistakeCount-int-}
```
public abstract void setMaxMistakeCount(int value)
```


Imposta il numero massimo di errori. Il valore predefinito è  2 .


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | int | Il numero massimo di errori. |
|

### getOnlyBestResults() {#getOnlyBestResults--}
```
public abstract boolean getOnlyBestResults()
```


Ottiene un valore che indica se verranno restituiti solo i risultati migliori. Il valore predefinito è  false .


**Returns:**
boolean -  true  se verranno restituiti solo i risultati migliori; altrimenti  false .

### setOnlyBestResults(boolean value) {#setOnlyBestResults-boolean-}
```
public abstract void setOnlyBestResults(boolean value)
```


Imposta un valore che indica se verranno restituiti solo i risultati migliori. Il valore predefinito è  false .


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | boolean | true  se verranno restituiti solo i risultati migliori; altrimenti  false . |
|

### getOnlyBestResultsRange() {#getOnlyBestResultsRange--}
```
public abstract byte getOnlyBestResultsRange()
```


Ottiene il superamento massimo del numero minimo di errori trovato. Il valore predefinito è  0 .


**Returns:**
byte - Il superamento massimo del numero minimo di errori trovato.

### setOnlyBestResultsRange(byte value) {#setOnlyBestResultsRange-byte-}
```
public abstract void setOnlyBestResultsRange(byte value)
```


Imposta il superamento massimo del numero minimo di errori trovato. Il valore predefinito è  0 .


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | byte | Il superamento massimo del numero minimo di errori trovato. |
|

### getConsiderTranspositions() {#getConsiderTranspositions--}
```
public abstract boolean getConsiderTranspositions()
```


Ottiene un valore che indica se l'algoritmo deve considerare la trasposizione di due caratteri adiacenti come un singolo errore. Il valore predefinito è  true .


**Returns:**
boolean -  true  se l'algoritmo correttore ortografico considera le trasposizioni; altrimenti  false .

### setConsiderTranspositions(boolean value) {#setConsiderTranspositions-boolean-}
```
public abstract void setConsiderTranspositions(boolean value)
```


Imposta un valore che indica se l'algoritmo deve considerare la trasposizione di due caratteri adiacenti come un singolo errore. Il valore predefinito è  true .


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | boolean | true  se l'algoritmo correttore ortografico considera le trasposizioni; altrimenti  false . |
|

