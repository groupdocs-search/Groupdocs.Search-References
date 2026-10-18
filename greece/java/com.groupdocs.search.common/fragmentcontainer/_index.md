---
title: "FragmentContainer"
second_title: "GroupDocs.Search για Java API Reference"
description: "Αναπαριστά ένα δοχείο για αποσπάσματα κειμένου με επισημασμένους εντοπισμένους όρους ενός πεδίου εγγράφου."
type: docs
weight: 22
url: /el/java/com.groupdocs.search.common/fragmentcontainer/
---
**Inheritance:**
java.lang.Object
```
public abstract class FragmentContainer
```

Αναπαριστά ένα δοχείο για αποσπάσματα κειμένου με επισημασμένους εντοπισμένους όρους ενός πεδίου εγγράφου.


**Learn more**

* [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [FragmentContainer()](#FragmentContainer--) |  |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getFieldName()](#getFieldName--) | Αποκτά το όνομα του πεδίου του εγγράφου. |
|
|  | [getCount()](#getCount--) | Αποκτά τον αριθμό των περιεχομένων τμημάτων κειμένου. |
|
|  | [getFragments()](#getFragments--) | Αποκτά έναν πίνακα των περιεχομένων τμημάτων κειμένου. |
|
### FragmentContainer() {#FragmentContainer--}
```
public FragmentContainer()
```


### getFieldName() {#getFieldName--}
```
public abstract String getFieldName()
```


Αποκτά το όνομα του πεδίου του εγγράφου.


**Returns:**
java.lang.String - Το όνομα του πεδίου του εγγράφου.

### getCount() {#getCount--}
```
public abstract int getCount()
```


Αποκτά τον αριθμό των περιεχομένων τμημάτων κειμένου.


**Returns:**
int - Ο αριθμός των περιεχομένων τμημάτων κειμένου.

### getFragments() {#getFragments--}
```
public abstract String[] getFragments()
```


Αποκτά έναν πίνακα των περιεχομένων τμημάτων κειμένου.


**Returns:**
java.lang.String[] - Ένας πίνακας των περιεχομένων τμημάτων κειμένου.

