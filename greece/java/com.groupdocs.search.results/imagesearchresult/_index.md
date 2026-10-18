---
title: "ImageSearchResult"
second_title: "GroupDocs.Search για Java API Reference"
description: "Αντιπροσωπεύει το αποτέλεσμα μιας αντίστροφης αναζήτησης εικόνας."
type: docs
weight: 17
url: /el/java/com.groupdocs.search.results/imagesearchresult/
---
**Inheritance:**
java.lang.Object
```
public abstract class ImageSearchResult
```

Αντιπροσωπεύει το αποτέλεσμα μιας αντίστροφης αναζήτησης εικόνας.

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [ImageSearchResult()](#ImageSearchResult--) |  |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getImageCount()](#getImageCount--) | Λαμβάνει τον αριθμό των εικόνων που βρέθηκαν. |
|
|  | [getFoundImage(int index)](#getFoundImage-int-) | Λαμβάνει την εικόνα που βρέθηκε με βάση το δείκτη. |
|
### ImageSearchResult() {#ImageSearchResult--}
```
public ImageSearchResult()
```


### getImageCount() {#getImageCount--}
```
public abstract int getImageCount()
```


Λαμβάνει τον αριθμό των εικόνων που βρέθηκαν.


**Returns:**
int - Ο αριθμός των εικόνων που βρέθηκαν.

### getFoundImage(int index) {#getFoundImage-int-}
```
public abstract FoundImageFrame getFoundImage(int index)
```


Λαμβάνει την εικόνα που βρέθηκε με βάση το δείκτη.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | ευρετήριο | int | Ο δείκτης μιας εικόνας που βρέθηκε. |
|

**Returns:**
[FoundImageFrame](../../com.groupdocs.search.results/foundimageframe) - The found image.

