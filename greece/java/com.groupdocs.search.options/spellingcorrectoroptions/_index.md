---
title: "SpellingCorrectorOptions"
second_title: "GroupDocs.Search για Java API Reference"
description: "Παρέχει επιλογές για το διορθωτή ορθογραφίας."
type: docs
weight: 36
url: /el/java/com.groupdocs.search.options/spellingcorrectoroptions/
---
**Inheritance:**
java.lang.Object
```
public abstract class SpellingCorrectorOptions
```

Παρέχει επιλογές για το διορθωτή ορθογραφίας.


**Learn more**

* [Spell checking](../https://docs.groupdocs.com/display/searchjava/Spell+checking)
* [Search options](../https://docs.groupdocs.com/display/searchjava/Search+options)

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [SpellingCorrectorOptions()](#SpellingCorrectorOptions--) |  |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getEnabled()](#getEnabled--) | Λαμβάνει μια τιμή που υποδεικνύει εάν ο διορθωτής ορθογραφίας είναι ενεργοποιημένος. |
|
|  | [setEnabled(boolean value)](#setEnabled-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν ο διορθωτής ορθογραφίας είναι ενεργοποιημένος. |
|
|  | [getMaxMistakeCount()](#getMaxMistakeCount--) | Λαμβάνει τον μέγιστο αριθμό λαθών. |
|
|  | [setMaxMistakeCount(int value)](#setMaxMistakeCount-int-) | Ορίζει τον μέγιστο αριθμό λαθών. |
|
|  | [getOnlyBestResults()](#getOnlyBestResults--) | Λαμβάνει μια τιμή που υποδεικνύει εάν θα επιστραφούν μόνο τα καλύτερα αποτελέσματα. |
|
|  | [setOnlyBestResults(boolean value)](#setOnlyBestResults-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν θα επιστραφούν μόνο τα καλύτερα αποτελέσματα. |
|
|  | [getOnlyBestResultsRange()](#getOnlyBestResultsRange--) | Λαμβάνει τη μέγιστη υπέρβαση του ελάχιστου αριθμού λαθών που εντοπίζονται. |
|
|  | [setOnlyBestResultsRange(byte value)](#setOnlyBestResultsRange-byte-) | Ορίζει τη μέγιστη υπέρβαση του ελάχιστου αριθμού λαθών που εντοπίζονται. |
|
|  | [getConsiderTranspositions()](#getConsiderTranspositions--) | Λαμβάνει μια τιμή που υποδεικνύει εάν ο αλγόριθμος πρέπει να θεωρεί τη μετατόπιση δύο διαδοχικών χαρακτήρων ως ένα μόνο λάθος. |
|
|  | [setConsiderTranspositions(boolean value)](#setConsiderTranspositions-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν ο αλγόριθμος πρέπει να θεωρεί τη μετατόπιση δύο διαδοχικών χαρακτήρων ως ένα μόνο λάθος. |
|
### SpellingCorrectorOptions() {#SpellingCorrectorOptions--}
```
public SpellingCorrectorOptions()
```


### getEnabled() {#getEnabled--}
```
public abstract boolean getEnabled()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν ο διορθωτής ορθογραφίας είναι ενεργοποιημένος. Η προεπιλεγμένη τιμή είναι false.


**Returns:**
boolean - Μια τιμή που υποδεικνύει εάν ο διορθωτής ορθογραφίας είναι ενεργοποιημένος.

### setEnabled(boolean value) {#setEnabled-boolean-}
```
public abstract void setEnabled(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει εάν ο διορθωτής ορθογραφίας είναι ενεργοποιημένος. Η προεπιλεγμένη τιμή είναι false.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | τιμή | boolean | Μια τιμή που υποδεικνύει εάν ο διορθωτής ορθογραφίας είναι ενεργοποιημένος. |
|

### getMaxMistakeCount() {#getMaxMistakeCount--}
```
public abstract int getMaxMistakeCount()
```


Λαμβάνει τον μέγιστο αριθμό λαθών. Η προεπιλεγμένη τιμή είναι 2.


**Returns:**
int - Μέγιστος αριθμός λαθών.

### setMaxMistakeCount(int value) {#setMaxMistakeCount-int-}
```
public abstract void setMaxMistakeCount(int value)
```


Ορίζει τον μέγιστο αριθμό λαθών. Η προεπιλεγμένη τιμή είναι  2 .


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | τιμή | int | Ο μέγιστος αριθμός λαθών. |
|

### getOnlyBestResults() {#getOnlyBestResults--}
```
public abstract boolean getOnlyBestResults()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν θα επιστραφούν μόνο τα καλύτερα αποτελέσματα. Η προεπιλεγμένη τιμή είναι  false .


**Returns:**
boolean -  true  εάν θα επιστραφούν μόνο τα καλύτερα αποτελέσματα· διαφορετικά  false .

### setOnlyBestResults(boolean value) {#setOnlyBestResults-boolean-}
```
public abstract void setOnlyBestResults(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει εάν θα επιστραφούν μόνο τα καλύτερα αποτελέσματα. Η προεπιλεγμένη τιμή είναι  false .


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | τιμή | boolean | true  εάν θα επιστραφούν μόνο τα καλύτερα αποτελέσματα· διαφορετικά  false . |
|

### getOnlyBestResultsRange() {#getOnlyBestResultsRange--}
```
public abstract byte getOnlyBestResultsRange()
```


Λαμβάνει τη μέγιστη υπέρβαση του ελάχιστου αριθμού λαθών που βρέθηκαν. Η προεπιλεγμένη τιμή είναι  0 .


**Returns:**
byte - Η μέγιστη υπέρβαση του ελάχιστου αριθμού λαθών που βρέθηκαν.

### setOnlyBestResultsRange(byte value) {#setOnlyBestResultsRange-byte-}
```
public abstract void setOnlyBestResultsRange(byte value)
```


Ορίζει τη μέγιστη υπέρβαση του ελάχιστου αριθμού λαθών που βρέθηκαν. Η προεπιλεγμένη τιμή είναι  0 .


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | τιμή | byte | Η μέγιστη υπέρβαση του ελάχιστου αριθμού λαθών που βρέθηκαν. |
|

### getConsiderTranspositions() {#getConsiderTranspositions--}
```
public abstract boolean getConsiderTranspositions()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν ο αλγόριθμος πρέπει να θεωρεί τη μετατόπιση δύο διαδοχικών χαρακτήρων ως ένα μόνο λάθος. Η προεπιλεγμένη τιμή είναι  true .


**Returns:**
boolean -  true  εάν ο αλγόριθμος διορθωτή ορθογραφίας θεωρεί τις μετατοπίσεις· διαφορετικά  false .

### setConsiderTranspositions(boolean value) {#setConsiderTranspositions-boolean-}
```
public abstract void setConsiderTranspositions(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει εάν ο αλγόριθμος πρέπει να θεωρεί τη μετατόπιση δύο διαδοχικών χαρακτήρων ως ένα μόνο λάθος. Η προεπιλεγμένη τιμή είναι  true .


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | τιμή | boolean | true  εάν ο αλγόριθμος διορθωτή ορθογραφίας θεωρεί τις μετατοπίσεις· διαφορετικά  false . |
|

