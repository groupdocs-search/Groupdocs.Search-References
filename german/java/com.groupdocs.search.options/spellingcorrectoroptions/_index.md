---
title: "SpellingCorrectorOptions"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Stellt Optionen für die Rechtschreibkorrektur bereit."
type: docs
weight: 36
url: /de/java/com.groupdocs.search.options/spellingcorrectoroptions/
---
**Inheritance:**
java.lang.Object
```
public abstract class SpellingCorrectorOptions
```

Stellt Optionen für die Rechtschreibkorrektur bereit.


**Learn more**

* [Spell checking](../https://docs.groupdocs.com/display/searchjava/Spell+checking)
* [Search options](../https://docs.groupdocs.com/display/searchjava/Search+options)

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [SpellingCorrectorOptions()](#SpellingCorrectorOptions--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getEnabled()](#getEnabled--) | Gibt einen Wert zurück, der angibt, ob die Rechtschreibkorrektur aktiviert ist. |
|
|  | [setEnabled(boolean value)](#setEnabled-boolean-) | Legt einen Wert fest, der angibt, ob die Rechtschreibkorrektur aktiviert ist. |
|
|  | [getMaxMistakeCount()](#getMaxMistakeCount--) | Gibt die maximale Anzahl von Fehlern zurück. |
|
|  | [setMaxMistakeCount(int value)](#setMaxMistakeCount-int-) | Legt die maximale Anzahl von Fehlern fest. |
|
|  | [getOnlyBestResults()](#getOnlyBestResults--) | Gibt einen Wert zurück, der angibt, ob nur die besten Ergebnisse zurückgegeben werden. |
|
|  | [setOnlyBestResults(boolean value)](#setOnlyBestResults-boolean-) | Legt einen Wert fest, der angibt, ob nur die besten Ergebnisse zurückgegeben werden. |
|
|  | [getOnlyBestResultsRange()](#getOnlyBestResultsRange--) | Gibt das maximale Überschreiten der minimal gefundenen Fehleranzahl zurück. |
|
|  | [setOnlyBestResultsRange(byte value)](#setOnlyBestResultsRange-byte-) | Legt das maximale Überschreiten der minimal gefundenen Fehleranzahl fest. |
|
|  | [getConsiderTranspositions()](#getConsiderTranspositions--) | Gibt einen Wert zurück, der angibt, ob der Algorithmus die Vertauschung zweier benachbarter Zeichen als einen einzelnen Fehler betrachten muss. |
|
|  | [setConsiderTranspositions(boolean value)](#setConsiderTranspositions-boolean-) | Legt einen Wert fest, der angibt, ob der Algorithmus die Vertauschung zweier benachbarter Zeichen als einen einzelnen Fehler betrachten muss. |
|
### SpellingCorrectorOptions() {#SpellingCorrectorOptions--}
```
public SpellingCorrectorOptions()
```


### getEnabled() {#getEnabled--}
```
public abstract boolean getEnabled()
```


Gibt einen Wert zurück, der angibt, ob die Rechtschreibkorrektur aktiviert ist. Der Standardwert ist false.


**Returns:**
boolean – Ein Wert, der angibt, ob die Rechtschreibkorrektur aktiviert ist.

### setEnabled(boolean value) {#setEnabled-boolean-}
```
public abstract void setEnabled(boolean value)
```


Legt einen Wert fest, der angibt, ob die Rechtschreibkorrektur aktiviert ist. Der Standardwert ist false.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | boolean | Ein Wert, der angibt, ob die Rechtschreibkorrektur aktiviert ist. |
|

### getMaxMistakeCount() {#getMaxMistakeCount--}
```
public abstract int getMaxMistakeCount()
```


Gibt die maximale Anzahl von Fehlern zurück. Der Standardwert ist 2.


**Returns:**
int - Die maximale Anzahl von Fehlern.

### setMaxMistakeCount(int value) {#setMaxMistakeCount-int-}
```
public abstract void setMaxMistakeCount(int value)
```


Legt die maximale Anzahl von Fehlern fest. Der Standardwert ist 2.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | int | Die maximale Anzahl von Fehlern. |
|

### getOnlyBestResults() {#getOnlyBestResults--}
```
public abstract boolean getOnlyBestResults()
```


Gibt einen Wert zurück, der angibt, ob nur die besten Ergebnisse zurückgegeben werden. Der Standardwert ist false.


**Returns:**
boolean - true, wenn nur die besten Ergebnisse zurückgegeben werden; andernfalls false.

### setOnlyBestResults(boolean value) {#setOnlyBestResults-boolean-}
```
public abstract void setOnlyBestResults(boolean value)
```


Legt einen Wert fest, der angibt, ob nur die besten Ergebnisse zurückgegeben werden. Der Standardwert ist false.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | boolean | true, wenn nur die besten Ergebnisse zurückgegeben werden; andernfalls false. |
|

### getOnlyBestResultsRange() {#getOnlyBestResultsRange--}
```
public abstract byte getOnlyBestResultsRange()
```


Gibt die maximale Überschreitung der minimal gefundenen Fehleranzahl zurück. Der Standardwert ist 0.


**Returns:**
byte - Die maximale Überschreitung der minimal gefundenen Fehleranzahl.

### setOnlyBestResultsRange(byte value) {#setOnlyBestResultsRange-byte-}
```
public abstract void setOnlyBestResultsRange(byte value)
```


Legt die maximale Überschreitung der minimal gefundenen Fehleranzahl fest. Der Standardwert ist 0.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | byte | Die maximale Überschreitung der minimal gefundenen Fehleranzahl. |
|

### getConsiderTranspositions() {#getConsiderTranspositions--}
```
public abstract boolean getConsiderTranspositions()
```


Gibt einen Wert zurück, der angibt, ob der Algorithmus die Vertauschung zweier benachbarter Zeichen als einen einzigen Fehler betrachten muss. Der Standardwert ist true.


**Returns:**
boolean - true, wenn der Rechtschreibkorrekturalgorithmus Vertauschungen berücksichtigt; andernfalls false.

### setConsiderTranspositions(boolean value) {#setConsiderTranspositions-boolean-}
```
public abstract void setConsiderTranspositions(boolean value)
```


Legt einen Wert fest, der angibt, ob der Algorithmus die Vertauschung zweier benachbarter Zeichen als einen einzigen Fehler betrachten muss. Der Standardwert ist true.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | boolean | true, wenn der Rechtschreibkorrekturalgorithmus Vertauschungen berücksichtigt; andernfalls false. |
|

