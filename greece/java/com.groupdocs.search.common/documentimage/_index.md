---
title: "DocumentImage"
second_title: "GroupDocs.Search για Java API Reference"
description: "Αναπαριστά δεδομένα εικόνας εγγράφου."
type: docs
weight: 16
url: /el/java/com.groupdocs.search.common/documentimage/
---
**Inheritance:**
java.lang.Object
```
public abstract class DocumentImage
```

Αναπαριστά δεδομένα εικόνας εγγράφου.

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [DocumentImage()](#DocumentImage--) |  |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getImageIndex()](#getImageIndex--) | Λαμβάνει τον διαδοχικό αριθμό της εικόνας στο έγγραφο. |
|
|  | [getFields()](#getFields--) | Λαμβάνει τα εξαγόμενα πεδία. |
|
|  | [getFrames()](#getFrames--) | Λαμβάνει τα πλαίσια της εικόνας. |
|
### DocumentImage() {#DocumentImage--}
```
public DocumentImage()
```


### getImageIndex() {#getImageIndex--}
```
public abstract int getImageIndex()
```


Λαμβάνει τον διαδοχικό αριθμό της εικόνας στο έγγραφο.


**Returns:**
int - Ο διαδοχικός αριθμός της εικόνας στο έγγραφο.

### getFields() {#getFields--}
```
public abstract DocumentField[] getFields()
```


Λαμβάνει τα εξαγόμενα πεδία.


**Returns:**
com.groupdocs.search.common.DocumentField[] - Τα εξαγόμενα πεδία.

### getFrames() {#getFrames--}
```
public abstract ImageFrame[] getFrames()
```


Λαμβάνει τα πλαίσια της εικόνας.


**Returns:**
com.groupdocs.search.common.ImageFrame[] - Τα πλαίσια της εικόνας.

