---
title: "Συμβάν"
second_title: "GroupDocs.Search για Java API Reference"
description: "Αυτή η κλάση προορίζεται να κληρονομείται όταν εγγράφεστε σε γεγονότα."
type: docs
weight: 11
url: /el/java/com.groupdocs.search.events/event/
---
**Inheritance:**
java.lang.Object
```
public abstract class Event<T>
```

Αυτή η κλάση προορίζεται να κληρονομείται όταν εγγράφεστε σε γεγονότα.

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [Event()](#Event--) | Αρχικοποιεί ένα νέο στιγμιότυπο της  Event  κλάσης. |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [add(T delegate)](#add-T-) | Προσθέτει έναν ακροατή για το συμβάν. |
|
|  | [remove(T delegate)](#remove-T-) | Αφαιρεί έναν ακροατή για το συμβάν. |
|
|  | [isEmpty()](#isEmpty--) | Ελέγχει την παρουσία τουλάχιστον ενός ακροατή. |
|
### Event() {#Event--}
```
public Event()
```


Αρχικοποιεί ένα νέο στιγμιότυπο της  Event  κλάσης.


### add(T delegate) {#add-T-}
```
public final synchronized void add(T delegate)
```


Προσθέτει έναν ακροατή για το συμβάν.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | delegate | T | Ένας ακροατής για το συμβάν προς προσθήκη. |
|

### remove(T delegate) {#remove-T-}
```
public final synchronized void remove(T delegate)
```


Αφαιρεί έναν ακροατή για το συμβάν.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | delegate | T | Ένας ακροατής για το συμβάν προς αφαίρεση. |
|

### isEmpty() {#isEmpty--}
```
public synchronized boolean isEmpty()
```


Ελέγχει την παρουσία τουλάχιστον ενός ακροατή.


**Returns:**
boolean - Μια τιμή που υποδεικνύει ότι τουλάχιστον ένας ακροατής προστέθηκε για το συμβάν.

