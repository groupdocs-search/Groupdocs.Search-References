---
title: "ExtractionOptions"
second_title: "GroupDocs.Search για Java API Reference"
description: "Παρέχει επιλογές για την εξαγωγή δεδομένων από έγγραφα."
type: docs
weight: 18
url: /el/java/com.groupdocs.search.options/extractionoptions/
---
**Inheritance:**
java.lang.Object
```
public class ExtractionOptions
```

Παρέχει επιλογές για την εξαγωγή δεδομένων από έγγραφα.

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [ExtractionOptions()](#ExtractionOptions--) | Αρχικοποιεί μια νέα παρουσία της  ExtractionOptions  κλάσης. |
|
|  | [ExtractionOptions(Object data)](#ExtractionOptions-java.lang.Object-) | Αρχικοποιεί μια νέα παρουσία της  ExtractionOptions  κλάσης. |
|
|  | [ExtractionOptions(IndexingOptions options, IFieldExtractor customExtractor, IOcrConnector ocrConnector)](#ExtractionOptions-com.groupdocs.search.options.IndexingOptions-com.groupdocs.search.common.IFieldExtractor-com.groupdocs.search.options.IOcrConnector-) | Αρχικοποιεί μια νέα παρουσία της  ExtractionOptions  κλάσης. |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getCustomExtractor()](#getCustomExtractor--) | Αποκτά τον προσαρμοσμένο εξαγωγέα κειμένου. |
|
|  | [setCustomExtractor(IFieldExtractor value)](#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-) | Ορίζει ή ορίζει τον προσαρμοσμένο εξαγωγέα κειμένου. |
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
### ExtractionOptions() {#ExtractionOptions--}
```
public ExtractionOptions()
```


Αρχικοποιεί μια νέα παρουσία της  ExtractionOptions  κλάσης.


### ExtractionOptions(Object data) {#ExtractionOptions-java.lang.Object-}
```
public ExtractionOptions(Object data)
```


Αρχικοποιεί μια νέα παρουσία της  ExtractionOptions  κλάσης.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | δεδομένα | java.lang.Object | Τα σειριοποιημένα δεδομένα. |
|

### ExtractionOptions(IndexingOptions options, IFieldExtractor customExtractor, IOcrConnector ocrConnector) {#ExtractionOptions-com.groupdocs.search.options.IndexingOptions-com.groupdocs.search.common.IFieldExtractor-com.groupdocs.search.options.IOcrConnector-}
```
public ExtractionOptions(IndexingOptions options, IFieldExtractor customExtractor, IOcrConnector ocrConnector)
```


Αρχικοποιεί μια νέα παρουσία της  ExtractionOptions  κλάσης.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | Οι επιλογές. |
|
|  | customExtractor | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | Ο προσαρμοσμένος εξαγωγέας. |
|
|  | ocrConnector | [IOcrConnector](../../com.groupdocs.search.options/iocrconnector) | Ο σύνδεσμος ocr. |
|

### getCustomExtractor() {#getCustomExtractor--}
```
public IFieldExtractor getCustomExtractor()
```


Αποκτά τον προσαρμοσμένο εξαγωγέα κειμένου. Η προεπιλεγμένη τιμή είναι  null .


**Returns:**
[IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) - The custom text extractor.

### setCustomExtractor(IFieldExtractor value) {#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-}
```
public void setCustomExtractor(IFieldExtractor value)
```


Ορίζει ή ορίζει τον προσαρμοσμένο εξαγωγέα κειμένου. Η προεπιλεγμένη τιμή είναι  null .


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | value | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | Ο προσαρμοσμένος εξαγωγέας κειμένου. |
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
