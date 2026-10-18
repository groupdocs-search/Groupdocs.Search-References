---
title: "UpdateOptions"
second_title: "GroupDocs.Search για Java API Reference"
description: "Παρέχει επιλογές για τη λειτουργία ενημέρωσης."
type: docs
weight: 43
url: /el/java/com.groupdocs.search.options/updateoptions/
---
**Inheritance:**
java.lang.Object
```
public class UpdateOptions
```

Παρέχει επιλογές για τη λειτουργία ενημέρωσης.


**Learn more**

* [Update index](../https://docs.groupdocs.com/display/searchjava/Update+index)
* [Delete indexed paths](../https://docs.groupdocs.com/display/searchjava/Delete+indexed+paths)

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [UpdateOptions()](#UpdateOptions--) | Αρχικοποιεί μια νέα παρουσία της  UpdateOptions  κλάσης. |
|
|  | [UpdateOptions(Object data)](#UpdateOptions-java.lang.Object-) | Αρχικοποιεί μια νέα παρουσία της  UpdateOptions  κλάσης. |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getThreads()](#getThreads--) | Λαμβάνει τον αριθμό των νημάτων που χρησιμοποιούνται για την ευρετηρίαση. |
|
|  | [setThreads(int value)](#setThreads-int-) | Ορίζει τον αριθμό των νημάτων που χρησιμοποιούνται για την ευρετηρίαση. |
|
|  | [isAsync()](#isAsync--) | Λαμβάνει τη σημαία της ασύγχρονης εκτέλεσης της λειτουργίας. |
|
|  | [setAsync(boolean value)](#setAsync-boolean-) | Ορίζει τη σημαία της ασύγχρονης εκτέλεσης της λειτουργίας. |
|
|  | [getCancellation()](#getCancellation--) | Λαμβάνει το αντικείμενο ακύρωσης της λειτουργίας. |
|
|  | [setCancellation(Cancellation value)](#setCancellation-com.groupdocs.search.common.Cancellation-) | Ορίζει το αντικείμενο ακύρωσης της λειτουργίας. |
|
|  | [getAutoDetectEncoding()](#getAutoDetectEncoding--) | Λαμβάνει μια τιμή που υποδεικνύει εάν θα ανιχνεύσει την κωδικοποίηση αυτόματα ή όχι. |
|
|  | [setAutoDetectEncoding(boolean value)](#setAutoDetectEncoding-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν θα ανιχνεύσει την κωδικοποίηση αυτόματα ή όχι. |
|
|  | [getEncoding()](#getEncoding--) | Λαμβάνει την κωδικοποίηση που χρησιμοποιείται για την εξαγωγή κειμένου από έγγραφα κειμένου. |
|
|  | [setEncoding(String value)](#setEncoding-java.lang.String-) | Ορίζει την κωδικοποίηση που χρησιμοποιείται για την εξαγωγή κειμένου από έγγραφα κειμένου. |
|
|  | [getUseRawTextExtraction()](#getUseRawTextExtraction--) | Λαμβάνει μια τιμή που υποδεικνύει εάν η ακατέργαστη λειτουργία χρησιμοποιείται για την εξαγωγή κειμένου, εφόσον είναι δυνατόν. |
|
|  | [setUseRawTextExtraction(boolean value)](#setUseRawTextExtraction-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν η ακατέργαστη λειτουργία χρησιμοποιείται για την εξαγωγή κειμένου, εφόσον είναι δυνατόν. |
|
|  | [getMetadataIndexingOptions()](#getMetadataIndexingOptions--) | Λαμβάνει τις επιλογές για την ευρετηρίαση πεδίων μεταδεδομένων. |
|
|  | [getOcrIndexingOptions()](#getOcrIndexingOptions--) | Λαμβάνει τις επιλογές για την επεξεργασία OCR και την ευρετηρίαση του αναγνωρισμένου κειμένου. |
|
|  | [getImageIndexingOptions()](#getImageIndexingOptions--) | Λαμβάνει τις επιλογές ευρετηρίασης εικόνας για την αντίστροφη αναζήτηση εικόνων. |
|
| [getCore()](#getCore--) |  |
### UpdateOptions() {#UpdateOptions--}
```
public UpdateOptions()
```


Αρχικοποιεί μια νέα παρουσία της  UpdateOptions  κλάσης.


### UpdateOptions(Object data) {#UpdateOptions-java.lang.Object-}
```
public UpdateOptions(Object data)
```


Αρχικοποιεί μια νέα παρουσία της  UpdateOptions  κλάσης.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | δεδομένα | java.lang.Object | Τα σειριοποιημένα δεδομένα. |
|

### getThreads() {#getThreads--}
```
public int getThreads()
```


Λαμβάνει τον αριθμό των νημάτων που χρησιμοποιούνται για την ευρετηρίαση. Η προεπιλεγμένη τιμή είναι  1 .


**Returns:**
int - Ο αριθμός των νημάτων που χρησιμοποιούνται για την ευρετηρίαση.

### setThreads(int value) {#setThreads-int-}
```
public void setThreads(int value)
```


Ορίζει τον αριθμό των νημάτων που χρησιμοποιούνται για την ευρετηρίαση. Η προεπιλεγμένη τιμή είναι  1 .


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | τιμή | int | Ο αριθμός των νημάτων που χρησιμοποιούνται για την ευρετηρίαση. |
|

### isAsync() {#isAsync--}
```
public boolean isAsync()
```


Λαμβάνει τη σημαία της ασύγχρονης εκτέλεσης της λειτουργίας. Η προεπιλεγμένη τιμή είναι  false .


**Returns:**
boolean - Η σημαία της ασύγχρονης εκτέλεσης της λειτουργίας.

### setAsync(boolean value) {#setAsync-boolean-}
```
public void setAsync(boolean value)
```


Ορίζει τη σημαία της ασύγχρονης εκτέλεσης της λειτουργίας. Η προεπιλεγμένη τιμή είναι  false .


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | τιμή | boolean | Η σημαία της ασύγχρονης εκτέλεσης της λειτουργίας. |
|

### getCancellation() {#getCancellation--}
```
public Cancellation getCancellation()
```


Λαμβάνει το αντικείμενο ακύρωσης της λειτουργίας. Η προεπιλεγμένη τιμή είναι  null .


**Returns:**
[Cancellation](../../com.groupdocs.search.common/cancellation) - The operation cancellation object.

### setCancellation(Cancellation value) {#setCancellation-com.groupdocs.search.common.Cancellation-}
```
public void setCancellation(Cancellation value)
```


Ορίζει το αντικείμενο ακύρωσης της λειτουργίας. Η προεπιλεγμένη τιμή είναι  null .


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | value | [Cancellation](../../com.groupdocs.search.common/cancellation) | Το αντικείμενο ακύρωσης της λειτουργίας. |
|

### getAutoDetectEncoding() {#getAutoDetectEncoding--}
```
public boolean getAutoDetectEncoding()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν η κωδικοποίηση θα ανιχνευθεί αυτόματα ή όχι. Η προεπιλεγμένη τιμή είναι  false .


**Returns:**
boolean - Μια τιμή που υποδεικνύει εάν η κωδικοποίηση θα ανιχνευθεί αυτόματα ή όχι.

### setAutoDetectEncoding(boolean value) {#setAutoDetectEncoding-boolean-}
```
public void setAutoDetectEncoding(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει εάν η κωδικοποίηση θα ανιχνευθεί αυτόματα ή όχι. Η προεπιλεγμένη τιμή είναι  false .


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | τιμή | boolean | Μια τιμή που υποδεικνύει εάν η κωδικοποίηση θα ανιχνευθεί αυτόματα ή όχι. |
|

### getEncoding() {#getEncoding--}
```
public String getEncoding()
```


Λαμβάνει την κωδικοποίηση που χρησιμοποιείται για την εξαγωγή κειμένου από έγγραφα κειμένου. Η προεπιλεγμένη τιμή είναι  null , που σημαίνει ότι χρησιμοποιείται η προεπιλεγμένη κωδικοποίηση UTF-8. Εάν το AutoDetectEncoding είναι  true  τότε αυτή η τιμή χρησιμοποιείται ως προεπιλεγμένη κωδικοποίηση.


**Returns:**
java.lang.String - Η κωδικοποίηση που χρησιμοποιείται για την εξαγωγή κειμένου από έγγραφα κειμένου.

### setEncoding(String value) {#setEncoding-java.lang.String-}
```
public void setEncoding(String value)
```


Ορίζει την κωδικοποίηση που χρησιμοποιείται για την εξαγωγή κειμένου από έγγραφα κειμένου. Η προεπιλεγμένη τιμή είναι  null , που σημαίνει ότι χρησιμοποιείται η προεπιλεγμένη κωδικοποίηση UTF-8. Εάν το AutoDetectEncoding είναι  true  τότε αυτή η τιμή χρησιμοποιείται ως προεπιλεγμένη κωδικοποίηση.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | τιμή | java.lang.String | Η κωδικοποίηση που χρησιμοποιείται για την εξαγωγή κειμένου από έγγραφα κειμένου. |
|

### getUseRawTextExtraction() {#getUseRawTextExtraction--}
```
public boolean getUseRawTextExtraction()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν χρησιμοποιείται η ακατέργαστη λειτουργία για εξαγωγή κειμένου, εάν είναι δυνατόν. Η προεπιλεγμένη τιμή είναι  true . Η ακατέργαστη λειτουργία μπορεί να αυξήσει σημαντικά την ταχύτητα ευρετηρίασης, αλλά η κανονική λειτουργία βελτιώνει τη μορφοποίηση του εξαγόμενου κειμένου.


**Returns:**
boolean - Μια τιμή που υποδεικνύει εάν χρησιμοποιείται η ακατέργαστη λειτουργία για εξαγωγή κειμένου, εάν είναι δυνατόν.

### setUseRawTextExtraction(boolean value) {#setUseRawTextExtraction-boolean-}
```
public void setUseRawTextExtraction(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει εάν χρησιμοποιείται η ακατέργαστη λειτουργία για εξαγωγή κειμένου, εάν είναι δυνατόν. Η προεπιλεγμένη τιμή είναι  true . Η ακατέργαστη λειτουργία μπορεί να αυξήσει σημαντικά την ταχύτητα ευρετηρίασης, αλλά η κανονική λειτουργία βελτιώνει τη μορφοποίηση του εξαγόμενου κειμένου.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | τιμή | boolean | Μια τιμή που υποδεικνύει εάν χρησιμοποιείται η ακατέργαστη λειτουργία για εξαγωγή κειμένου, εάν είναι δυνατόν. |
|

### getMetadataIndexingOptions() {#getMetadataIndexingOptions--}
```
public MetadataIndexingOptions getMetadataIndexingOptions()
```


Λαμβάνει τις επιλογές για την ευρετηρίαση πεδίων μεταδεδομένων.


**Returns:**
[MetadataIndexingOptions](../../com.groupdocs.search.options/metadataindexingoptions) - The options for indexing metadata fields.

### getOcrIndexingOptions() {#getOcrIndexingOptions--}
```
public OcrIndexingOptions getOcrIndexingOptions()
```


Λαμβάνει τις επιλογές για την επεξεργασία OCR και την ευρετηρίαση του αναγνωρισμένου κειμένου.


**Returns:**
[OcrIndexingOptions](../../com.groupdocs.search.options/ocrindexingoptions) - The options for OCR processing and indexing recognized text.

### getImageIndexingOptions() {#getImageIndexingOptions--}
```
public ImageIndexingOptions getImageIndexingOptions()
```


Λαμβάνει τις επιλογές ευρετηρίασης εικόνας για την αντίστροφη αναζήτηση εικόνων.


**Returns:**
[ImageIndexingOptions](../../com.groupdocs.search.options/imageindexingoptions) - The image indexing options for reverse image search.

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
