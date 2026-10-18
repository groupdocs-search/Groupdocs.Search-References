---
title: "Έγγραφο"
second_title: "GroupDocs.Search για Java API Reference"
description: "Αναπαριστά την βασική κλάση για έγγραφα που προστίθενται σε ένα ευρετήριο από ροή ή δομή του συστήματος αρχείων."
type: docs
weight: 13
url: /el/java/com.groupdocs.search/document/
---
**Inheritance:**
java.lang.Object
```
public abstract class Document
```

Αναπαριστά την βασική κλάση για έγγραφα που προστίθενται σε ένα ευρετήριο από το σύστημα αρχείων, ροή ή δομή. Περιέχει στατικές μεθόδους για τη δημιουργία εγγράφων από διαφορετικούς τύπους πηγών.


**Learn more**

* [Indexing from different sources](../https://docs.groupdocs.com/search/java/indexing-from-different-sources/)

## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getDocumentSourceKind()](#getDocumentSourceKind--) | Λαμβάνει τον τύπο προέλευσης του εγγράφου. |
|
|  | [getDocumentKey()](#getDocumentKey--) | Λαμβάνει το κλειδί του εγγράφου που χρησιμοποιείται για την ταυτοποίηση του εγγράφου μέσα σε ένα ευρετήριο. |
|
|  | [isLazy()](#isLazy--) | Λαμβάνει μια τιμή που υποδεικνύει αν το έγγραφο φορτώνεται κατά την ανάγκη ή όχι. |
|
|  | [getModificationDate()](#getModificationDate--) | Λαμβάνει την ημερομηνία τελευταίας τροποποίησης του εγγράφου. |
|
|  | [getExtension()](#getExtension--) | Λαμβάνει την επέκταση που χρησιμοποιείται για αυτόν τον τύπο εγγράφου. |
|
|  | [getAdditionalFields()](#getAdditionalFields--) | Λαμβάνει τα πρόσθετα πεδία για το έγγραφο. |
|
|  | [setAdditionalFields(DocumentField[] value)](#setAdditionalFields-com.groupdocs.search.common.DocumentField---) | Ορίζει τα πρόσθετα πεδία για το έγγραφο. |
|
|  | [getAttributes()](#getAttributes--) | Λαμβάνει τα χαρακτηριστικά του εγγράφου. |
|
|  | [setAttributes(String[] value)](#setAttributes-java.lang.String---) | Ορίζει τα χαρακτηριστικά του εγγράφου. |
|
|  | [createFromFile(String filePath)](#createFromFile-java.lang.String-) | Δημιουργεί ένα έγγραφο από αρχείο. |
|
|  | [createFromStream(String documentKey, Date modificationDate, String extension, InputStream stream)](#createFromStream-java.lang.String-java.util.Date-java.lang.String-java.io.InputStream-) | Δημιουργεί ένα έγγραφο από ροή. |
|
|  | [createFromStructure(String documentKey, Date modificationDate, DocumentField[] fields)](#createFromStructure-java.lang.String-java.util.Date-com.groupdocs.search.common.DocumentField---) | Δημιουργεί ένα έγγραφο από δομή που είναι ένας πίνακας πεδίων κειμένου. |
|
|  | [createLazy(DocumentSourceKind documentSourceKind, String documentKey, IDocumentLoader documentLoader)](#createLazy-com.groupdocs.search.common.DocumentSourceKind-java.lang.String-com.groupdocs.search.common.IDocumentLoader-) | Δημιουργεί ένα έγγραφο με καθυστερημένη φόρτωση. |
|
|  | [toString()](#toString--) | Επιστρέφει ένα  java.lang.String  που αντιπροσωπεύει το τρέχον  Document . |
|
### getDocumentSourceKind() {#getDocumentSourceKind--}
```
public abstract DocumentSourceKind getDocumentSourceKind()
```


Λαμβάνει τον τύπο προέλευσης του εγγράφου.


**Returns:**
[DocumentSourceKind](../../com.groupdocs.search.common/documentsourcekind) - The document source kind.

### getDocumentKey() {#getDocumentKey--}
```
public abstract String getDocumentKey()
```


Λαμβάνει το κλειδί του εγγράφου που χρησιμοποιείται για την ταυτοποίηση του εγγράφου μέσα σε ένα ευρετήριο.


**Returns:**
java.lang.String - Το κλειδί του εγγράφου που χρησιμοποιείται για την ταυτοποίηση του εγγράφου μέσα σε ένα ευρετήριο.

### isLazy() {#isLazy--}
```
public abstract boolean isLazy()
```


Λαμβάνει μια τιμή που υποδεικνύει αν το έγγραφο φορτώνεται κατά την ανάγκη ή όχι.


**Returns:**
boolean - Μια τιμή που υποδεικνύει αν το έγγραφο φορτώνεται κατά την ανάγκη ή όχι.

### getModificationDate() {#getModificationDate--}
```
public abstract Date getModificationDate()
```


Λαμβάνει την ημερομηνία τελευταίας τροποποίησης του εγγράφου.


**Returns:**
java.util.Date - Η ημερομηνία τελευταίας τροποποίησης του εγγράφου.

### getExtension() {#getExtension--}
```
public abstract String getExtension()
```


Λαμβάνει την επέκταση που χρησιμοποιείται για αυτόν τον τύπο εγγράφου.


**Returns:**
java.lang.String - Η επέκταση που χρησιμοποιείται για αυτόν τον τύπο εγγράφου.

### getAdditionalFields() {#getAdditionalFields--}
```
public DocumentField[] getAdditionalFields()
```


Λαμβάνει τα πρόσθετα πεδία για το έγγραφο.


**Returns:**
com.groupdocs.search.common.DocumentField[] - Τα πρόσθετα πεδία για το έγγραφο.

### setAdditionalFields(DocumentField[] value) {#setAdditionalFields-com.groupdocs.search.common.DocumentField---}
```
public void setAdditionalFields(DocumentField[] value)
```


Ορίζει τα πρόσθετα πεδία για το έγγραφο.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | value | [DocumentField\[\]](../../com.groupdocs.search.common/documentfield) | Τα πρόσθετα πεδία για το έγγραφο. |
|

### getAttributes() {#getAttributes--}
```
public String[] getAttributes()
```


Λαμβάνει τα χαρακτηριστικά του εγγράφου.


**Returns:**
java.lang.String[] - Τα χαρακτηριστικά του εγγράφου.

### setAttributes(String[] value) {#setAttributes-java.lang.String---}
```
public void setAttributes(String[] value)
```


Ορίζει τα χαρακτηριστικά του εγγράφου.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | τιμή | java.lang.String[] | Τα χαρακτηριστικά του εγγράφου. |
|

### createFromFile(String filePath) {#createFromFile-java.lang.String-}
```
public static Document createFromFile(String filePath)
```


Δημιουργεί ένα έγγραφο από αρχείο.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | filePath | java.lang.String | Η διαδρομή αρχείου του εγγράφου. |
|

**Returns:**
[Document](../../com.groupdocs.search/document) - The created document.

### createFromStream(String documentKey, Date modificationDate, String extension, InputStream stream) {#createFromStream-java.lang.String-java.util.Date-java.lang.String-java.io.InputStream-}
```
public static Document createFromStream(String documentKey, Date modificationDate, String extension, InputStream stream)
```


Δημιουργεί ένα έγγραφο από ροή.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | documentKey | java.lang.String | Το κλειδί του εγγράφου. |
|
|  | modificationDate | java.util.Date | Η ημερομηνία τροποποίησης του εγγράφου. |
|
|  | επέκταση | java.lang.String | Η επέκταση του εγγράφου. |
|
|  | ροή | java.io.InputStream | Η ροή του εγγράφου. |
|

**Returns:**
[Document](../../com.groupdocs.search/document) - The created document.

### createFromStructure(String documentKey, Date modificationDate, DocumentField[] fields) {#createFromStructure-java.lang.String-java.util.Date-com.groupdocs.search.common.DocumentField---}
```
public static Document createFromStructure(String documentKey, Date modificationDate, DocumentField[] fields)
```


Δημιουργεί ένα έγγραφο από δομή που είναι ένας πίνακας πεδίων κειμένου.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | documentKey | java.lang.String | Το κλειδί του εγγράφου. |
|
|  | modificationDate | java.util.Date | Η ημερομηνία τροποποίησης του εγγράφου. |
|
|  | fields | [DocumentField\[\]](../../com.groupdocs.search.common/documentfield) | Τα πεδία του εγγράφου. |
|

**Returns:**
[Document](../../com.groupdocs.search/document) - The created document.

### createLazy(DocumentSourceKind documentSourceKind, String documentKey, IDocumentLoader documentLoader) {#createLazy-com.groupdocs.search.common.DocumentSourceKind-java.lang.String-com.groupdocs.search.common.IDocumentLoader-}
```
public static Document createLazy(DocumentSourceKind documentSourceKind, String documentKey, IDocumentLoader documentLoader)
```


Δημιουργεί ένα έγγραφο με καθυστερημένη φόρτωση.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | documentSourceKind | [DocumentSourceKind](../../com.groupdocs.search.common/documentsourcekind) | Ο τύπος πηγής του εγγράφου. Αυτή η τιμή πρέπει να ταιριάζει με τον τύπο του φορτωμένου εγγράφου. |
|
|  | documentKey | java.lang.String | Το κλειδί του εγγράφου. Αυτή η τιμή πρέπει να ταιριάζει με το κλειδί του φορτωμένου εγγράφου. |
|
|  | documentLoader | [IDocumentLoader](../../com.groupdocs.search.common/idocumentloader) | Ο φορτωτής εγγράφου. |
|

**Returns:**
[Document](../../com.groupdocs.search/document) - The created document.

### toString() {#toString--}
```
public String toString()
```


Επιστρέφει ένα  java.lang.String  που αντιπροσωπεύει το τρέχον  Document .


**Returns:**
java.lang.String - Ένα  java.lang.String  που αντιπροσωπεύει το τρέχον  Document .

