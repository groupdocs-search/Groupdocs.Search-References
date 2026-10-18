---
title: "CustomExtractorCollection"
second_title: "GroupDocs.Search για Java API Reference"
description: "Περιέχει μια συλλογή προσαρμοσμένων εξαγωγέων."
type: docs
weight: 13
url: /el/java/com.groupdocs.search.common/customextractorcollection/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public abstract class CustomExtractorCollection implements Iterable
```

Περιέχει μια συλλογή προσαρμοσμένων εξαγωγέων. Εάν η συλλογή περιέχει έναν εξαγωγέα για κάποια επέκταση αρχείου που καλύπτεται από ενσωματωμένους εξαγωγείς, τότε αυτός ο εξαγωγέας θα χρησιμοποιηθεί αντί για τον ενσωματωμένο.


**Learn more**

* [Custom text extractors](../https://docs.groupdocs.com/display/searchjava/Custom+text+extractors)

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [CustomExtractorCollection()](#CustomExtractorCollection--) |  |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [size()](#size--) | Λαμβάνει τον αριθμό των εξαγωγέων που περιέχονται στη συλλογή. |
|
|  | [isReadOnly()](#isReadOnly--) | Λαμβάνει μια τιμή που υποδεικνύει εάν η συλλογή είναι μόνο για ανάγνωση. |
|
|  | [iterator()](#iterator--) | Επιστρέφει έναν επαναλήπτη για αυτή τη συλλογή. |
|
|  | [addItem(IFieldExtractor extractor)](#addItem-com.groupdocs.search.common.IFieldExtractor-) | Προσθέτει έναν εξαγωγέα στη συλλογή. |
|
|  | [clear()](#clear--) | Αφαιρεί όλους τους εξαγωγείς από τη συλλογή. |
|
|  | [containsItem(IFieldExtractor item)](#containsItem-com.groupdocs.search.common.IFieldExtractor-) | Καθορίζει εάν η συλλογή περιέχει έναν συγκεκριμένο εξαγωγέα. |
|
|  | [copyToTArray(IFieldExtractor[] array, int arrayIndex)](#copyToTArray-com.groupdocs.search.common.IFieldExtractor---int-) | Αντιγράφει τα στοιχεία της συλλογής σε έναν πίνακα, ξεκινώντας από ένα συγκεκριμένο δείκτη πίνακα. |
|
|  | [removeItem(IFieldExtractor extractor)](#removeItem-com.groupdocs.search.common.IFieldExtractor-) | Αφαιρεί έναν εξαγωγέα από τη συλλογή. |
|
### CustomExtractorCollection() {#CustomExtractorCollection--}
```
public CustomExtractorCollection()
```


### size() {#size--}
```
public abstract int size()
```


Λαμβάνει τον αριθμό των εξαγωγέων που περιέχονται στη συλλογή.


**Returns:**
int - Ο αριθμός των εξαγωγέων που περιέχονται στη συλλογή.

### isReadOnly() {#isReadOnly--}
```
public abstract boolean isReadOnly()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν η συλλογή είναι μόνο για ανάγνωση.


**Returns:**
boolean - Μια τιμή που υποδεικνύει εάν η συλλογή είναι μόνο για ανάγνωση.

### iterator() {#iterator--}
```
public abstract Iterator<IFieldExtractor> iterator()
```


Επιστρέφει έναν επαναλήπτη για αυτή τη συλλογή.


**Returns:**
java.util.Iterator<com.groupdocs.search.common.IFieldExtractor> - Ένα αντικείμενο επαναλήπτη που μπορεί να χρησιμοποιηθεί για επανάληψη στη συλλογή.

### addItem(IFieldExtractor extractor) {#addItem-com.groupdocs.search.common.IFieldExtractor-}
```
public abstract void addItem(IFieldExtractor extractor)
```


Προσθέτει έναν εξαγωγέα στη συλλογή.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | extractor | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | Ο εξαγωγέας που θα προστεθεί στη συλλογή. |
|

### clear() {#clear--}
```
public abstract void clear()
```


Αφαιρεί όλους τους εξαγωγείς από τη συλλογή.


### containsItem(IFieldExtractor item) {#containsItem-com.groupdocs.search.common.IFieldExtractor-}
```
public abstract boolean containsItem(IFieldExtractor item)
```


Καθορίζει εάν η συλλογή περιέχει έναν συγκεκριμένο εξαγωγέα.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | item | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | Ο εξαγωγέας που θα εντοπιστεί στη συλλογή. |
|

**Returns:**
boolean -  true  εάν  το στοιχείο  βρεθεί στη συλλογή· διαφορετικά,  false .

### copyToTArray(IFieldExtractor[] array, int arrayIndex) {#copyToTArray-com.groupdocs.search.common.IFieldExtractor---int-}
```
public abstract void copyToTArray(IFieldExtractor[] array, int arrayIndex)
```


Αντιγράφει τα στοιχεία της συλλογής σε έναν πίνακα, ξεκινώντας από ένα συγκεκριμένο δείκτη πίνακα.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | array | [IFieldExtractor\[\]](../../com.groupdocs.search.common/ifieldextractor) | Ο μονοδιάστατος πίνακας που είναι ο προορισμός των στοιχείων που αντιγράφηκαν από τη συλλογή. Ο πίνακας πρέπει να έχει μηδενική βάση ευρετηρίασης. |
|
|  | arrayIndex | int | Ο μηδενικός δείκτης στον πίνακα από όπου αρχίζει η αντιγραφή. |
|

### removeItem(IFieldExtractor extractor) {#removeItem-com.groupdocs.search.common.IFieldExtractor-}
```
public abstract boolean removeItem(IFieldExtractor extractor)
```


Αφαιρεί έναν εξαγωγέα από τη συλλογή.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | extractor | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | Ο εξαγωγέας που θα αφαιρεθεί από τη συλλογή. |
|

**Returns:**
boolean -  true  εάν  ο εξαγωγέας  αφαιρεθεί επιτυχώς από τη συλλογή· διαφορετικά,  false . Αυτή η μέθοδος επιστρέφει επίσης  false  εάν  ο εξαγωγέας  δεν βρεθεί στην αρχική συλλογή.

