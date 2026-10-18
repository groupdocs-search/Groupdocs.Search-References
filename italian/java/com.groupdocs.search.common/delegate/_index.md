---
title: "Delegate"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Rappresenta un delegato che si riferisce a un'istanza di classe che possiede un metodo da invocare."
type: docs
weight: 14
url: /it/java/com.groupdocs.search.common/delegate/
---
**Inheritance:**
java.lang.Object
```
public abstract class Delegate
```

Rappresenta un delegato, che si riferisce a un'istanza di classe che possiede un metodo da invocare.

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [Delegate()](#Delegate--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getInvocationList()](#getInvocationList--) | Restituisce un elenco di invocazioni. |
|
|  | [combine(Delegate a, Delegate b)](#combine-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-) | Combina due delegati in uno. |
|
|  | [combine(Delegate[] delegates)](#combine-com.groupdocs.search.common.Delegate...-) | Combina diversi delegati in uno. |
|
|  | [remove(Delegate source, Delegate value)](#remove-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-) | Rimuove il delegato valore dal delegato sorgente. |
|
|  | [removeAll(Delegate source, Delegate value)](#removeAll-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-) | Rimuove il delegato valore dal delegato sorgente. |
|
|  | [op_Equality(Delegate d1, Delegate d2)](#op-Equality-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-) | Verifica l'uguaglianza di due delegati. |
|
|  | [op_Inequality(Delegate d1, Delegate d2)](#op-Inequality-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-) | Verifica la disuguaglianza di due delegati. |
|
### Delegate() {#Delegate--}
```
public Delegate()
```


### getInvocationList() {#getInvocationList--}
```
public Delegate[] getInvocationList()
```


Restituisce un elenco di invocazioni.


**Returns:**
com.groupdocs.search.common.Delegate[] - Un elenco di invocazioni.

### combine(Delegate a, Delegate b) {#combine-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-}
```
public static Delegate combine(Delegate a, Delegate b)
```


Combina due delegati in uno.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | a | [Delegate](../../com.groupdocs.search.common/delegate) | Il primo delegato da combinare. |
|
|  | b | [Delegate](../../com.groupdocs.search.common/delegate) | Il secondo delegato da combinare. |
|

**Returns:**
[Delegate](../../com.groupdocs.search.common/delegate) - A new combined delegate.

### combine(Delegate[] delegates) {#combine-com.groupdocs.search.common.Delegate...-}
```
public static Delegate combine(Delegate[] delegates)
```


Combina diversi delegati in uno.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | delegates | [Delegate\[\]](../../com.groupdocs.search.common/delegate) | I delegati da combinare. |
|

**Returns:**
[Delegate](../../com.groupdocs.search.common/delegate) - A new combined delegate.

### remove(Delegate source, Delegate value) {#remove-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-}
```
public static Delegate remove(Delegate source, Delegate value)
```


Rimuove il delegato valore dal delegato sorgente.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | source | [Delegate](../../com.groupdocs.search.common/delegate) | Il delegato sorgente. |
|
|  | value | [Delegate](../../com.groupdocs.search.common/delegate) | Il delegato valore. |
|

**Returns:**
[Delegate](../../com.groupdocs.search.common/delegate) - A new delegate that is a result of removing.

### removeAll(Delegate source, Delegate value) {#removeAll-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-}
```
public static Delegate removeAll(Delegate source, Delegate value)
```


Rimuove il delegato valore dal delegato sorgente.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | source | [Delegate](../../com.groupdocs.search.common/delegate) | Il delegato sorgente. |
|
|  | value | [Delegate](../../com.groupdocs.search.common/delegate) | Il delegato valore. |
|

**Returns:**
[Delegate](../../com.groupdocs.search.common/delegate) - A new delegate that is a result of removing.

### op_Equality(Delegate d1, Delegate d2) {#op-Equality-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-}
```
public static boolean op_Equality(Delegate d1, Delegate d2)
```


Verifica l'uguaglianza di due delegati.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | d1 | [Delegate](../../com.groupdocs.search.common/delegate) | Il primo delegato. |
|
|  | d2 | [Delegate](../../com.groupdocs.search.common/delegate) | Il secondo delegato. |
|

**Returns:**
boolean - Il risultato del controllo di due delegati per uguaglianza.

### op_Inequality(Delegate d1, Delegate d2) {#op-Inequality-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-}
```
public static boolean op_Inequality(Delegate d1, Delegate d2)
```


Verifica la disuguaglianza di due delegati.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | d1 | [Delegate](../../com.groupdocs.search.common/delegate) | Il primo delegato. |
|
|  | d2 | [Delegate](../../com.groupdocs.search.common/delegate) | Il secondo delegato. |
|

**Returns:**
boolean - Il risultato del controllo di due delegati per disuguaglianza.

