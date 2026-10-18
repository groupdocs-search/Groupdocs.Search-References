---
title: "PasswordDictionary"
second_title: "GroupDocs.Search για Java API Reference"
description: "Ορίζει τη διεπαφή ενός λεξικού κωδικών πρόσβασης εγγράφων."
type: docs
weight: 20
url: /el/java/com.groupdocs.search.dictionaries/passworddictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface PasswordDictionary extends DictionaryBase, Iterable<String>
```

Ορίζει τη διεπαφή ενός λεξικού κωδικών πρόσβασης εγγράφων.


**Learn more**

* [Indexing password protected documents](../https://docs.groupdocs.com/display/searchjava/Indexing+password+protected+documents)
* [Managing document passwords](../https://docs.groupdocs.com/display/searchjava/Document+passwords)

## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getCount()](#getCount--) | Λαμβάνει τον αριθμό των στοιχείων που περιέχονται στο λεξικό. |
|
|  | [getPassword(String filePath)](#getPassword-java.lang.String-) | Λαμβάνει τον κωδικό πρόσβασης για το αρχείο. |
|
|  | [clear()](#clear--) | Αφαιρεί όλους τους κωδικούς πρόσβασης από αυτό το αντικείμενο PasswordDictionary. |
|
|  | [contains(String filePath)](#contains-java.lang.String-) | Καθορίζει εάν το λεξικό περιέχει κωδικό πρόσβασης για το συγκεκριμένο έγγραφο. |
|
|  | [add(String filePath, String password)](#add-java.lang.String-java.lang.String-) | Προσθέτει έναν κωδικό πρόσβασης για ένα έγγραφο στο λεξικό. |
|
|  | [remove(String filePath)](#remove-java.lang.String-) | Αφαιρεί έναν κωδικό πρόσβασης του συγκεκριμένου εγγράφου από το λεξικό. |
|
|  | [iterator()](#iterator--) | Επιστρέφει έναν επαναλήπτη που διασχίζει τη συλλογή. |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


Λαμβάνει τον αριθμό των στοιχείων που περιέχονται στο λεξικό.


**Returns:**
int - Ο αριθμός των στοιχείων που περιέχονται στο λεξικό.

### getPassword(String filePath) {#getPassword-java.lang.String-}
```
public abstract String getPassword(String filePath)
```


Λαμβάνει τον κωδικό πρόσβασης για το αρχείο.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | filePath | java.lang.String | Η διαδρομή του αρχείου. |
|

**Returns:**
java.lang.String - Ο κωδικός πρόσβασης για το αρχείο.

### clear() {#clear--}
```
public abstract void clear()
```


Αφαιρεί όλους τους κωδικούς πρόσβασης από αυτό το αντικείμενο PasswordDictionary.


### contains(String filePath) {#contains-java.lang.String-}
```
public abstract boolean contains(String filePath)
```


Καθορίζει εάν το λεξικό περιέχει κωδικό πρόσβασης για το συγκεκριμένο έγγραφο.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | filePath | java.lang.String | Η διαδρομή αρχείου του εγγράφου. |
|

**Returns:**
boolean -  true  εάν το λεξικό περιέχει κωδικό πρόσβασης για το έγγραφο· διαφορετικά,  false .

### add(String filePath, String password) {#add-java.lang.String-java.lang.String-}
```
public abstract void add(String filePath, String password)
```


Προσθέτει έναν κωδικό πρόσβασης για ένα έγγραφο στο λεξικό.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | filePath | java.lang.String | Η διαδρομή αρχείου του εγγράφου. |
|
|  | κωδικός | java.lang.String | Ο κωδικός πρόσβασης του εγγράφου. |
|

### remove(String filePath) {#remove-java.lang.String-}
```
public abstract boolean remove(String filePath)
```


Αφαιρεί έναν κωδικό πρόσβασης του συγκεκριμένου εγγράφου από το λεξικό.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | filePath | java.lang.String | Η διαδρομή αρχείου του εγγράφου. |
|

**Returns:**
boolean -  true  εάν ο κωδικός πρόσβασης αφαιρέθηκε επιτυχώς· διαφορετικά,  false . Αυτή η μέθοδος επιστρέφει επίσης  false  εάν το filePath δεν βρέθηκε στο λεξικό.

### iterator() {#iterator--}
```
public abstract Iterator<String> iterator()
```


Επιστρέφει έναν επαναλήπτη που διασχίζει τη συλλογή.


**Returns:**
java.util.Iterator<java.lang.String> - Ένας επαναλήπτης που μπορεί να χρησιμοποιηθεί για επανάληψη μέσω της συλλογής.

