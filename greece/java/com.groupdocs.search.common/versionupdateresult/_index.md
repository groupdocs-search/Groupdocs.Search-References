---
title: "VersionUpdateResult"
second_title: "GroupDocs.Search για Java API Reference"
description: "Αντιπροσωπεύει το αποτέλεσμα μιας λειτουργίας ενημέρωσης έκδοσης ευρετηρίου."
type: docs
weight: 42
url: /el/java/com.groupdocs.search.common/versionupdateresult/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum VersionUpdateResult extends Enum<VersionUpdateResult>
```

Αντιπροσωπεύει το αποτέλεσμα μιας λειτουργίας ενημέρωσης έκδοσης ευρετηρίου.

## Πεδία

| Πεδίο | Περιγραφή |
| --- | --- |
|  | [Updated](#Updated) | Η έκδοση του ευρετηρίου ενημερώθηκε. |
|
|  | [AlreadyUpToDate](#AlreadyUpToDate) | Η έκδοση του ευρετηρίου είναι ήδη ενημερωμένη. |
|
|  | [Unsupported](#Unsupported) | Η έκδοση του ευρετηρίου δεν υποστηρίζεται ή ο φάκελος δεν περιέχει έγκυρα δεδομένα ευρετηρίου. |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Updated {#Updated}
```
public static final VersionUpdateResult Updated
```


Η έκδοση του ευρετηρίου ενημερώθηκε.


### AlreadyUpToDate {#AlreadyUpToDate}
```
public static final VersionUpdateResult AlreadyUpToDate
```


Η έκδοση του ευρετηρίου είναι ήδη ενημερωμένη.


### Unsupported {#Unsupported}
```
public static final VersionUpdateResult Unsupported
```


Η έκδοση του ευρετηρίου δεν υποστηρίζεται ή ο φάκελος δεν περιέχει έγκυρα δεδομένα ευρετηρίου.


### values() {#values--}
```
public static VersionUpdateResult[] values()
```




**Returns:**
com.groupdocs.search.common.VersionUpdateResult[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static VersionUpdateResult valueOf(String name)
```




**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| όνομα | java.lang.String |  |

**Returns:**
[VersionUpdateResult](../../com.groupdocs.search.common/versionupdateresult)
