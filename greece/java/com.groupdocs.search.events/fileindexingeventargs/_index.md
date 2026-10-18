---
title: "FileIndexingEventArgs"
second_title: "GroupDocs.Search για Java API Reference"
description: "Αναπαριστά τα ορίσματα για το γεγονός έναρξης ευρετηρίασης εγγράφου."
type: docs
weight: 14
url: /el/java/com.groupdocs.search.events/fileindexingeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class FileIndexingEventArgs extends BaseIndexEventArgs
```

Αναπαριστά τα ορίσματα για το γεγονός έναρξης ευρετηρίασης εγγράφου.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getDocument()](#getDocument--) | Λαμβάνει το έγγραφο. |
|
|  | [getDocumentFullPath()](#getDocumentFullPath--) | Λαμβάνει τη πλήρη διαδρομή του εγγράφου. |
|
|  | [getDocumentKey()](#getDocumentKey--) | Λαμβάνει το κλειδί του εγγράφου. |
|
|  | [getSkipIndexing()](#getSkipIndexing--) | Λαμβάνει μια τιμή που υποδεικνύει ότι η ευρετηρίαση του εγγράφου πρέπει να παραληφθεί. |
|
|  | [setSkipIndexing(boolean value)](#setSkipIndexing-boolean-) | Ορίζει μια τιμή που υποδεικνύει ότι η ευρετηρίαση του εγγράφου πρέπει να παραληφθεί. |
|
|  | [getEncoding()](#getEncoding--) | Λαμβάνει την κωδικοποίηση του εγγράφου. |
|
|  | [setEncoding(String value)](#setEncoding-java.lang.String-) | Ορίζει την κωδικοποίηση του εγγράφου. |
|
|  | [getCustomExtractor()](#getCustomExtractor--) | Αποκτά τον προσαρμοσμένο εξαγωγέα κειμένου. |
|
|  | [setCustomExtractor(IFieldExtractor value)](#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-) | Ορίζει τον προσαρμοσμένο εξαγωγέα κειμένου. |
|
|  | [getAdditionalFields()](#getAdditionalFields--) | Λαμβάνει τα πρόσθετα πεδία για το έγγραφο. |
|
|  | [setAdditionalFields(DocumentField[] value)](#setAdditionalFields-com.groupdocs.search.common.DocumentField---) | Ορίζει τα πρόσθετα πεδία για το έγγραφο. |
|
|  | [getAttributes()](#getAttributes--) | Λαμβάνει τα χαρακτηριστικά του εγγράφου. |
|
|  | [setAttributes(String[] value)](#setAttributes-java.lang.String---) | Ορίστε τα χαρακτηριστικά του εγγράφου. |
|
### getDocument() {#getDocument--}
```
public final Document getDocument()
```


Λαμβάνει το έγγραφο.


**Returns:**
[Document](../../com.groupdocs.search/document) - The document.

### getDocumentFullPath() {#getDocumentFullPath--}
```
public final String getDocumentFullPath()
```


Λαμβάνει τη πλήρη διαδρομή του εγγράφου.


**Returns:**
java.lang.String - Η πλήρης διαδρομή του εγγράφου.

### getDocumentKey() {#getDocumentKey--}
```
public final String getDocumentKey()
```


Λαμβάνει το κλειδί του εγγράφου.


**Returns:**
java.lang.String - Το κλειδί του εγγράφου.

### getSkipIndexing() {#getSkipIndexing--}
```
public final boolean getSkipIndexing()
```


Λαμβάνει μια τιμή που υποδεικνύει ότι η ευρετηρίαση του εγγράφου πρέπει να παραληφθεί.


**Returns:**
boolean - Μια τιμή που υποδεικνύει ότι η ευρετηρίαση του εγγράφου πρέπει να παραληφθεί.

### setSkipIndexing(boolean value) {#setSkipIndexing-boolean-}
```
public final void setSkipIndexing(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει ότι η ευρετηρίαση του εγγράφου πρέπει να παραληφθεί.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | τιμή | boolean | Μια τιμή που υποδεικνύει ότι η ευρετηρίαση του εγγράφου πρέπει να παραληφθεί. |
|

### getEncoding() {#getEncoding--}
```
public final String getEncoding()
```


Λαμβάνει την κωδικοποίηση του εγγράφου.


**Returns:**
java.lang.String - Η κωδικοποίηση του εγγράφου.

### setEncoding(String value) {#setEncoding-java.lang.String-}
```
public final void setEncoding(String value)
```


Ορίζει την κωδικοποίηση του εγγράφου.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | τιμή | java.lang.String | Η κωδικοποίηση του εγγράφου. |
|

### getCustomExtractor() {#getCustomExtractor--}
```
public final IFieldExtractor getCustomExtractor()
```


Αποκτά τον προσαρμοσμένο εξαγωγέα κειμένου.


**Returns:**
[IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) - The custom text extractor.

### setCustomExtractor(IFieldExtractor value) {#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-}
```
public final void setCustomExtractor(IFieldExtractor value)
```


Ορίζει τον προσαρμοσμένο εξαγωγέα κειμένου.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | value | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | Ο προσαρμοσμένος εξαγωγέας κειμένου. |
|

### getAdditionalFields() {#getAdditionalFields--}
```
public final DocumentField[] getAdditionalFields()
```


Λαμβάνει τα πρόσθετα πεδία για το έγγραφο.


**Returns:**
com.groupdocs.search.common.DocumentField[] - Τα πρόσθετα πεδία για το έγγραφο.

### setAdditionalFields(DocumentField[] value) {#setAdditionalFields-com.groupdocs.search.common.DocumentField---}
```
public final void setAdditionalFields(DocumentField[] value)
```


Ορίζει τα πρόσθετα πεδία για το έγγραφο.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | value | [DocumentField\[\]](../../com.groupdocs.search.common/documentfield) | Τα πρόσθετα πεδία για το έγγραφο. |
|

### getAttributes() {#getAttributes--}
```
public final String[] getAttributes()
```


Λαμβάνει τα χαρακτηριστικά του εγγράφου.


**Returns:**
java.lang.String[] - Τα χαρακτηριστικά του εγγράφου.

### setAttributes(String[] value) {#setAttributes-java.lang.String---}
```
public final void setAttributes(String[] value)
```


Ορίστε τα χαρακτηριστικά του εγγράφου.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | τιμή | java.lang.String[] | Τα χαρακτηριστικά του εγγράφου. |
|

