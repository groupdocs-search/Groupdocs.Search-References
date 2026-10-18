---
title: "DateFormatCollection"
second_title: "GroupDocs.Search για Java API Reference"
description: "Αναπαριστά μια συλλογή αντικειμένων DateFormat."
type: docs
weight: 14
url: /el/java/com.groupdocs.search.options/dateformatcollection/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public abstract class DateFormatCollection implements Iterable<DateFormat>
```

Αναπαριστά μια συλλογή αντικειμένων DateFormat.


**Learn more**

* [Date range search](../https://docs.groupdocs.com/display/searchjava/Date+range+search)

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [DateFormatCollection()](#DateFormatCollection--) |  |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [addItem(DateFormat item)](#addItem-com.groupdocs.search.options.DateFormat-) | Προσθέτει ένα αντικείμενο μορφής ημερομηνίας στη συλλογή. |
|
|  | [clear()](#clear--) | Αφαιρεί όλα τα στοιχεία από τη συλλογή. |
|
|  | [containsItem(DateFormat item)](#containsItem-com.groupdocs.search.options.DateFormat-) | Καθορίζει εάν η συλλογή περιέχει ένα συγκεκριμένο στοιχείο. |
|
|  | [copyToTArray(DateFormat[] array, int arrayIndex)](#copyToTArray-com.groupdocs.search.options.DateFormat---int-) | Αντιγράφει τα στοιχεία της συλλογής σε έναν  Array , ξεκινώντας από ένα συγκεκριμένο δείκτη  Array . |
|
|  | [size()](#size--) | Λαμβάνει τον αριθμό των στοιχείων που περιέχονται στη συλλογή. |
|
|  | [isReadOnly()](#isReadOnly--) | Λαμβάνει μια τιμή που υποδεικνύει εάν η συλλογή είναι μόνο για ανάγνωση. |
|
|  | [removeItem(DateFormat item)](#removeItem-com.groupdocs.search.options.DateFormat-) | Αφαιρεί την πρώτη εμφάνιση ενός συγκεκριμένου στοιχείου από τη συλλογή. |
|
|  | [iterator()](#iterator--) | Επιστρέφει έναν απαριθμητή που διατρέχει τη συλλογή. |
|
### DateFormatCollection() {#DateFormatCollection--}
```
public DateFormatCollection()
```


### addItem(DateFormat item) {#addItem-com.groupdocs.search.options.DateFormat-}
```
public abstract void addItem(DateFormat item)
```


Προσθέτει ένα αντικείμενο μορφής ημερομηνίας στη συλλογή.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | item | [DateFormat](../../com.groupdocs.search.options/dateformat) | Το αντικείμενο μορφής ημερομηνίας που θα προστεθεί στη συλλογή. |
|

### clear() {#clear--}
```
public abstract void clear()
```


Αφαιρεί όλα τα στοιχεία από τη συλλογή.


### containsItem(DateFormat item) {#containsItem-com.groupdocs.search.options.DateFormat-}
```
public abstract boolean containsItem(DateFormat item)
```


Καθορίζει εάν η συλλογή περιέχει ένα συγκεκριμένο στοιχείο.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | item | [DateFormat](../../com.groupdocs.search.options/dateformat) | Το στοιχείο που θα εντοπιστεί στη συλλογή. |
|

**Returns:**
boolean -  true  εάν το στοιχείο βρεθεί στη συλλογή· διαφορετικά,  false .

### copyToTArray(DateFormat[] array, int arrayIndex) {#copyToTArray-com.groupdocs.search.options.DateFormat---int-}
```
public abstract void copyToTArray(DateFormat[] array, int arrayIndex)
```


Αντιγράφει τα στοιχεία της συλλογής σε έναν  Array , ξεκινώντας από ένα συγκεκριμένο δείκτη  Array .


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | array | [DateFormat\[\]](../../com.groupdocs.search.options/dateformat) | Ο μονοδιάστατος  Array  που είναι ο προορισμός των στοιχείων που αντιγράφονται από τη συλλογή. |
|
|  | arrayIndex | int | Ο μηδενικός δείκτης στον πίνακα από όπου αρχίζει η αντιγραφή. |
|

### size() {#size--}
```
public abstract int size()
```


Λαμβάνει τον αριθμό των στοιχείων που περιέχονται στη συλλογή.


**Returns:**
int - Ο αριθμός των στοιχείων που περιέχονται στη συλλογή.

### isReadOnly() {#isReadOnly--}
```
public abstract boolean isReadOnly()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν η συλλογή είναι μόνο για ανάγνωση.


**Returns:**
boolean -  true  εάν η συλλογή είναι μόνο για ανάγνωση· διαφορετικά,  false .

### removeItem(DateFormat item) {#removeItem-com.groupdocs.search.options.DateFormat-}
```
public abstract boolean removeItem(DateFormat item)
```


Αφαιρεί την πρώτη εμφάνιση ενός συγκεκριμένου στοιχείου από τη συλλογή.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | item | [DateFormat](../../com.groupdocs.search.options/dateformat) | Το στοιχείο που θα αφαιρεθεί από τη συλλογή. |
|

**Returns:**
boolean -  true  εάν το στοιχείο αφαιρεθεί επιτυχώς από τη συλλογή· διαφορετικά,  false . Αυτή η μέθοδος επιστρέφει επίσης  false  εάν το στοιχείο δεν βρεθεί στη συλλογή.

### iterator() {#iterator--}
```
public abstract Iterator<DateFormat> iterator()
```


Επιστρέφει έναν απαριθμητή που διατρέχει τη συλλογή.


**Returns:**
java.util.Iterator<com.groupdocs.search.options.DateFormat> - Ένας απαριθμητής που μπορεί να χρησιμοποιηθεί για τη διαπέραση της συλλογής.

