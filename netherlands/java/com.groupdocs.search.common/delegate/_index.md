---
title: "Delegate"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Stelt een delegate voor die verwijst naar een klasse-instatie die een methode heeft die moet worden aangeroepen."
type: docs
weight: 14
url: /nl/java/com.groupdocs.search.common/delegate/
---
**Inheritance:**
java.lang.Object
```
public abstract class Delegate
```

Stelt een delegate voor, die verwijst naar een klasse‑instantie met een methode die moet worden aangeroepen.

## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [Delegate()](#Delegate--) |  |
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getInvocationList()](#getInvocationList--) | Retourneert een aanroeplijst. |
|
|  | [combine(Delegate a, Delegate b)](#combine-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-) | Combineert twee delegates tot één. |
|
|  | [combine(Delegate[] delegates)](#combine-com.groupdocs.search.common.Delegate...-) | Combineert meerdere delegates tot één. |
|
|  | [remove(Delegate source, Delegate value)](#remove-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-) | Verwijdert de waardedelegate van de bron-delegate. |
|
|  | [removeAll(Delegate source, Delegate value)](#removeAll-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-) | Verwijdert de waardedelegate van de bron-delegate. |
|
|  | [op_Equality(Delegate d1, Delegate d2)](#op-Equality-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-) | Controleert twee delegates op gelijkheid. |
|
|  | [op_Inequality(Delegate d1, Delegate d2)](#op-Inequality-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-) | Controleert twee delegates op ongelijkheid. |
|
### Delegate() {#Delegate--}
```
public Delegate()
```


### getInvocationList() {#getInvocationList--}
```
public Delegate[] getInvocationList()
```


Retourneert een aanroeplijst.


**Returns:**
com.groupdocs.search.common.Delegate[] - Een aanroeplijst.

### combine(Delegate a, Delegate b) {#combine-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-}
```
public static Delegate combine(Delegate a, Delegate b)
```


Combineert twee delegates tot één.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | a | [Delegate](../../com.groupdocs.search.common/delegate) | De eerste delegate om te combineren. |
|
|  | b | [Delegate](../../com.groupdocs.search.common/delegate) | De tweede delegate om te combineren. |
|

**Returns:**
[Delegate](../../com.groupdocs.search.common/delegate) - A new combined delegate.

### combine(Delegate[] delegates) {#combine-com.groupdocs.search.common.Delegate...-}
```
public static Delegate combine(Delegate[] delegates)
```


Combineert meerdere delegates tot één.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | delegates | [Delegate\[\]](../../com.groupdocs.search.common/delegate) | De delegates om te combineren. |
|

**Returns:**
[Delegate](../../com.groupdocs.search.common/delegate) - A new combined delegate.

### remove(Delegate source, Delegate value) {#remove-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-}
```
public static Delegate remove(Delegate source, Delegate value)
```


Verwijdert de waardedelegate van de bron-delegate.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | source | [Delegate](../../com.groupdocs.search.common/delegate) | De bron-delegate. |
|
|  | value | [Delegate](../../com.groupdocs.search.common/delegate) | De waarde-delegate. |
|

**Returns:**
[Delegate](../../com.groupdocs.search.common/delegate) - A new delegate that is a result of removing.

### removeAll(Delegate source, Delegate value) {#removeAll-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-}
```
public static Delegate removeAll(Delegate source, Delegate value)
```


Verwijdert de waardedelegate van de bron-delegate.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | source | [Delegate](../../com.groupdocs.search.common/delegate) | De bron-delegate. |
|
|  | value | [Delegate](../../com.groupdocs.search.common/delegate) | De waarde-delegate. |
|

**Returns:**
[Delegate](../../com.groupdocs.search.common/delegate) - A new delegate that is a result of removing.

### op_Equality(Delegate d1, Delegate d2) {#op-Equality-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-}
```
public static boolean op_Equality(Delegate d1, Delegate d2)
```


Controleert twee delegates op gelijkheid.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | d1 | [Delegate](../../com.groupdocs.search.common/delegate) | De eerste delegate. |
|
|  | d2 | [Delegate](../../com.groupdocs.search.common/delegate) | De tweede delegate. |
|

**Returns:**
boolean - Het resultaat van het controleren van twee delegates op gelijkheid.

### op_Inequality(Delegate d1, Delegate d2) {#op-Inequality-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-}
```
public static boolean op_Inequality(Delegate d1, Delegate d2)
```


Controleert twee delegates op ongelijkheid.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | d1 | [Delegate](../../com.groupdocs.search.common/delegate) | De eerste delegate. |
|
|  | d2 | [Delegate](../../com.groupdocs.search.common/delegate) | De tweede delegate. |
|

**Returns:**
boolean - Het resultaat van het controleren van twee delegates op ongelijkheid.

