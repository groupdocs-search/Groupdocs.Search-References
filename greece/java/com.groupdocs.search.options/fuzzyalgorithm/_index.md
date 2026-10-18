---
title: "FuzzyAlgorithm"
second_title: "GroupDocs.Search για Java API Reference"
description: "Αναπαριστά την βασική κλάση για αλγόριθμους ασαφούς αναζήτησης."
type: docs
weight: 20
url: /el/java/com.groupdocs.search.options/fuzzyalgorithm/
---
**Inheritance:**
java.lang.Object
```
public abstract class FuzzyAlgorithm
```

Αναπαριστά την βασική κλάση για αλγόριθμους ασαφούς αναζήτησης.


**Learn more**

* [Fuzzy search](../https://docs.groupdocs.com/display/searchjava/Fuzzy+search)

## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getSimilarityLevel(int termLength)](#getSimilarityLevel-int-) | Λαμβάνει το επίπεδο ομοιότητας για το καθορισμένο μήκος όρου. |
|
|  | [getMaxMistakeCount(int termLength)](#getMaxMistakeCount-int-) | Λαμβάνει τον μέγιστο επιτρεπόμενο αριθμό λαθών για το καθορισμένο μήκος όρου. |
|
| [getCore()](#getCore--) |  |
### getSimilarityLevel(int termLength) {#getSimilarityLevel-int-}
```
public abstract double getSimilarityLevel(int termLength)
```


Λαμβάνει το επίπεδο ομοιότητας για το καθορισμένο μήκος όρου.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | termLength | int | Το μήκος του όρου. |
|

**Returns:**
double - Το επίπεδο ομοιότητας.

### getMaxMistakeCount(int termLength) {#getMaxMistakeCount-int-}
```
public abstract int getMaxMistakeCount(int termLength)
```


Λαμβάνει τον μέγιστο επιτρεπόμενο αριθμό λαθών για το καθορισμένο μήκος όρου.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | termLength | int | Το μήκος του όρου. |
|

**Returns:**
int - Μέγιστος επιτρεπτός αριθμός λαθών.

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
