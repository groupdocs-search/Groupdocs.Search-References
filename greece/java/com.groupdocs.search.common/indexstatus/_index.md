---
title: "IndexStatus"
second_title: "GroupDocs.Search για Java API Reference"
description: "Καθορίζει την κατάσταση του ευρετηρίου."
type: docs
weight: 41
url: /el/java/com.groupdocs.search.common/indexstatus/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum IndexStatus extends Enum<IndexStatus>
```

Καθορίζει την κατάσταση του ευρετηρίου.

## Πεδία

| Πεδίο | Περιγραφή |
| --- | --- |
|  | [Ready](#Ready) | Το ευρετήριο είναι ελεύθερο και έτοιμο για αλλαγή. |
|
|  | [Failed](#Failed) | Το ευρετήριο χρειάζεται επαναφόρτωση λόγω σφάλματος. |
|
|  | [Indexing](#Indexing) | Το ευρετήριο εκτελεί λειτουργία ευρετηρίασης. |
|
|  | [Updating](#Updating) | Το ευρετήριο εκτελεί λειτουργία ενημέρωσης. |
|
|  | [Merging](#Merging) | Το ευρετήριο εκτελεί λειτουργία συγχώνευσης. |
|
|  | [Optimizing](#Optimizing) | Το ευρετήριο εκτελεί λειτουργία βελτιστοποίησης. |
|
|  | [Deleting](#Deleting) | Το Index εκτελεί μια διαγραφή. |
|
|  | [Renaming](#Renaming) | Το Index εκτελεί μια μετονομασία. |
|
|  | [ChangingAttributes](#ChangingAttributes) | Το Index αλλάζει ιδιότητες. |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Ready {#Ready}
```
public static final IndexStatus Ready
```


Το ευρετήριο είναι ελεύθερο και έτοιμο για αλλαγή.


### Failed {#Failed}
```
public static final IndexStatus Failed
```


Το ευρετήριο χρειάζεται επαναφόρτωση λόγω σφάλματος.


### Indexing {#Indexing}
```
public static final IndexStatus Indexing
```


Το ευρετήριο εκτελεί λειτουργία ευρετηρίασης.


### Updating {#Updating}
```
public static final IndexStatus Updating
```


Το ευρετήριο εκτελεί λειτουργία ενημέρωσης.


### Merging {#Merging}
```
public static final IndexStatus Merging
```


Το ευρετήριο εκτελεί λειτουργία συγχώνευσης.


### Optimizing {#Optimizing}
```
public static final IndexStatus Optimizing
```


Το ευρετήριο εκτελεί λειτουργία βελτιστοποίησης.


### Deleting {#Deleting}
```
public static final IndexStatus Deleting
```


Το Index εκτελεί μια διαγραφή.


### Renaming {#Renaming}
```
public static final IndexStatus Renaming
```


Το Index εκτελεί μια μετονομασία.


### ChangingAttributes {#ChangingAttributes}
```
public static final IndexStatus ChangingAttributes
```


Το Index αλλάζει ιδιότητες.


### values() {#values--}
```
public static IndexStatus[] values()
```




**Returns:**
com.groupdocs.search.common.IndexStatus[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static IndexStatus valueOf(String name)
```




**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| όνομα | java.lang.String |  |

**Returns:**
[IndexStatus](../../com.groupdocs.search.common/indexstatus)
