---
title: "OcrIndexingOptions"
second_title: "GroupDocs.Search για Java API Reference"
description: "Παρέχει επιλογές για την επεξεργασία OCR και την ευρετηρίαση του αναγνωρισμένου κειμένου."
type: docs
weight: 31
url: /el/java/com.groupdocs.search.options/ocrindexingoptions/
---
**Inheritance:**
java.lang.Object
```
public abstract class OcrIndexingOptions
```

Παρέχει επιλογές για την επεξεργασία OCR και την ευρετηρίαση του αναγνωρισμένου κειμένου.

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [OcrIndexingOptions()](#OcrIndexingOptions--) |  |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getEnabledForSeparateImages()](#getEnabledForSeparateImages--) | Λαμβάνει μια τιμή που υποδεικνύει εάν θα αναγνωριστεί κείμενο σε ξεχωριστά αρχεία εικόνας. |
|
|  | [setEnabledForSeparateImages(boolean value)](#setEnabledForSeparateImages-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν θα αναγνωριστεί κείμενο σε ξεχωριστά αρχεία εικόνας. |
|
|  | [getEnabledForContainerItemImages()](#getEnabledForContainerItemImages--) | Λαμβάνει μια τιμή που υποδεικνύει εάν θα αναγνωριστεί κείμενο σε εικόνες που είναι στοιχεία σε ένα κοντέινερ (για παράδειγμα, εικόνες σε αρχείο ZIP). |
|
|  | [setEnabledForContainerItemImages(boolean value)](#setEnabledForContainerItemImages-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν θα αναγνωριστεί κείμενο σε εικόνες που είναι στοιχεία σε ένα κοντέινερ (για παράδειγμα, εικόνες σε αρχείο ZIP). |
|
|  | [getEnabledForEmbeddedImages()](#getEnabledForEmbeddedImages--) | Λαμβάνει μια τιμή που υποδεικνύει εάν θα αναγνωριστεί κείμενο σε ενσωματωμένες εικόνες (για παράδειγμα, εικόνες σε έγγραφο DOCX). |
|
|  | [setEnabledForEmbeddedImages(boolean value)](#setEnabledForEmbeddedImages-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν θα αναγνωριστεί κείμενο σε ενσωματωμένες εικόνες (για παράδειγμα, εικόνες σε έγγραφο DOCX). |
|
|  | [getOcrConnector()](#getOcrConnector--) | Λαμβάνει έναν σύνδεσμο OCR που χρησιμοποιείται για επεξεργασία OCR. |
|
|  | [setOcrConnector(IOcrConnector value)](#setOcrConnector-com.groupdocs.search.options.IOcrConnector-) | Ορίζει έναν σύνδεσμο OCR που χρησιμοποιείται για επεξεργασία OCR. |
|
### OcrIndexingOptions() {#OcrIndexingOptions--}
```
public OcrIndexingOptions()
```


### getEnabledForSeparateImages() {#getEnabledForSeparateImages--}
```
public abstract boolean getEnabledForSeparateImages()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν θα αναγνωριστεί κείμενο σε ξεχωριστά αρχεία εικόνας. Η προεπιλεγμένη τιμή είναι false.


**Returns:**
boolean - Μια τιμή που υποδεικνύει εάν θα αναγνωριστεί κείμενο σε ξεχωριστά αρχεία εικόνας.

### setEnabledForSeparateImages(boolean value) {#setEnabledForSeparateImages-boolean-}
```
public abstract void setEnabledForSeparateImages(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει εάν θα αναγνωριστεί κείμενο σε ξεχωριστά αρχεία εικόνας. Η προεπιλεγμένη τιμή είναι false.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | τιμή | boolean | Μια τιμή που υποδεικνύει εάν θα αναγνωριστεί κείμενο σε ξεχωριστά αρχεία εικόνας. |
|

### getEnabledForContainerItemImages() {#getEnabledForContainerItemImages--}
```
public abstract boolean getEnabledForContainerItemImages()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν θα αναγνωριστεί κείμενο σε εικόνες που είναι στοιχεία σε ένα κοντέινερ (για παράδειγμα, εικόνες σε αρχείο ZIP). Η προεπιλεγμένη τιμή είναι false.


**Returns:**
boolean - Μια τιμή που υποδεικνύει εάν θα αναγνωριστεί κείμενο σε εικόνες που είναι στοιχεία σε ένα κοντέινερ.

### setEnabledForContainerItemImages(boolean value) {#setEnabledForContainerItemImages-boolean-}
```
public abstract void setEnabledForContainerItemImages(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει εάν θα αναγνωριστεί κείμενο σε εικόνες που είναι στοιχεία σε ένα κοντέινερ (για παράδειγμα, εικόνες σε αρχείο ZIP). Η προεπιλεγμένη τιμή είναι false.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | τιμή | boolean | Μια τιμή που υποδεικνύει εάν θα αναγνωριστεί κείμενο σε εικόνες που είναι στοιχεία σε ένα κοντέινερ. |
|

### getEnabledForEmbeddedImages() {#getEnabledForEmbeddedImages--}
```
public abstract boolean getEnabledForEmbeddedImages()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν θα αναγνωριστεί κείμενο σε ενσωματωμένες εικόνες (για παράδειγμα, εικόνες σε έγγραφο DOCX). Η προεπιλεγμένη τιμή είναι false.


**Returns:**
boolean - Μια τιμή που υποδεικνύει εάν θα αναγνωριστεί κείμενο σε ενσωματωμένες εικόνες.

### setEnabledForEmbeddedImages(boolean value) {#setEnabledForEmbeddedImages-boolean-}
```
public abstract void setEnabledForEmbeddedImages(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει εάν θα αναγνωριστεί κείμενο σε ενσωματωμένες εικόνες (για παράδειγμα, εικόνες σε έγγραφο DOCX). Η προεπιλεγμένη τιμή είναι false.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | τιμή | boolean | Μια τιμή που υποδεικνύει εάν θα αναγνωριστεί κείμενο σε ενσωματωμένες εικόνες. |
|

### getOcrConnector() {#getOcrConnector--}
```
public abstract IOcrConnector getOcrConnector()
```


Λαμβάνει έναν σύνδεσμο OCR που χρησιμοποιείται για επεξεργασία OCR. Η προεπιλεγμένη τιμή είναι null, που σημαίνει ότι δεν χρησιμοποιείται OCR.


**Returns:**
[IOcrConnector](../../com.groupdocs.search.options/iocrconnector) - An OCR connector that is used for OCR processing.

### setOcrConnector(IOcrConnector value) {#setOcrConnector-com.groupdocs.search.options.IOcrConnector-}
```
public abstract void setOcrConnector(IOcrConnector value)
```


Ορίζει έναν σύνδεσμο OCR που χρησιμοποιείται για επεξεργασία OCR. Η προεπιλεγμένη τιμή είναι null, που σημαίνει ότι δεν χρησιμοποιείται OCR.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | value | [IOcrConnector](../../com.groupdocs.search.options/iocrconnector) | Ένας σύνδεσμος OCR που χρησιμοποιείται για επεξεργασία OCR. |
|

