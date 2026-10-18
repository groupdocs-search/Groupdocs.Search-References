---
title: "Delegate"
second_title: "GroupDocs.Search för Java API-referens"
description: "Representerar en delegat som refererar till en klassinstans som har en metod som ska anropas."
type: docs
weight: 14
url: /sv/java/com.groupdocs.search.common/delegate/
---
**Inheritance:**
java.lang.Object
```
public abstract class Delegate
```

Representerar en delegat som refererar till en klassinstans som har en metod som ska anropas.

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [Delegate()](#Delegate--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getInvocationList()](#getInvocationList--) | Returnerar en anropslista. |
|
|  | [combine(Delegate a, Delegate b)](#combine-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-) | Kombinerar två delegater till en. |
|
|  | [combine(Delegate[] delegates)](#combine-com.groupdocs.search.common.Delegate...-) | Kombinerar flera delegater till en. |
|
|  | [remove(Delegate source, Delegate value)](#remove-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-) | Tar bort värdelegaten från källdelegaten. |
|
|  | [removeAll(Delegate source, Delegate value)](#removeAll-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-) | Tar bort värdelegaten från källdelegaten. |
|
|  | [op_Equality(Delegate d1, Delegate d2)](#op-Equality-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-) | Kontrollerar två delegater för likhet. |
|
|  | [op_Inequality(Delegate d1, Delegate d2)](#op-Inequality-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-) | Kontrollerar två delegater för olikhet. |
|
### Delegate() {#Delegate--}
```
public Delegate()
```


### getInvocationList() {#getInvocationList--}
```
public Delegate[] getInvocationList()
```


Returnerar en anropslista.


**Returns:**
com.groupdocs.search.common.Delegate[] - En anropslista.

### combine(Delegate a, Delegate b) {#combine-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-}
```
public static Delegate combine(Delegate a, Delegate b)
```


Kombinerar två delegater till en.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | a | [Delegate](../../com.groupdocs.search.common/delegate) | Den första delegaten att kombinera. |
|
|  | b | [Delegate](../../com.groupdocs.search.common/delegate) | Den andra delegaten att kombinera. |
|

**Returns:**
[Delegate](../../com.groupdocs.search.common/delegate) - A new combined delegate.

### combine(Delegate[] delegates) {#combine-com.groupdocs.search.common.Delegate...-}
```
public static Delegate combine(Delegate[] delegates)
```


Kombinerar flera delegater till en.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | delegates | [Delegate\[\]](../../com.groupdocs.search.common/delegate) | Delegaterna att kombinera. |
|

**Returns:**
[Delegate](../../com.groupdocs.search.common/delegate) - A new combined delegate.

### remove(Delegate source, Delegate value) {#remove-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-}
```
public static Delegate remove(Delegate source, Delegate value)
```


Tar bort värdelegaten från källdelegaten.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | source | [Delegate](../../com.groupdocs.search.common/delegate) | Källdelegaten. |
|
|  | value | [Delegate](../../com.groupdocs.search.common/delegate) | Värdedelegaten. |
|

**Returns:**
[Delegate](../../com.groupdocs.search.common/delegate) - A new delegate that is a result of removing.

### removeAll(Delegate source, Delegate value) {#removeAll-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-}
```
public static Delegate removeAll(Delegate source, Delegate value)
```


Tar bort värdelegaten från källdelegaten.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | source | [Delegate](../../com.groupdocs.search.common/delegate) | Källdelegaten. |
|
|  | value | [Delegate](../../com.groupdocs.search.common/delegate) | Värdedelegaten. |
|

**Returns:**
[Delegate](../../com.groupdocs.search.common/delegate) - A new delegate that is a result of removing.

### op_Equality(Delegate d1, Delegate d2) {#op-Equality-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-}
```
public static boolean op_Equality(Delegate d1, Delegate d2)
```


Kontrollerar två delegater för likhet.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | d1 | [Delegate](../../com.groupdocs.search.common/delegate) | Den första delegaten. |
|
|  | d2 | [Delegate](../../com.groupdocs.search.common/delegate) | Den andra delegaten. |
|

**Returns:**
boolean - Resultatet av att kontrollera två delegater för likhet.

### op_Inequality(Delegate d1, Delegate d2) {#op-Inequality-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-}
```
public static boolean op_Inequality(Delegate d1, Delegate d2)
```


Kontrollerar två delegater för olikhet.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | d1 | [Delegate](../../com.groupdocs.search.common/delegate) | Den första delegaten. |
|
|  | d2 | [Delegate](../../com.groupdocs.search.common/delegate) | Den andra delegaten. |
|

**Returns:**
boolean - Resultatet av att kontrollera två delegater för ojämlikhet.

