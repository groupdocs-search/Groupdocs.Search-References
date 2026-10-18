---
title: "TextOptions"
second_title: "GroupDocs.Search για Java API Reference"
description: "Παρέχει επιλογές για την ανάκτηση του κειμένου εγγράφου από ένα ευρετήριο."
type: docs
weight: 41
url: /el/java/com.groupdocs.search.options/textoptions/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.search.options.ITextOptions](../../com.groupdocs.search.options/itextoptions)
```
public class TextOptions implements ITextOptions
```

Παρέχει επιλογές για την ανάκτηση του κειμένου εγγράφου από ένα ευρετήριο.


**Learn more**

* [Getting indexed documents](../https://docs.groupdocs.com/display/searchjava/Getting+indexed+documents)
* [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [TextOptions()](#TextOptions--) | Αρχικοποιεί μια νέα παρουσία της κλάσης TextOptions. |
|
|  | [TextOptions(Object data)](#TextOptions-java.lang.Object-) | Αρχικοποιεί μια νέα παρουσία της κλάσης TextOptions. |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getCustomExtractor()](#getCustomExtractor--) | Ανακτά τον προσαρμοσμένο εξαγωγέα κειμένου που χρησιμοποιήθηκε για την ευρετηρίαση. |
|
|  | [setCustomExtractor(IFieldExtractor value)](#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-) | Ορίζει τον προσαρμοσμένο εξαγωγέα κειμένου που χρησιμοποιήθηκε για την ευρετηρίαση. |
|
|  | [getAdditionalFields()](#getAdditionalFields--) | Λαμβάνει τα πρόσθετα πεδία εγγράφου που χρησιμοποιήθηκαν για την ευρετηρίαση. |
|
|  | [setAdditionalFields(DocumentField[] value)](#setAdditionalFields-com.groupdocs.search.common.DocumentField---) | Ορίζει τα πρόσθετα πεδία εγγράφου που χρησιμοποιήθηκαν για την ευρετηρίαση. |
|
|  | [getCancellation()](#getCancellation--) | Λαμβάνει το αντικείμενο ακύρωσης. |
|
|  | [setCancellation(Cancellation value)](#setCancellation-com.groupdocs.search.common.Cancellation-) | Ορίζει το αντικείμενο ακύρωσης. |
|
|  | [getGenerateHead()](#getGenerateHead--) | Λαμβάνει μια τιμή που υποδεικνύει αν η ετικέτα Head δημιουργείται στο παραγόμενο HTML. |
|
|  | [setGenerateHead(boolean value)](#setGenerateHead-boolean-) | Ορίζει μια τιμή που υποδεικνύει αν η ετικέτα Head δημιουργείται στο παραγόμενο HTML. |
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
### TextOptions() {#TextOptions--}
```
public TextOptions()
```


Αρχικοποιεί μια νέα παρουσία της κλάσης TextOptions.


### TextOptions(Object data) {#TextOptions-java.lang.Object-}
```
public TextOptions(Object data)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης TextOptions.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | δεδομένα | java.lang.Object | Τα σειριοποιημένα δεδομένα. |
|

### getCustomExtractor() {#getCustomExtractor--}
```
public IFieldExtractor getCustomExtractor()
```


Λαμβάνει τον προσαρμοσμένο εξαγωγέα κειμένου που χρησιμοποιήθηκε για την ευρετηρίαση. Η προεπιλεγμένη τιμή είναι null. Σημειώστε ότι αυτή η τιμή χρησιμοποιείται μόνο εάν το κείμενο του εγγράφου δεν αποθηκεύτηκε στο ευρετήριο.


**Returns:**
[IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) - The custom text extractor that was used for indexing.

### setCustomExtractor(IFieldExtractor value) {#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-}
```
public void setCustomExtractor(IFieldExtractor value)
```


Ορίζει τον προσαρμοσμένο εξαγωγέα κειμένου που χρησιμοποιήθηκε για την ευρετηρίαση. Η προεπιλεγμένη τιμή είναι null. Σημειώστε ότι αυτή η τιμή χρησιμοποιείται μόνο εάν το κείμενο του εγγράφου δεν αποθηκεύτηκε στο ευρετήριο.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | value | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | Ο προσαρμοσμένος εξαγωγέας κειμένου που χρησιμοποιήθηκε για την ευρετηρίαση. |
|

### getAdditionalFields() {#getAdditionalFields--}
```
public DocumentField[] getAdditionalFields()
```


Λαμβάνει τα πρόσθετα πεδία εγγράφου που χρησιμοποιήθηκαν για την ευρετηρίαση. Η προεπιλεγμένη τιμή είναι null. Σημειώστε ότι αυτή η τιμή χρησιμοποιείται μόνο εάν το κείμενο του εγγράφου δεν αποθηκεύτηκε στο ευρετήριο.


**Returns:**
com.groupdocs.search.common.DocumentField[] - Τα πρόσθετα πεδία εγγράφου που χρησιμοποιήθηκαν για την ευρετηρίαση.

### setAdditionalFields(DocumentField[] value) {#setAdditionalFields-com.groupdocs.search.common.DocumentField---}
```
public void setAdditionalFields(DocumentField[] value)
```


Ορίζει τα πρόσθετα πεδία εγγράφου που χρησιμοποιήθηκαν για την ευρετηρίαση. Η προεπιλεγμένη τιμή είναι null. Σημειώστε ότι αυτή η τιμή χρησιμοποιείται μόνο εάν το κείμενο του εγγράφου δεν αποθηκεύτηκε στο ευρετήριο.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | value | [DocumentField\[\]](../../com.groupdocs.search.common/documentfield) | Τα πρόσθετα πεδία εγγράφου που χρησιμοποιήθηκαν για την ευρετηρίαση. |
|

### getCancellation() {#getCancellation--}
```
public Cancellation getCancellation()
```


Λαμβάνει το αντικείμενο ακύρωσης. Η προεπιλεγμένη τιμή είναι null.


**Returns:**
[Cancellation](../../com.groupdocs.search.common/cancellation) - The cancellation object.

### setCancellation(Cancellation value) {#setCancellation-com.groupdocs.search.common.Cancellation-}
```
public void setCancellation(Cancellation value)
```


Ορίζει το αντικείμενο ακύρωσης. Η προεπιλεγμένη τιμή είναι null.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | value | [Cancellation](../../com.groupdocs.search.common/cancellation) | Το αντικείμενο ακύρωσης. |
|

### getGenerateHead() {#getGenerateHead--}
```
public boolean getGenerateHead()
```


Λαμβάνει μια τιμή που υποδεικνύει αν η ετικέτα Head δημιουργείται στο παραγόμενο HTML. Η προεπιλεγμένη τιμή είναι true.


**Returns:**
boolean - Μια τιμή που υποδεικνύει αν η ετικέτα Head δημιουργείται στο παραγόμενο HTML.

### setGenerateHead(boolean value) {#setGenerateHead-boolean-}
```
public void setGenerateHead(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει αν η ετικέτα Head δημιουργείται στο παραγόμενο HTML. Η προεπιλεγμένη τιμή είναι true.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | τιμή | boolean | Μια τιμή που υποδεικνύει αν η ετικέτα Head δημιουργείται στο παραγόμενο HTML. |
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
