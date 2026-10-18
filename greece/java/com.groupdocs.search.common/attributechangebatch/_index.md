---
title: "AttributeChangeBatch"
second_title: "GroupDocs.Search για Java API Reference"
description: "Αναπαριστά ένα δοχείο για αλλαγές χαρακτηριστικών."
type: docs
weight: 10
url: /el/java/com.groupdocs.search.common/attributechangebatch/
---
**Inheritance:**
java.lang.Object
```
public class AttributeChangeBatch
```

Αναπαριστά ένα δοχείο για αλλαγές χαρακτηριστικών.


**Learn more**

* [Document attributes](../https://docs.groupdocs.com/display/searchjava/Document+attributes)
* [Document filtering in search result](../https://docs.groupdocs.com/display/searchjava/Document+filtering+in+search+result)

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [AttributeChangeBatch()](#AttributeChangeBatch--) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης AttributeChangeBatch. |
|
|  | [AttributeChangeBatch(Object data)](#AttributeChangeBatch-java.lang.Object-) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης AttributeChangeBatch. |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [add(String path, String[] attributes)](#add-java.lang.String-java.lang.String...-) | Προσθέτει τα καθορισμένα χαρακτηριστικά στο καθορισμένο ευρετηριασμένο έγγραφο. |
|
|  | [add(String[] paths, String[] attributes)](#add-java.lang.String---java.lang.String...-) | Προσθέτει τα καθορισμένα χαρακτηριστικά στα καθορισμένα ευρετηριασμένα έγγραφα. |
|
|  | [addToAll(String[] attributes)](#addToAll-java.lang.String...-) | Προσθέτει τα καθορισμένα χαρακτηριστικά σε όλα τα έγγραφα στο ευρετήριο. |
|
|  | [remove(String path, String[] attributes)](#remove-java.lang.String-java.lang.String...-) | Αφαιρεί τα καθορισμένα χαρακτηριστικά από το καθορισμένο ευρετηριασμένο έγγραφο. |
|
|  | [remove(String[] paths, String[] attributes)](#remove-java.lang.String---java.lang.String...-) | Αφαιρεί τα καθορισμένα χαρακτηριστικά από τα καθορισμένα ευρετηριασμένα έγγραφα. |
|
|  | [removeAll(String path)](#removeAll-java.lang.String-) | Αφαιρεί όλα τα χαρακτηριστικά από το καθορισμένο ευρετηριασμένο έγγραφο. |
|
|  | [removeAll(String[] paths)](#removeAll-java.lang.String---) | Αφαιρεί όλα τα χαρακτηριστικά από τα καθορισμένα ευρετηριασμένα έγγραφα. |
|
|  | [removeFromAll(String[] attributes)](#removeFromAll-java.lang.String...-) | Αφαιρεί τα καθορισμένα χαρακτηριστικά από όλα τα έγγραφα στο ευρετήριο. |
|
|  | [clear()](#clear--) | Αφαιρεί όλα τα χαρακτηριστικά από όλα τα έγγραφα στο ευρετήριο. |
|
| [getCore()](#getCore--) |  |
### AttributeChangeBatch() {#AttributeChangeBatch--}
```
public AttributeChangeBatch()
```


Αρχικοποιεί ένα νέο αντικείμενο της κλάσης AttributeChangeBatch.


### AttributeChangeBatch(Object data) {#AttributeChangeBatch-java.lang.Object-}
```
public AttributeChangeBatch(Object data)
```


Αρχικοποιεί ένα νέο αντικείμενο της κλάσης AttributeChangeBatch.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | δεδομένα | java.lang.Object | Τα σειριοποιημένα δεδομένα. |
|

### add(String path, String[] attributes) {#add-java.lang.String-java.lang.String...-}
```
public void add(String path, String[] attributes)
```


Προσθέτει τα καθορισμένα χαρακτηριστικά στο καθορισμένο ευρετηριασμένο έγγραφο.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | path | java.lang.String | Η διαδρομή του εγγράφου. |
|
|  | ιδιότητες | java.lang.String[] | Τα χαρακτηριστικά προς προσθήκη. |
|

### add(String[] paths, String[] attributes) {#add-java.lang.String---java.lang.String...-}
```
public void add(String[] paths, String[] attributes)
```


Προσθέτει τα καθορισμένα χαρακτηριστικά στα καθορισμένα ευρετηριασμένα έγγραφα.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | paths | java.lang.String[] | Οι διαδρομές των εγγράφων. |
|
|  | ιδιότητες | java.lang.String[] | Τα χαρακτηριστικά προς προσθήκη. |
|

### addToAll(String[] attributes) {#addToAll-java.lang.String...-}
```
public void addToAll(String[] attributes)
```


Προσθέτει τα καθορισμένα χαρακτηριστικά σε όλα τα έγγραφα στο ευρετήριο.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | ιδιότητες | java.lang.String[] | Τα χαρακτηριστικά προς προσθήκη. |
|

### remove(String path, String[] attributes) {#remove-java.lang.String-java.lang.String...-}
```
public void remove(String path, String[] attributes)
```


Αφαιρεί τα καθορισμένα χαρακτηριστικά από το καθορισμένο ευρετηριασμένο έγγραφο.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | path | java.lang.String | Η διαδρομή του εγγράφου. |
|
|  | ιδιότητες | java.lang.String[] | Τα χαρακτηριστικά προς αφαίρεση. |
|

### remove(String[] paths, String[] attributes) {#remove-java.lang.String---java.lang.String...-}
```
public void remove(String[] paths, String[] attributes)
```


Αφαιρεί τα καθορισμένα χαρακτηριστικά από τα καθορισμένα ευρετηριασμένα έγγραφα.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | paths | java.lang.String[] | Οι διαδρομές των εγγράφων. |
|
|  | ιδιότητες | java.lang.String[] | Τα χαρακτηριστικά προς αφαίρεση. |
|

### removeAll(String path) {#removeAll-java.lang.String-}
```
public void removeAll(String path)
```


Αφαιρεί όλα τα χαρακτηριστικά από το καθορισμένο ευρετηριασμένο έγγραφο.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | path | java.lang.String | Η διαδρομή του εγγράφου. |
|

### removeAll(String[] paths) {#removeAll-java.lang.String---}
```
public void removeAll(String[] paths)
```


Αφαιρεί όλα τα χαρακτηριστικά από τα καθορισμένα ευρετηριασμένα έγγραφα.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | paths | java.lang.String[] | Οι διαδρομές των εγγράφων. |
|

### removeFromAll(String[] attributes) {#removeFromAll-java.lang.String...-}
```
public void removeFromAll(String[] attributes)
```


Αφαιρεί τα καθορισμένα χαρακτηριστικά από όλα τα έγγραφα στο ευρετήριο.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | ιδιότητες | java.lang.String[] | Τα χαρακτηριστικά προς αφαίρεση. |
|

### clear() {#clear--}
```
public void clear()
```


Αφαιρεί όλα τα χαρακτηριστικά από όλα τα έγγραφα στο ευρετήριο.


### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
