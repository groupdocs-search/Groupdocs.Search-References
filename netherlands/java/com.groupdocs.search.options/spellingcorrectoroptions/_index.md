---
title: "SpellingCorrectorOptions"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Biedt opties voor de spellingscorrector."
type: docs
weight: 36
url: /nl/java/com.groupdocs.search.options/spellingcorrectoroptions/
---
**Inheritance:**
java.lang.Object
```
public abstract class SpellingCorrectorOptions
```

Biedt opties voor de spellingscorrector.


**Learn more**

* [Spell checking](../https://docs.groupdocs.com/display/searchjava/Spell+checking)
* [Search options](../https://docs.groupdocs.com/display/searchjava/Search+options)

## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [SpellingCorrectorOptions()](#SpellingCorrectorOptions--) |  |
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getEnabled()](#getEnabled--) | Haalt een waarde op die aangeeft of de spellingcorrector is ingeschakeld. |
|
|  | [setEnabled(boolean value)](#setEnabled-boolean-) | Stelt een waarde in die aangeeft of de spellingcorrector is ingeschakeld. |
|
|  | [getMaxMistakeCount()](#getMaxMistakeCount--) | Haalt het maximum aantal fouten op. |
|
|  | [setMaxMistakeCount(int value)](#setMaxMistakeCount-int-) | Stelt het maximum aantal fouten in. |
|
|  | [getOnlyBestResults()](#getOnlyBestResults--) | Haalt een waarde op die aangeeft of alleen de beste resultaten worden geretourneerd. |
|
|  | [setOnlyBestResults(boolean value)](#setOnlyBestResults-boolean-) | Stelt een waarde in die aangeeft of alleen de beste resultaten worden geretourneerd. |
|
|  | [getOnlyBestResultsRange()](#getOnlyBestResultsRange--) | Haalt de maximale overschrijding van het minimum aantal gevonden fouten op. |
|
|  | [setOnlyBestResultsRange(byte value)](#setOnlyBestResultsRange-byte-) | Stelt de maximale overschrijding van het minimum aantal gevonden fouten in. |
|
|  | [getConsiderTranspositions()](#getConsiderTranspositions--) | Haalt een waarde op die aangeeft of het algoritme transpositie van twee aangrenzende tekens als één fout moet beschouwen. |
|
|  | [setConsiderTranspositions(boolean value)](#setConsiderTranspositions-boolean-) | Stelt een waarde in die aangeeft of het algoritme transpositie van twee aangrenzende tekens als één fout moet beschouwen. |
|
### SpellingCorrectorOptions() {#SpellingCorrectorOptions--}
```
public SpellingCorrectorOptions()
```


### getEnabled() {#getEnabled--}
```
public abstract boolean getEnabled()
```


Haalt een waarde op die aangeeft of de spellingcorrector is ingeschakeld. De standaardwaarde is false.


**Returns:**
boolean - Een waarde die aangeeft of de spellingcorrector is ingeschakeld.

### setEnabled(boolean value) {#setEnabled-boolean-}
```
public abstract void setEnabled(boolean value)
```


Stelt een waarde in die aangeeft of de spellingcorrector is ingeschakeld. De standaardwaarde is false.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | waarde | boolean | Een waarde die aangeeft of de spellingcorrector is ingeschakeld. |
|

### getMaxMistakeCount() {#getMaxMistakeCount--}
```
public abstract int getMaxMistakeCount()
```


Haalt het maximum aantal fouten op. De standaardwaarde is 2.


**Returns:**
int - Het maximum aantal fouten.

### setMaxMistakeCount(int value) {#setMaxMistakeCount-int-}
```
public abstract void setMaxMistakeCount(int value)
```


Stelt het maximum aantal fouten in. De standaardwaarde is  2 .


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | waarde | int | Het maximum aantal fouten. |
|

### getOnlyBestResults() {#getOnlyBestResults--}
```
public abstract boolean getOnlyBestResults()
```


Haalt een waarde op die aangeeft of alleen de beste resultaten worden geretourneerd. De standaardwaarde is  false .


**Returns:**
boolean -  true  als alleen de beste resultaten worden geretourneerd; anders  false .

### setOnlyBestResults(boolean value) {#setOnlyBestResults-boolean-}
```
public abstract void setOnlyBestResults(boolean value)
```


Stelt een waarde in die aangeeft of alleen de beste resultaten worden geretourneerd. De standaardwaarde is  false .


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | waarde | boolean | true  als alleen de beste resultaten worden geretourneerd; anders  false . |
|

### getOnlyBestResultsRange() {#getOnlyBestResultsRange--}
```
public abstract byte getOnlyBestResultsRange()
```


Haalt het maximale overschrijding van het minimum aantal gevonden fouten op. De standaardwaarde is  0 .


**Returns:**
byte - Het maximale overschrijding van het minimum aantal gevonden fouten.

### setOnlyBestResultsRange(byte value) {#setOnlyBestResultsRange-byte-}
```
public abstract void setOnlyBestResultsRange(byte value)
```


Stelt het maximale overschrijding van het minimum aantal gevonden fouten in. De standaardwaarde is  0 .


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | waarde | byte | Het maximale overschrijding van het minimum aantal gevonden fouten. |
|

### getConsiderTranspositions() {#getConsiderTranspositions--}
```
public abstract boolean getConsiderTranspositions()
```


Haalt een waarde op die aangeeft of het algoritme transpositie van twee aangrenzende tekens als één fout moet beschouwen. De standaardwaarde is  true .


**Returns:**
boolean -  true  als het spellingcorrectie-algoritme transposities beschouwt; anders  false .

### setConsiderTranspositions(boolean value) {#setConsiderTranspositions-boolean-}
```
public abstract void setConsiderTranspositions(boolean value)
```


Stelt een waarde in die aangeeft of het algoritme transpositie van twee aangrenzende tekens als één fout moet beschouwen. De standaardwaarde is  true .


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | waarde | boolean | true  als het spellingcorrectie-algoritme transposities beschouwt; anders  false . |
|

