---
title: "NetworkImageSearchResult"
second_title: "GroupDocs.Search για Java API Reference"
description: "Αντιπροσωπεύει ένα αποτέλεσμα αναζήτησης εικόνας που ταιριάζει με μια εικόνα αναζήτησης."
type: docs
weight: 12
url: /el/java/com.groupdocs.search.scaling.results/networkimagesearchresult/
---
**Inheritance:**
java.lang.Object
```
public abstract class NetworkImageSearchResult
```

Αντιπροσωπεύει ένα αποτέλεσμα αναζήτησης εικόνας που ταιριάζει με μια εικόνα αναζήτησης.

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [NetworkImageSearchResult()](#NetworkImageSearchResult--) |  |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getImageCount()](#getImageCount--) | Λαμβάνει τον αριθμό των εικόνων που βρέθηκαν. |
|
|  | [getFoundImage(int index)](#getFoundImage-int-) | Λαμβάνει την εικόνα που βρέθηκε με βάση το δείκτη. |
|
|  | [getNetworkImageSearchToken()](#getNetworkImageSearchToken--) | Λαμβάνει ένα διακριτικό αναζήτησης τμηματικής εικόνας για την αναζήτηση του επόμενου τμήματος. |
|
|  | [getNodeIndex()](#getNodeIndex--) | Λαμβάνει το δείκτη του κόμβου από τον οποίο ελήφθη το αποτέλεσμα. |
|
|  | [getShardIndex()](#getShardIndex--) | Λαμβάνει το δείκτη του shard από τον οποίο ελήφθη το αποτέλεσμα. |
|
### NetworkImageSearchResult() {#NetworkImageSearchResult--}
```
public NetworkImageSearchResult()
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

### getNetworkImageSearchToken() {#getNetworkImageSearchToken--}
```
public abstract NetworkImageSearchToken getNetworkImageSearchToken()
```


Λαμβάνει ένα διακριτικό αναζήτησης τμηματικής εικόνας για την αναζήτηση του επόμενου τμήματος.


**Returns:**
[NetworkImageSearchToken](../../com.groupdocs.search.scaling.results/networkimagesearchtoken) - A chunk image search token for searching the next chunk.

### getNodeIndex() {#getNodeIndex--}
```
public abstract int getNodeIndex()
```


Λαμβάνει το δείκτη του κόμβου από τον οποίο ελήφθη το αποτέλεσμα.


**Returns:**
int - Ο δείκτης του κόμβου από τον οποίο ελήφθη το αποτέλεσμα.

### getShardIndex() {#getShardIndex--}
```
public abstract int getShardIndex()
```


Λαμβάνει το δείκτη του shard από τον οποίο ελήφθη το αποτέλεσμα.


**Returns:**
int - Ο δείκτης του shard από τον οποίο ελήφθη το αποτέλεσμα.

