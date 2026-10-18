---
title: "NetworkSearchResult"
second_title: "GroupDocs.Search για Java API Reference"
description: "Αντιπροσωπεύει ένα αποτέλεσμα αναζήτησης που ταιριάζει με ένα ερώτημα αναζήτησης."
type: docs
weight: 14
url: /el/java/com.groupdocs.search.scaling.results/networksearchresult/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public abstract class NetworkSearchResult implements Iterable<NetworkFoundDocument>
```

Αντιπροσωπεύει ένα αποτέλεσμα αναζήτησης που ταιριάζει με ένα ερώτημα αναζήτησης.

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [NetworkSearchResult()](#NetworkSearchResult--) |  |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getDocumentCount()](#getDocumentCount--) | Λαμβάνει τον αριθμό των εγγράφων που βρέθηκαν. |
|
|  | [getOccurrenceCount()](#getOccurrenceCount--) | Λαμβάνει τον συνολικό αριθμό των εμφανίσεων που βρέθηκαν. |
|
|  | [getTruncated()](#getTruncated--) | Λαμβάνει μια τιμή που υποδεικνύει ότι το αποτέλεσμα είναι περικομμένο. |
|
|  | [getWarnings()](#getWarnings--) | Λαμβάνει μια προειδοποίηση που περιγράφει το αποτέλεσμα. |
|
|  | [getStartTime()](#getStartTime--) | Λαμβάνει την ώρα έναρξης της αναζήτησης. |
|
|  | [getEndTime()](#getEndTime--) | Λαμβάνει την ώρα λήξης της αναζήτησης. |
|
|  | [getSearchDuration()](#getSearchDuration--) | Λαμβάνει τη διάρκεια της αναζήτησης σε δευτερόλεπτα. |
|
|  | [getFoundDocument(int index)](#getFoundDocument-int-) | Λαμβάνει το έγγραφο που βρέθηκε με βάση το δείκτη. |
|
|  | [iterator()](#iterator--) | Επιστρέφει έναν επαναλήπτη που διατρέχει τη συλλογή των εγγράφων που βρέθηκαν. |
|
|  | [getNextChunkSearchToken()](#getNextChunkSearchToken--) | Λαμβάνει ένα διακριτικό αναζήτησης τμήματος για την αναζήτηση του επόμενου τμήματος. |
|
|  | [getNodeIndex()](#getNodeIndex--) | Λαμβάνει το δείκτη του κόμβου από τον οποίο ελήφθη το αποτέλεσμα. |
|
### NetworkSearchResult() {#NetworkSearchResult--}
```
public NetworkSearchResult()
```


### getDocumentCount() {#getDocumentCount--}
```
public abstract int getDocumentCount()
```


Λαμβάνει τον αριθμό των εγγράφων που βρέθηκαν.


**Returns:**
int - Ο αριθμός των εγγράφων που βρέθηκαν.

### getOccurrenceCount() {#getOccurrenceCount--}
```
public abstract int getOccurrenceCount()
```


Λαμβάνει τον συνολικό αριθμό των εμφανίσεων που βρέθηκαν.


**Returns:**
int - Ο συνολικός αριθμός των εμφανίσεων που βρέθηκαν.

### getTruncated() {#getTruncated--}
```
public abstract boolean getTruncated()
```


Λαμβάνει μια τιμή που υποδεικνύει ότι το αποτέλεσμα είναι περικομμένο.


**Returns:**
boolean - Μια τιμή που υποδεικνύει ότι το αποτέλεσμα είναι περικομμένο.

### getWarnings() {#getWarnings--}
```
public abstract String getWarnings()
```


Λαμβάνει μια προειδοποίηση που περιγράφει το αποτέλεσμα.


**Returns:**
java.lang.String - Μια προειδοποίηση που περιγράφει το αποτέλεσμα.

### getStartTime() {#getStartTime--}
```
public abstract Date getStartTime()
```


Λαμβάνει την ώρα έναρξης της αναζήτησης.


**Returns:**
java.util.Date - Η ώρα έναρξης της αναζήτησης.

### getEndTime() {#getEndTime--}
```
public abstract Date getEndTime()
```


Λαμβάνει την ώρα λήξης της αναζήτησης.


**Returns:**
java.util.Date - Η ώρα λήξης της αναζήτησης.

### getSearchDuration() {#getSearchDuration--}
```
public abstract double getSearchDuration()
```


Λαμβάνει τη διάρκεια της αναζήτησης σε δευτερόλεπτα.


**Returns:**
double - Η διάρκεια της αναζήτησης σε δευτερόλεπτα.

### getFoundDocument(int index) {#getFoundDocument-int-}
```
public abstract NetworkFoundDocument getFoundDocument(int index)
```


Λαμβάνει το έγγραφο που βρέθηκε με βάση το δείκτη.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | ευρετήριο | int | Ο δείκτης ενός εγγράφου που βρέθηκε. |
|

**Returns:**
[NetworkFoundDocument](../../com.groupdocs.search.scaling.results/networkfounddocument) - The found document.

### iterator() {#iterator--}
```
public abstract Iterator<NetworkFoundDocument> iterator()
```


Επιστρέφει έναν επαναλήπτη που διατρέχει τη συλλογή των εγγράφων που βρέθηκαν.


**Returns:**
java.util.Iterator<com.groupdocs.search.scaling.results.NetworkFoundDocument> - Ένας επαναλήπτης που μπορεί να χρησιμοποιηθεί για την επανάληψη στη συλλογή των εγγράφων που βρέθηκαν.

### getNextChunkSearchToken() {#getNextChunkSearchToken--}
```
public abstract NetworkSearchToken getNextChunkSearchToken()
```


Λαμβάνει ένα διακριτικό αναζήτησης τμήματος για την αναζήτηση του επόμενου τμήματος.


**Returns:**
[NetworkSearchToken](../../com.groupdocs.search.scaling.results/networksearchtoken) - A chunk search token for searching the next chunk.

### getNodeIndex() {#getNodeIndex--}
```
public abstract int getNodeIndex()
```


Λαμβάνει το δείκτη του κόμβου από τον οποίο ελήφθη το αποτέλεσμα.


**Returns:**
int - Ο δείκτης του κόμβου από τον οποίο ελήφθη το αποτέλεσμα.

