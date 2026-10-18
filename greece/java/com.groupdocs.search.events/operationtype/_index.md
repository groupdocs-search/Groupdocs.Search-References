---
title: "OperationType"
second_title: "GroupDocs.Search για Java API Reference"
description: "Αναπαριστά έναν τύπο λειτουργίας ευρετηρίου."
type: docs
weight: 23
url: /el/java/com.groupdocs.search.events/operationtype/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum OperationType extends Enum<OperationType>
```

Αναπαριστά έναν τύπο λειτουργίας ευρετηρίου.

## Πεδία

| Πεδίο | Περιγραφή |
| --- | --- |
|  | [Indexing](#Indexing) | Προσθήκη εγγράφων σε ένα ευρετήριο. |
|
|  | [Updating](#Updating) | Ενημέρωση εγγράφων σε ένα ευρετήριο. |
|
|  | [Merging](#Merging) | Συγχώνευση ευρετηρίων. |
|
|  | [Optimizing](#Optimizing) | Βελτιστοποίηση ενός ευρετηρίου. |
|
|  | [Deleting](#Deleting) | Διαγραφή διαδρομών από ένα ευρετήριο. |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Indexing {#Indexing}
```
public static final OperationType Indexing
```


Προσθήκη εγγράφων σε ένα ευρετήριο.


### Updating {#Updating}
```
public static final OperationType Updating
```


Ενημέρωση εγγράφων σε ένα ευρετήριο.


### Merging {#Merging}
```
public static final OperationType Merging
```


Συγχώνευση ευρετηρίων.


### Optimizing {#Optimizing}
```
public static final OperationType Optimizing
```


Βελτιστοποίηση ενός ευρετηρίου.


### Deleting {#Deleting}
```
public static final OperationType Deleting
```


Διαγραφή διαδρομών από ένα ευρετήριο.


### values() {#values--}
```
public static OperationType[] values()
```




**Returns:**
com.groupdocs.search.events.OperationType[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static OperationType valueOf(String name)
```




**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| όνομα | java.lang.String |  |

**Returns:**
[OperationType](../../com.groupdocs.search.events/operationtype)
