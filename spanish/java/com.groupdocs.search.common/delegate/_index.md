---
title: "Delegate"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Representa un delegado que se refiere a una instancia de clase que tiene un método que será invocado."
type: docs
weight: 14
url: /es/java/com.groupdocs.search.common/delegate/
---
**Inheritance:**
java.lang.Object
```
public abstract class Delegate
```

Representa un delegado, que se refiere a una instancia de clase que tiene un método que será invocado.

## Constructores

| Constructor | Descripción |
| --- | --- |
| [Delegate()](#Delegate--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getInvocationList()](#getInvocationList--) | Devuelve una lista de invocación. |
|
|  | [combine(Delegate a, Delegate b)](#combine-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-) | Combina dos delegados en uno. |
|
|  | [combine(Delegate[] delegates)](#combine-com.groupdocs.search.common.Delegate...-) | Combina varios delegados en uno. |
|
|  | [remove(Delegate source, Delegate value)](#remove-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-) | Elimina el delegado de valor del delegado origen. |
|
|  | [removeAll(Delegate source, Delegate value)](#removeAll-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-) | Elimina el delegado de valor del delegado origen. |
|
|  | [op_Equality(Delegate d1, Delegate d2)](#op-Equality-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-) | Comprueba la igualdad de dos delegados. |
|
|  | [op_Inequality(Delegate d1, Delegate d2)](#op-Inequality-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-) | Comprueba la desigualdad de dos delegados. |
|
### Delegate() {#Delegate--}
```
public Delegate()
```


### getInvocationList() {#getInvocationList--}
```
public Delegate[] getInvocationList()
```


Devuelve una lista de invocación.


**Returns:**
com.groupdocs.search.common.Delegate[] - Una lista de invocación.

### combine(Delegate a, Delegate b) {#combine-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-}
```
public static Delegate combine(Delegate a, Delegate b)
```


Combina dos delegados en uno.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | a | [Delegate](../../com.groupdocs.search.common/delegate) | El primer delegado a combinar. |
|
|  | b | [Delegate](../../com.groupdocs.search.common/delegate) | El segundo delegado para combinar. |
|

**Returns:**
[Delegate](../../com.groupdocs.search.common/delegate) - A new combined delegate.

### combine(Delegate[] delegates) {#combine-com.groupdocs.search.common.Delegate...-}
```
public static Delegate combine(Delegate[] delegates)
```


Combina varios delegados en uno.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | delegates | [Delegate\[\]](../../com.groupdocs.search.common/delegate) | Los delegados para combinar. |
|

**Returns:**
[Delegate](../../com.groupdocs.search.common/delegate) - A new combined delegate.

### remove(Delegate source, Delegate value) {#remove-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-}
```
public static Delegate remove(Delegate source, Delegate value)
```


Elimina el delegado de valor del delegado origen.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | source | [Delegate](../../com.groupdocs.search.common/delegate) | El delegado de origen. |
|
|  | value | [Delegate](../../com.groupdocs.search.common/delegate) | El delegado de valor. |
|

**Returns:**
[Delegate](../../com.groupdocs.search.common/delegate) - A new delegate that is a result of removing.

### removeAll(Delegate source, Delegate value) {#removeAll-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-}
```
public static Delegate removeAll(Delegate source, Delegate value)
```


Elimina el delegado de valor del delegado origen.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | source | [Delegate](../../com.groupdocs.search.common/delegate) | El delegado de origen. |
|
|  | value | [Delegate](../../com.groupdocs.search.common/delegate) | El delegado de valor. |
|

**Returns:**
[Delegate](../../com.groupdocs.search.common/delegate) - A new delegate that is a result of removing.

### op_Equality(Delegate d1, Delegate d2) {#op-Equality-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-}
```
public static boolean op_Equality(Delegate d1, Delegate d2)
```


Comprueba la igualdad de dos delegados.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | d1 | [Delegate](../../com.groupdocs.search.common/delegate) | El primer delegado. |
|
|  | d2 | [Delegate](../../com.groupdocs.search.common/delegate) | El segundo delegado. |
|

**Returns:**
boolean - El resultado de comprobar la igualdad de dos delegados.

### op_Inequality(Delegate d1, Delegate d2) {#op-Inequality-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-}
```
public static boolean op_Inequality(Delegate d1, Delegate d2)
```


Comprueba la desigualdad de dos delegados.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | d1 | [Delegate](../../com.groupdocs.search.common/delegate) | El primer delegado. |
|
|  | d2 | [Delegate](../../com.groupdocs.search.common/delegate) | El segundo delegado. |
|

**Returns:**
boolean - El resultado de comprobar la desigualdad de dos delegados.

