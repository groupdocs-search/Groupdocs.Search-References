---
title: "Delegate"
second_title: "GroupDocs.Search για Java API Reference"
description: "Αντιπροσωπεύει έναν delegate που αναφέρεται σε μια παρουσία κλάσης που έχει μια μέθοδο που θα κληθεί."
type: docs
weight: 14
url: /el/java/com.groupdocs.search.common/delegate/
---
**Inheritance:**
java.lang.Object
```
public abstract class Delegate
```

Αναπαριστά έναν αντιπρόσωπο, που αναφέρεται σε μια παρουσία κλάσης που έχει μια μέθοδο προς κλήση.

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [Delegate()](#Delegate--) |  |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getInvocationList()](#getInvocationList--) | Επιστρέφει μια λίστα κλήσεων. |
|
|  | [combine(Delegate a, Delegate b)](#combine-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-) | Συνδυάζει δύο delegates σε ένα. |
|
|  | [combine(Delegate[] delegates)](#combine-com.groupdocs.search.common.Delegate...-) | Συνδυάζει πολλούς delegates σε ένα. |
|
|  | [remove(Delegate source, Delegate value)](#remove-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-) | Αφαιρεί το delegate τιμής από το πηγαίο delegate. |
|
|  | [removeAll(Delegate source, Delegate value)](#removeAll-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-) | Αφαιρεί το delegate τιμής από το πηγαίο delegate. |
|
|  | [op_Equality(Delegate d1, Delegate d2)](#op-Equality-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-) | Ελέγχει δύο delegates για ισότητα. |
|
|  | [op_Inequality(Delegate d1, Delegate d2)](#op-Inequality-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-) | Ελέγχει δύο delegates για ανισότητα. |
|
### Delegate() {#Delegate--}
```
public Delegate()
```


### getInvocationList() {#getInvocationList--}
```
public Delegate[] getInvocationList()
```


Επιστρέφει μια λίστα κλήσεων.


**Returns:**
com.groupdocs.search.common.Delegate[] - Μια λίδα κλήσεων.

### combine(Delegate a, Delegate b) {#combine-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-}
```
public static Delegate combine(Delegate a, Delegate b)
```


Συνδυάζει δύο delegates σε ένα.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | a | [Delegate](../../com.groupdocs.search.common/delegate) | Ο πρώτος delegate για συνδυασμό. |
|
|  | b | [Delegate](../../com.groupdocs.search.common/delegate) | Ο δεύτερος εκπρόσωπος για συνδυασμό. |
|

**Returns:**
[Delegate](../../com.groupdocs.search.common/delegate) - A new combined delegate.

### combine(Delegate[] delegates) {#combine-com.groupdocs.search.common.Delegate...-}
```
public static Delegate combine(Delegate[] delegates)
```


Συνδυάζει πολλούς delegates σε ένα.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | delegates | [Delegate\[\]](../../com.groupdocs.search.common/delegate) | Οι εκπρόσωποι για συνδυασμό. |
|

**Returns:**
[Delegate](../../com.groupdocs.search.common/delegate) - A new combined delegate.

### remove(Delegate source, Delegate value) {#remove-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-}
```
public static Delegate remove(Delegate source, Delegate value)
```


Αφαιρεί το delegate τιμής από το πηγαίο delegate.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | source | [Delegate](../../com.groupdocs.search.common/delegate) | Ο εκπρόσωπος προέλευσης. |
|
|  | value | [Delegate](../../com.groupdocs.search.common/delegate) | Ο εκπρόσωπος τιμής. |
|

**Returns:**
[Delegate](../../com.groupdocs.search.common/delegate) - A new delegate that is a result of removing.

### removeAll(Delegate source, Delegate value) {#removeAll-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-}
```
public static Delegate removeAll(Delegate source, Delegate value)
```


Αφαιρεί το delegate τιμής από το πηγαίο delegate.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | source | [Delegate](../../com.groupdocs.search.common/delegate) | Ο εκπρόσωπος προέλευσης. |
|
|  | value | [Delegate](../../com.groupdocs.search.common/delegate) | Ο εκπρόσωπος τιμής. |
|

**Returns:**
[Delegate](../../com.groupdocs.search.common/delegate) - A new delegate that is a result of removing.

### op_Equality(Delegate d1, Delegate d2) {#op-Equality-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-}
```
public static boolean op_Equality(Delegate d1, Delegate d2)
```


Ελέγχει δύο delegates για ισότητα.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | d1 | [Delegate](../../com.groupdocs.search.common/delegate) | Ο πρώτος εκπρόσωπος. |
|
|  | d2 | [Delegate](../../com.groupdocs.search.common/delegate) | Ο δεύτερος εκπρόσωπος. |
|

**Returns:**
boolean - Το αποτέλεσμα του ελέγχου δύο εκπροσώπων για ισότητα.

### op_Inequality(Delegate d1, Delegate d2) {#op-Inequality-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-}
```
public static boolean op_Inequality(Delegate d1, Delegate d2)
```


Ελέγχει δύο delegates για ανισότητα.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | d1 | [Delegate](../../com.groupdocs.search.common/delegate) | Ο πρώτος εκπρόσωπος. |
|
|  | d2 | [Delegate](../../com.groupdocs.search.common/delegate) | Ο δεύτερος εκπρόσωπος. |
|

**Returns:**
boolean - Το αποτέλεσμα του ελέγχου δύο εκπροσώπων για ανισότητα.

