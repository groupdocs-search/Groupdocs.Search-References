---
title: "MulticastDelegate"
second_title: "GroupDocs.Search για Java API Reference"
description: "Αντιπροσωπεύει έναν delegate που αναφέρεται σε παρουσίες κλάσης που έχουν μέθοδο προς κλήση."
type: docs
weight: 26
url: /el/java/com.groupdocs.search.common/multicastdelegate/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.Delegate](../../com.groupdocs.search.common/delegate)
```
public abstract class MulticastDelegate extends Delegate
```

Αναπαριστά έναν αντιπρόσωπο, που αναφέρεται σε παρουσίες κλάσεων που έχουν μέθοδο προς κλήση.

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [MulticastDelegate()](#MulticastDelegate--) |  |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getInvocationList()](#getInvocationList--) | Επιστρέφει μια λίστα κλήσεων. |
|
|  | [getDelegateId()](#getDelegateId--) | Επιστρέφει ένα αναγνωριστικό delegate. |
|
|  | [op_Equality(MulticastDelegate d1, MulticastDelegate d2)](#op-Equality-com.groupdocs.search.common.MulticastDelegate-com.groupdocs.search.common.MulticastDelegate-) | Ελέγχει δύο delegates για ισότητα. |
|
|  | [op_Inequality(MulticastDelegate d1, MulticastDelegate d2)](#op-Inequality-com.groupdocs.search.common.MulticastDelegate-com.groupdocs.search.common.MulticastDelegate-) | Ελέγχει δύο delegates για ανισότητα. |
|
### MulticastDelegate() {#MulticastDelegate--}
```
public MulticastDelegate()
```


### getInvocationList() {#getInvocationList--}
```
public final Delegate[] getInvocationList()
```


Επιστρέφει μια λίστα κλήσεων.


**Returns:**
com.groupdocs.search.common.Delegate[] - Μια λίδα κλήσεων.

### getDelegateId() {#getDelegateId--}
```
public String getDelegateId()
```


Επιστρέφει ένα αναγνωριστικό delegate.


**Returns:**
java.lang.String - Ένα αναγνωριστικό delegate.

### op_Equality(MulticastDelegate d1, MulticastDelegate d2) {#op-Equality-com.groupdocs.search.common.MulticastDelegate-com.groupdocs.search.common.MulticastDelegate-}
```
public static boolean op_Equality(MulticastDelegate d1, MulticastDelegate d2)
```


Ελέγχει δύο delegates για ισότητα.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | d1 | [MulticastDelegate](../../com.groupdocs.search.common/multicastdelegate) | Ο πρώτος εκπρόσωπος. |
|
|  | d2 | [MulticastDelegate](../../com.groupdocs.search.common/multicastdelegate) | Ο δεύτερος εκπρόσωπος. |
|

**Returns:**
boolean - Το αποτέλεσμα του ελέγχου δύο εκπροσώπων για ισότητα.

### op_Inequality(MulticastDelegate d1, MulticastDelegate d2) {#op-Inequality-com.groupdocs.search.common.MulticastDelegate-com.groupdocs.search.common.MulticastDelegate-}
```
public static boolean op_Inequality(MulticastDelegate d1, MulticastDelegate d2)
```


Ελέγχει δύο delegates για ανισότητα.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | d1 | [MulticastDelegate](../../com.groupdocs.search.common/multicastdelegate) | Ο πρώτος εκπρόσωπος. |
|
|  | d2 | [MulticastDelegate](../../com.groupdocs.search.common/multicastdelegate) | Ο δεύτερος εκπρόσωπος. |
|

**Returns:**
boolean - Το αποτέλεσμα του ελέγχου δύο εκπροσώπων για ανισότητα.

