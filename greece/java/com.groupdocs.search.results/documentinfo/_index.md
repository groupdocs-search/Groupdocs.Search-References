---
title: "DocumentInfo"
second_title: "GroupDocs.Search για Java API Reference"
description: "Αντιπροσωπεύει έναν περιγραφέα για ένα ευρετηριασμένο έγγραφο."
type: docs
weight: 11
url: /el/java/com.groupdocs.search.results/documentinfo/
---
**Inheritance:**
java.lang.Object
```
public abstract class DocumentInfo
```

Αντιπροσωπεύει έναν περιγραφέα για ένα ευρετηριασμένο έγγραφο.


**Learn more**

* [Search results](../https://docs.groupdocs.com/display/searchjava/Search+results)
* [Getting indexed documents](../https://docs.groupdocs.com/display/searchjava/Getting+indexed+documents)

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [DocumentInfo()](#DocumentInfo--) |  |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [toString()](#toString--) | Επιστρέφει ένα  System.String  που αντιπροσωπεύει το τρέχον  DocumentInfo . |
|
|  | [getFilePath()](#getFilePath--) | Λαμβάνει τη διαδρομή αρχείου για ευρετηρίαση από αρχείο ή το κλειδί εγγράφου για ευρετηρίαση από ροή ή δομή. |
|
|  | [getFileType()](#getFileType--) | Λαμβάνει τον τύπο αρχείου. |
|
|  | [getFormatFamily()](#getFormatFamily--) | Λαμβάνει την οικογένεια μορφής του εγγράφου. |
|
|  | [getInnerPath()](#getInnerPath--) | Λαμβάνει τη εσωτερική διαδρομή για το στοιχείο εγγράφου του container. |
|
|  | [getInnerPathParts()](#getInnerPathParts--) | Λαμβάνει τα μέρη της εσωτερικής διαδρομής για το στοιχείο εγγράφου του container. |
|
|  | [getDocumentSourceKind()](#getDocumentSourceKind--) | Λαμβάνει τον τύπο προέλευσης του εγγράφου. |
|
|  | [getIndexedWithError()](#getIndexedWithError--) | Λαμβάνει τον δείκτη σφάλματος ευρετηρίασης. |
|
|  | [serialize()](#serialize--) | Σειριοποιεί την τρέχουσα παρουσία σε έναν πίνακα byte. |
|
|  | [deserialize(byte[] array)](#deserialize-byte---) | Αποσειριοποιεί μια παρουσία από έναν πίνακα byte. |
|
### DocumentInfo() {#DocumentInfo--}
```
public DocumentInfo()
```


### toString() {#toString--}
```
public abstract String toString()
```


Επιστρέφει ένα  System.String  που αντιπροσωπεύει το τρέχον  DocumentInfo .


**Returns:**
java.lang.String - Ένα  System.String  που αντιπροσωπεύει το τρέχον  DocumentInfo .

### getFilePath() {#getFilePath--}
```
public abstract String getFilePath()
```


Λαμβάνει τη διαδρομή αρχείου για ευρετηρίαση από αρχείο ή το κλειδί εγγράφου για ευρετηρίαση από ροή ή δομή.


**Returns:**
java.lang.String - Η διαδρομή αρχείου ή το κλειδί εγγράφου.

### getFileType() {#getFileType--}
```
public abstract FileType getFileType()
```


Λαμβάνει τον τύπο αρχείου.


**Returns:**
[FileType](../../com.groupdocs.search.results/filetype) - The file type.

### getFormatFamily() {#getFormatFamily--}
```
public abstract FormatFamily getFormatFamily()
```


Λαμβάνει την οικογένεια μορφής του εγγράφου.


**Returns:**
[FormatFamily](../../com.groupdocs.search.results/formatfamily) - The document format family.

### getInnerPath() {#getInnerPath--}
```
public abstract String getInnerPath()
```


Λαμβάνει τη εσωτερική διαδρομή για το στοιχείο εγγράφου του container.


**Returns:**
java.lang.String - Η εσωτερική διαδρομή.

### getInnerPathParts() {#getInnerPathParts--}
```
public abstract String[] getInnerPathParts()
```


Λαμβάνει τα μέρη της εσωτερικής διαδρομής για το στοιχείο εγγράφου του container.


**Returns:**
java.lang.String[] - Τα μέρη της εσωτερικής διαδρομής.

### getDocumentSourceKind() {#getDocumentSourceKind--}
```
public abstract DocumentSourceKind getDocumentSourceKind()
```


Λαμβάνει τον τύπο προέλευσης του εγγράφου.


**Returns:**
[DocumentSourceKind](../../com.groupdocs.search.common/documentsourcekind) - The document source kind.

### getIndexedWithError() {#getIndexedWithError--}
```
public abstract boolean getIndexedWithError()
```


Λαμβάνει τον δείκτη σφάλματος ευρετηρίασης.


**Returns:**
boolean - Ο δείκτης σφάλματος ευρετηρίασης.

### serialize() {#serialize--}
```
public abstract byte[] serialize()
```


Σειριοποιεί την τρέχουσα παρουσία σε έναν πίνακα byte.


**Returns:**
byte[] - Ένας πίνακας byte που αντιπροσωπεύει την τρέχουσα παρουσία.

### deserialize(byte[] array) {#deserialize-byte---}
```
public static DocumentInfo deserialize(byte[] array)
```


Αποσειριοποιεί μια παρουσία από έναν πίνακα byte.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | πίνακας | byte[] | Ένας πίνακας byte για αποσειριοποίηση. |
|

**Returns:**
[DocumentInfo](../../com.groupdocs.search.results/documentinfo) - An instance deserialized from a byte array.

