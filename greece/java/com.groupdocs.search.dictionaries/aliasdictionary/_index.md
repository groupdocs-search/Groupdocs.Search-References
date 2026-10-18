---
title: "AliasDictionary"
second_title: "GroupDocs.Search για Java API Reference"
description: "Ορίζει τη διεπαφή ενός λεξικού ψευδωνύμων."
type: docs
weight: 14
url: /el/java/com.groupdocs.search.dictionaries/aliasdictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface AliasDictionary extends DictionaryBase, Iterable<String>
```

Ορίζει τη διεπαφή ενός λεξικού ψευδωνύμων.


**Learn more**

* [Using aliases](../https://docs.groupdocs.com/display/searchjava/Using+aliases)
* [Managing alias dictionary](../https://docs.groupdocs.com/display/searchjava/Alias+dictionary)

## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getCount()](#getCount--) | Λαμβάνει τον αριθμό των ψευδωνύμων που περιέχονται στο AliasDictionary. |
|
|  | [addRange(Iterable<AliasReplacementPair> pairs)](#addRange-java.lang.Iterable-com.groupdocs.search.dictionaries.AliasReplacementPair--) | Προσθέτει τη συγκεκριμένη συλλογή ζευγών ψευδώνυμου/αντικατάστασης σε αυτήν την περίπτωση του AliasDictionary. |
|
|  | [addRange(AliasReplacementPair[] pairs)](#addRange-com.groupdocs.search.dictionaries.AliasReplacementPair---) | Προσθέτει τη συγκεκριμένη συλλογή ζευγών ψευδώνυμου/αντικατάστασης σε αυτήν την περίπτωση του AliasDictionary. |
|
|  | [add(String alias, String text)](#add-java.lang.String-java.lang.String-) | Προσθέτει το συγκεκριμένο ζευγάρι ψευδώνυμου και σχετικού κειμένου σε αυτήν την περίπτωση του AliasDictionary. |
|
|  | [remove(String alias)](#remove-java.lang.String-) | Αφαιρεί το συγκεκριμένο ψευδώνυμο από ένα αντικείμενο AliasDictionary. |
|
|  | [contains(String alias)](#contains-java.lang.String-) | Καθορίζει εάν ένα αντικείμενο AliasDictionary περιέχει το συγκεκριμένο ψευδώνυμο. |
|
|  | [getText(String alias)](#getText-java.lang.String-) | Λαμβάνει ένα κείμενο που συνδέεται με το συγκεκριμένο ψευδώνυμο. |
|
|  | [clear()](#clear--) | Αφαιρεί όλα τα ψευδώνυμα από ένα αντικείμενο AliasDictionary. |
|
|  | [iterator()](#iterator--) | Επιστρέφει έναν επαναλήπτη που διασχίζει τη συλλογή. |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


Λαμβάνει τον αριθμό των ψευδωνύμων που περιέχονται στο AliasDictionary.


**Returns:**
int - Ο αριθμός των ψευδωνύμων που περιέχονται στο AliasDictionary.

### addRange(Iterable<AliasReplacementPair> pairs) {#addRange-java.lang.Iterable-com.groupdocs.search.dictionaries.AliasReplacementPair--}
```
public abstract void addRange(Iterable<AliasReplacementPair> pairs)
```


Προσθέτει τη συγκεκριμένη συλλογή ζευγών ψευδώνυμου/αντικατάστασης σε αυτήν την περίπτωση του AliasDictionary.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | pairs | java.lang.Iterable<com.groupdocs.search.dictionaries.AliasReplacementPair> | Η συλλογή των ζευγών ψευδώνυμου/αντικατάστασης για προσθήκη στο λεξικό. |
|

### addRange(AliasReplacementPair[] pairs) {#addRange-com.groupdocs.search.dictionaries.AliasReplacementPair---}
```
public abstract void addRange(AliasReplacementPair[] pairs)
```


Προσθέτει τη συγκεκριμένη συλλογή ζευγών ψευδώνυμου/αντικατάστασης σε αυτήν την περίπτωση του AliasDictionary.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | pairs | [AliasReplacementPair\[\]](../../com.groupdocs.search.dictionaries/aliasreplacementpair) | Η συλλογή των ζευγών ψευδώνυμου/αντικατάστασης για προσθήκη στο λεξικό. |
|

### add(String alias, String text) {#add-java.lang.String-java.lang.String-}
```
public abstract void add(String alias, String text)
```


Προσθέτει το συγκεκριμένο ζευγάρι ψευδώνυμου και σχετικού κειμένου σε αυτήν την περίπτωση του AliasDictionary.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | alias | java.lang.String | Το ψευδώνυμο για προσθήκη στο λεξικό. |
|
|  | text | java.lang.String | Το κείμενο που θα συσχετιστεί με το ψευδώνυμο. |
|

### remove(String alias) {#remove-java.lang.String-}
```
public abstract boolean remove(String alias)
```


Αφαιρεί το συγκεκριμένο ψευδώνυμο από ένα αντικείμενο AliasDictionary.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | alias | java.lang.String | Το ψευδώνυμο για αφαίρεση. |
|

**Returns:**
boolean - Αυτή η μέθοδος επιστρέφει  true  εάν το ψευδώνυμο βρεθεί επιτυχώς και αφαιρεθεί. Η μέθοδος επιστρέφει  false  εάν το ψευδώνυμο δεν βρεθεί στο αντικείμενο  AliasDictionary .

### contains(String alias) {#contains-java.lang.String-}
```
public abstract boolean contains(String alias)
```


Καθορίζει εάν ένα αντικείμενο AliasDictionary περιέχει το συγκεκριμένο ψευδώνυμο.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | alias | java.lang.String | Το ψευδώνυμο προς εντοπισμό στο αντικείμενο  AliasDictionary . |
|

**Returns:**
boolean -  true  εάν το αντικείμενο  AliasDictionary  περιέχει το καθορισμένο ψευδώνυμο· διαφορετικά,  false .

### getText(String alias) {#getText-java.lang.String-}
```
public abstract String getText(String alias)
```


Λαμβάνει ένα κείμενο που συνδέεται με το συγκεκριμένο ψευδώνυμο.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | alias | java.lang.String | Το ψευδώνυμο προς εντοπισμό στο αντικείμενο  AliasDictionary . |
|

**Returns:**
java.lang.String - Ένα κείμενο που σχετίζεται με το καθορισμένο ψευδώνυμο ή  null .

### clear() {#clear--}
```
public abstract void clear()
```


Αφαιρεί όλα τα ψευδώνυμα από ένα αντικείμενο AliasDictionary.


### iterator() {#iterator--}
```
public abstract Iterator<String> iterator()
```


Επιστρέφει έναν επαναλήπτη που διασχίζει τη συλλογή.


**Returns:**
java.util.Iterator<java.lang.String> - Ένας επαναλήπτης που μπορεί να χρησιμοποιηθεί για επανάληψη μέσω της συλλογής.

