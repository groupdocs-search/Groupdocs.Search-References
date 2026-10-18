---
title: "DeleteResult"
second_title: "GroupDocs.Search για Java API Reference"
description: "Αντιπροσωπεύει το αποτέλεσμα της λειτουργίας διαγραφής ευρετηριασμένων αρχείων ή φακέλων από ένα ευρετήριο."
type: docs
weight: 10
url: /el/java/com.groupdocs.search.results/deleteresult/
---
**Inheritance:**
java.lang.Object
```
public class DeleteResult
```

Αντιπροσωπεύει το αποτέλεσμα της λειτουργίας διαγραφής ευρετηριασμένων αρχείων ή φακέλων από ένα ευρετήριο.


**Learn more**

* [Delete indexed paths](../https://docs.groupdocs.com/display/searchjava/Delete+indexed+paths)

## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getItemResults()](#getItemResults--) | Επιστρέφει τα αποτελέσματα της διαγραφής κάθε διαδρομής. |
|
|  | [getTotalCount()](#getTotalCount--) | Επιστρέφει το συνολικό αριθμό διαδρομών προς διαγραφή. |
|
|  | [getSuccessCount()](#getSuccessCount--) | Επιστρέφει τον αριθμό των διαδρομών που διαγράφηκαν επιτυχώς. |
|
|  | [getFailedCount()](#getFailedCount--) | Επιστρέφει τον αριθμό των διαδρομών που δεν διαγράφηκαν λόγω σφαλμάτων. |
|
|  | [getErrors()](#getErrors--) | Επιστρέφει περιγραφές των σφαλμάτων διαγραφής. |
|
### getItemResults() {#getItemResults--}
```
public final PathDeleteResult[] getItemResults()
```


Επιστρέφει τα αποτελέσματα της διαγραφής κάθε διαδρομής.


**Returns:**
com.groupdocs.search.results.PathDeleteResult[] - Τα αποτελέσματα της διαγραφής κάθε διαδρομής.

### getTotalCount() {#getTotalCount--}
```
public final int getTotalCount()
```


Επιστρέφει το συνολικό αριθμό διαδρομών προς διαγραφή.


**Returns:**
int - Ο συνολικός αριθμός διαδρομών προς διαγραφή.

### getSuccessCount() {#getSuccessCount--}
```
public final int getSuccessCount()
```


Επιστρέφει τον αριθμό των διαδρομών που διαγράφηκαν επιτυχώς.


**Returns:**
int - Ο αριθμός των διαδρομών που διαγράφηκαν επιτυχώς.

### getFailedCount() {#getFailedCount--}
```
public final int getFailedCount()
```


Επιστρέφει τον αριθμό των διαδρομών που δεν διαγράφηκαν λόγω σφαλμάτων.


**Returns:**
int - Ο αριθμός των διαδρομών που δεν διαγράφηκαν λόγω σφαλμάτων.

### getErrors() {#getErrors--}
```
public final String[] getErrors()
```


Επιστρέφει περιγραφές των σφαλμάτων διαγραφής.


**Returns:**
java.lang.String[] - Περιγραφές σφαλμάτων διαγραφής.

