---
title: "PathDeleteResult"
second_title: "GroupDocs.Search για Java API Reference"
description: "Αντιπροσωπεύει το αποτέλεσμα της λειτουργίας διαγραφής ενός ευρετηριασμένου αρχείου ή φακέλου από το ευρετήριο."
type: docs
weight: 18
url: /el/java/com.groupdocs.search.results/pathdeleteresult/
---
**Inheritance:**
java.lang.Object
```
public class PathDeleteResult
```

Αντιπροσωπεύει το αποτέλεσμα της λειτουργίας διαγραφής ενός ευρετηριασμένου αρχείου ή φακέλου από το ευρετήριο.


**Learn more**

* [Delete indexed paths](../https://docs.groupdocs.com/display/searchjava/Delete+indexed+paths)

## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [isSuccess()](#isSuccess--) | Επιστρέφει το δείκτη επιτυχίας της λειτουργίας διαγραφής. |
|
|  | [getError()](#getError--) | Επιστρέφει μια περιγραφή του σφάλματος διαγραφής. |
|
|  | [getPath()](#getPath--) | Επιστρέφει τη διαδρομή του αρχείου ή του φακέλου προς διαγραφή. |
|
### isSuccess() {#isSuccess--}
```
public final boolean isSuccess()
```


Επιστρέφει το δείκτη επιτυχίας της λειτουργίας διαγραφής.


**Returns:**
boolean -  true  εάν η λειτουργία διαγραφής ήταν επιτυχής· διαφορετικά, επιστρέφει  false .

### getError() {#getError--}
```
public final String getError()
```


Επιστρέφει μια περιγραφή του σφάλματος διαγραφής.


**Returns:**
java.lang.String - Μια περιγραφή του σφάλματος διαγραφής.

### getPath() {#getPath--}
```
public final String getPath()
```


Επιστρέφει τη διαδρομή του αρχείου ή του φακέλου προς διαγραφή.


**Returns:**
java.lang.String - Η διαδρομή του αρχείου ή του φακέλου προς διαγραφή.

