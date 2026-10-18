---
title: "ImageIndexingOptions"
second_title: "GroupDocs.Search για Java API Reference"
description: "Παρέχει επιλογές ευρετηρίασης εικόνων για αντίστροφη αναζήτηση εικόνας."
type: docs
weight: 23
url: /el/java/com.groupdocs.search.options/imageindexingoptions/
---
**Inheritance:**
java.lang.Object
```
public abstract class ImageIndexingOptions
```

Παρέχει επιλογές ευρετηρίασης εικόνων για αντίστροφη αναζήτηση εικόνας.

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [ImageIndexingOptions()](#ImageIndexingOptions--) |  |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getEnabledForSeparateImages()](#getEnabledForSeparateImages--) | Αποκτά μια τιμή που υποδεικνύει εάν θα γίνει ευρετηρίαση ξεχωριστών αρχείων εικόνας. |
|
|  | [setEnabledForSeparateImages(boolean value)](#setEnabledForSeparateImages-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν θα γίνει ευρετηρίαση ξεχωριστών αρχείων εικόνας. |
|
|  | [getEnabledForContainerItemImages()](#getEnabledForContainerItemImages--) | Αποκτά μια τιμή που υποδεικνύει εάν θα γίνει ευρετηρίαση εικόνων που είναι στοιχεία σε ένα κοντέινερ (π.χ., εικόνες σε αρχείο ZIP). |
|
|  | [setEnabledForContainerItemImages(boolean value)](#setEnabledForContainerItemImages-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν θα γίνει ευρετηρίαση εικόνων που είναι στοιχεία σε ένα κοντέινερ (π.χ., εικόνες σε αρχείο ZIP). |
|
|  | [getEnabledForEmbeddedImages()](#getEnabledForEmbeddedImages--) | Αποκτά μια τιμή που υποδεικνύει εάν θα γίνει ευρετηρίαση ενσωματωμένων εικόνων (π.χ., εικόνες σε έγγραφο DOCX). |
|
|  | [setEnabledForEmbeddedImages(boolean value)](#setEnabledForEmbeddedImages-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν θα γίνει ευρετηρίαση ενσωματωμένων εικόνων (π.χ., εικόνες σε έγγραφο DOCX). |
|
### ImageIndexingOptions() {#ImageIndexingOptions--}
```
public ImageIndexingOptions()
```


### getEnabledForSeparateImages() {#getEnabledForSeparateImages--}
```
public abstract boolean getEnabledForSeparateImages()
```


Αποκτά μια τιμή που υποδεικνύει εάν θα γίνει ευρετηρίαση ξεχωριστών αρχείων εικόνας. Η προεπιλεγμένη τιμή είναι  false .


**Returns:**
boolean - Μια τιμή που υποδεικνύει εάν θα γίνει ευρετηρίαση ξεχωριστών αρχείων εικόνας.

### setEnabledForSeparateImages(boolean value) {#setEnabledForSeparateImages-boolean-}
```
public abstract void setEnabledForSeparateImages(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει εάν θα γίνει ευρετηρίαση ξεχωριστών αρχείων εικόνας. Η προεπιλεγμένη τιμή είναι  false .


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | τιμή | boolean | Μια τιμή που υποδεικνύει εάν θα γίνει ευρετηρίαση ξεχωριστών αρχείων εικόνας. |
|

### getEnabledForContainerItemImages() {#getEnabledForContainerItemImages--}
```
public abstract boolean getEnabledForContainerItemImages()
```


Αποκτά μια τιμή που υποδεικνύει εάν θα γίνει ευρετηρίαση εικόνων που είναι στοιχεία σε ένα κοντέινερ (π.χ., εικόνες σε αρχείο ZIP). Η προεπιλεγμένη τιμή είναι  false .


**Returns:**
boolean - Τιμή που υποδεικνύει εάν θα γίνει ευρετηρίαση των εικόνων που είναι στοιχεία σε ένα κοντέινερ.

### setEnabledForContainerItemImages(boolean value) {#setEnabledForContainerItemImages-boolean-}
```
public abstract void setEnabledForContainerItemImages(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει εάν θα γίνει ευρετηρίαση των εικόνων που είναι στοιχεία σε ένα κοντέινερ (για παράδειγμα, εικόνες σε αρχείο ZIP). Η προεπιλεγμένη τιμή είναι false.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | τιμή | boolean | Τιμή που υποδεικνύει εάν θα γίνει ευρετηρίαση των εικόνων που είναι στοιχεία σε ένα κοντέινερ. |
|

### getEnabledForEmbeddedImages() {#getEnabledForEmbeddedImages--}
```
public abstract boolean getEnabledForEmbeddedImages()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν θα γίνει ευρετηρίαση ενσωματωμένων εικόνων (για παράδειγμα, εικόνες σε έγγραφο DOCX). Η προεπιλεγμένη τιμή είναι false.


**Returns:**
boolean - Τιμή που υποδεικνύει εάν θα γίνει ευρετηρίαση ενσωματωμένων εικόνων.

### setEnabledForEmbeddedImages(boolean value) {#setEnabledForEmbeddedImages-boolean-}
```
public abstract void setEnabledForEmbeddedImages(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει εάν θα γίνει ευρετηρίαση ενσωματωμένων εικόνων (για παράδειγμα, εικόνες σε έγγραφο DOCX). Η προεπιλεγμένη τιμή είναι false.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | τιμή | boolean | Τιμή που υποδεικνύει εάν θα γίνει ευρετηρίαση ενσωματωμένων εικόνων. |
|

