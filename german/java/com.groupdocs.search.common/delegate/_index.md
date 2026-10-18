---
title: "Delegate"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Stellt einen Delegaten dar, der auf eine Klasseninstanz verweist, die eine aufzurufende Methode hat."
type: docs
weight: 14
url: /de/java/com.groupdocs.search.common/delegate/
---
**Inheritance:**
java.lang.Object
```
public abstract class Delegate
```

Stellt einen Delegaten dar, der auf eine Klasseninstanz verweist, die eine aufzurufende Methode hat.

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [Delegate()](#Delegate--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getInvocationList()](#getInvocationList--) | Gibt eine Aufrufliste zurück. |
|
|  | [combine(Delegate a, Delegate b)](#combine-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-) | Kombiniert zwei Delegaten zu einem. |
|
|  | [combine(Delegate[] delegates)](#combine-com.groupdocs.search.common.Delegate...-) | Kombiniert mehrere Delegaten zu einem. |
|
|  | [remove(Delegate source, Delegate value)](#remove-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-) | Entfernt den Wert-Delegaten vom Quell-Delegaten. |
|
|  | [removeAll(Delegate source, Delegate value)](#removeAll-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-) | Entfernt den Wert-Delegaten vom Quell-Delegaten. |
|
|  | [op_Equality(Delegate d1, Delegate d2)](#op-Equality-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-) | Überprüft zwei Delegaten auf Gleichheit. |
|
|  | [op_Inequality(Delegate d1, Delegate d2)](#op-Inequality-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-) | Überprüft zwei Delegaten auf Ungleichheit. |
|
### Delegate() {#Delegate--}
```
public Delegate()
```


### getInvocationList() {#getInvocationList--}
```
public Delegate[] getInvocationList()
```


Gibt eine Aufrufliste zurück.


**Returns:**
com.groupdocs.search.common.Delegate[] - Eine Aufrufliste.

### combine(Delegate a, Delegate b) {#combine-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-}
```
public static Delegate combine(Delegate a, Delegate b)
```


Kombiniert zwei Delegaten zu einem.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | a | [Delegate](../../com.groupdocs.search.common/delegate) | Der erste zu kombinierende Delegat. |
|
|  | b | [Delegate](../../com.groupdocs.search.common/delegate) | Der zweite Delegat zum Kombinieren. |
|

**Returns:**
[Delegate](../../com.groupdocs.search.common/delegate) - A new combined delegate.

### combine(Delegate[] delegates) {#combine-com.groupdocs.search.common.Delegate...-}
```
public static Delegate combine(Delegate[] delegates)
```


Kombiniert mehrere Delegaten zu einem.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | delegates | [Delegate\[\]](../../com.groupdocs.search.common/delegate) | Die Delegaten zum Kombinieren. |
|

**Returns:**
[Delegate](../../com.groupdocs.search.common/delegate) - A new combined delegate.

### remove(Delegate source, Delegate value) {#remove-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-}
```
public static Delegate remove(Delegate source, Delegate value)
```


Entfernt den Wert-Delegaten vom Quell-Delegaten.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | source | [Delegate](../../com.groupdocs.search.common/delegate) | Der Quell-Delegat. |
|
|  | value | [Delegate](../../com.groupdocs.search.common/delegate) | Der Wert-Delegat. |
|

**Returns:**
[Delegate](../../com.groupdocs.search.common/delegate) - A new delegate that is a result of removing.

### removeAll(Delegate source, Delegate value) {#removeAll-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-}
```
public static Delegate removeAll(Delegate source, Delegate value)
```


Entfernt den Wert-Delegaten vom Quell-Delegaten.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | source | [Delegate](../../com.groupdocs.search.common/delegate) | Der Quell-Delegat. |
|
|  | value | [Delegate](../../com.groupdocs.search.common/delegate) | Der Wert-Delegat. |
|

**Returns:**
[Delegate](../../com.groupdocs.search.common/delegate) - A new delegate that is a result of removing.

### op_Equality(Delegate d1, Delegate d2) {#op-Equality-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-}
```
public static boolean op_Equality(Delegate d1, Delegate d2)
```


Überprüft zwei Delegaten auf Gleichheit.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | d1 | [Delegate](../../com.groupdocs.search.common/delegate) | Der erste Delegat. |
|
|  | d2 | [Delegate](../../com.groupdocs.search.common/delegate) | Der zweite Delegat. |
|

**Returns:**
boolean - Das Ergebnis der Überprüfung zweier Delegaten auf Gleichheit.

### op_Inequality(Delegate d1, Delegate d2) {#op-Inequality-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-}
```
public static boolean op_Inequality(Delegate d1, Delegate d2)
```


Überprüft zwei Delegaten auf Ungleichheit.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | d1 | [Delegate](../../com.groupdocs.search.common/delegate) | Der erste Delegat. |
|
|  | d2 | [Delegate](../../com.groupdocs.search.common/delegate) | Der zweite Delegat. |
|

**Returns:**
boolean - Das Ergebnis der Überprüfung zweier Delegaten auf Ungleichheit.

