---
title: "FoundImageFrame"
second_title: "GroupDocs.Search για Java API Reference"
description: "Αντιπροσωπεύει ένα βρεθέν πλαίσιο εικόνας."
type: docs
weight: 16
url: /el/java/com.groupdocs.search.results/foundimageframe/
---
**Inheritance:**
java.lang.Object
```
public abstract class FoundImageFrame
```

Αντιπροσωπεύει ένα βρεθέν πλαίσιο εικόνας.

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [FoundImageFrame()](#FoundImageFrame--) |  |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getDocumentInfo()](#getDocumentInfo--) | Λαμβάνει τις πληροφορίες του εγγράφου. |
|
|  | [getImageIndex()](#getImageIndex--) | Λαμβάνει τον διαδοχικό αριθμό της εικόνας στο έγγραφο. |
|
|  | [getFrameIndex()](#getFrameIndex--) | Λαμβάνει το δείκτη του πλαισίου στην εικόνα. |
|
|  | [getHashDifferences()](#getHashDifferences--) | Λαμβάνει τον αριθμό των μη αντιστοιχούντων bits στο hash της εικόνας. |
|
|  | [toString()](#toString--) | Επιστρέφει ένα  System.String  που αντιπροσωπεύει το τρέχον  FoundImageFrame . |
|
### FoundImageFrame() {#FoundImageFrame--}
```
public FoundImageFrame()
```


### getDocumentInfo() {#getDocumentInfo--}
```
public abstract DocumentInfo getDocumentInfo()
```


Λαμβάνει τις πληροφορίες του εγγράφου.


**Returns:**
[DocumentInfo](../../com.groupdocs.search.results/documentinfo) - The document info.

### getImageIndex() {#getImageIndex--}
```
public abstract int getImageIndex()
```


Λαμβάνει τον διαδοχικό αριθμό της εικόνας στο έγγραφο.


**Returns:**
int - Ο διαδοχικός αριθμός της εικόνας στο έγγραφο.

### getFrameIndex() {#getFrameIndex--}
```
public abstract int getFrameIndex()
```


Λαμβάνει το δείκτη του πλαισίου στην εικόνα.


**Returns:**
int - Δείκτης του πλαισίου στην εικόνα.

### getHashDifferences() {#getHashDifferences--}
```
public abstract int getHashDifferences()
```


Λαμβάνει τον αριθμό των μη αντιστοιχούντων bits στο hash της εικόνας.


**Returns:**
int - Ο αριθμός των μη αντιστοιχούντων bits στο hash της εικόνας.

### toString() {#toString--}
```
public abstract String toString()
```


Επιστρέφει ένα  System.String  που αντιπροσωπεύει το τρέχον  FoundImageFrame .


**Returns:**
java.lang.String - Ένα  System.String  που αντιπροσωπεύει το τρέχον  FoundImageFrame .

