---
title: "MulticastDelegate"
second_title: "GroupDocs.Search för Java API-referens"
description: "Representerar en delegat som refererar till klassinstanser som har en metod som ska anropas."
type: docs
weight: 26
url: /sv/java/com.groupdocs.search.common/multicastdelegate/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.Delegate](../../com.groupdocs.search.common/delegate)
```
public abstract class MulticastDelegate extends Delegate
```

Representerar en delegat som refererar till klassinstanser som har en metod som ska anropas.

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [MulticastDelegate()](#MulticastDelegate--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getInvocationList()](#getInvocationList--) | Returnerar en anropslista. |
|
|  | [getDelegateId()](#getDelegateId--) | Returnerar ett delegat-ID. |
|
|  | [op_Equality(MulticastDelegate d1, MulticastDelegate d2)](#op-Equality-com.groupdocs.search.common.MulticastDelegate-com.groupdocs.search.common.MulticastDelegate-) | Kontrollerar två delegater för likhet. |
|
|  | [op_Inequality(MulticastDelegate d1, MulticastDelegate d2)](#op-Inequality-com.groupdocs.search.common.MulticastDelegate-com.groupdocs.search.common.MulticastDelegate-) | Kontrollerar två delegater för olikhet. |
|
### MulticastDelegate() {#MulticastDelegate--}
```
public MulticastDelegate()
```


### getInvocationList() {#getInvocationList--}
```
public final Delegate[] getInvocationList()
```


Returnerar en anropslista.


**Returns:**
com.groupdocs.search.common.Delegate[] - En anropslista.

### getDelegateId() {#getDelegateId--}
```
public String getDelegateId()
```


Returnerar ett delegat-ID.


**Returns:**
java.lang.String - Ett delegat-ID.

### op_Equality(MulticastDelegate d1, MulticastDelegate d2) {#op-Equality-com.groupdocs.search.common.MulticastDelegate-com.groupdocs.search.common.MulticastDelegate-}
```
public static boolean op_Equality(MulticastDelegate d1, MulticastDelegate d2)
```


Kontrollerar två delegater för likhet.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | d1 | [MulticastDelegate](../../com.groupdocs.search.common/multicastdelegate) | Den första delegaten. |
|
|  | d2 | [MulticastDelegate](../../com.groupdocs.search.common/multicastdelegate) | Den andra delegaten. |
|

**Returns:**
boolean - Resultatet av att kontrollera två delegater för likhet.

### op_Inequality(MulticastDelegate d1, MulticastDelegate d2) {#op-Inequality-com.groupdocs.search.common.MulticastDelegate-com.groupdocs.search.common.MulticastDelegate-}
```
public static boolean op_Inequality(MulticastDelegate d1, MulticastDelegate d2)
```


Kontrollerar två delegater för olikhet.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | d1 | [MulticastDelegate](../../com.groupdocs.search.common/multicastdelegate) | Den första delegaten. |
|
|  | d2 | [MulticastDelegate](../../com.groupdocs.search.common/multicastdelegate) | Den andra delegaten. |
|

**Returns:**
boolean - Resultatet av att kontrollera två delegater för ojämlikhet.

