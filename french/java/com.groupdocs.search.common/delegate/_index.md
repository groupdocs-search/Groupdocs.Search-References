---
title: "Delegate"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Représente un délégué qui fait référence à une instance de classe possédant une méthode à invoquer."
type: docs
weight: 14
url: /fr/java/com.groupdocs.search.common/delegate/
---
**Inheritance:**
java.lang.Object
```
public abstract class Delegate
```

Représente un délégué, qui fait référence à une instance de classe possédant une méthode à invoquer.

## Constructeurs

| Constructeur | Description |
| --- | --- |
| [Delegate()](#Delegate--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getInvocationList()](#getInvocationList--) | Renvoie une liste d'invocation. |
|
|  | [combine(Delegate a, Delegate b)](#combine-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-) | Combine deux délégués en un seul. |
|
|  | [combine(Delegate[] delegates)](#combine-com.groupdocs.search.common.Delegate...-) | Combine plusieurs délégués en un seul. |
|
|  | [remove(Delegate source, Delegate value)](#remove-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-) | Supprime le délégué de valeur du délégué source. |
|
|  | [removeAll(Delegate source, Delegate value)](#removeAll-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-) | Supprime le délégué de valeur du délégué source. |
|
|  | [op_Equality(Delegate d1, Delegate d2)](#op-Equality-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-) | Vérifie l'égalité de deux délégués. |
|
|  | [op_Inequality(Delegate d1, Delegate d2)](#op-Inequality-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-) | Vérifie la différence de deux délégués. |
|
### Delegate() {#Delegate--}
```
public Delegate()
```


### getInvocationList() {#getInvocationList--}
```
public Delegate[] getInvocationList()
```


Renvoie une liste d'invocation.


**Returns:**
com.groupdocs.search.common.Delegate[] - Une liste d'invocation.

### combine(Delegate a, Delegate b) {#combine-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-}
```
public static Delegate combine(Delegate a, Delegate b)
```


Combine deux délégués en un seul.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | a | [Delegate](../../com.groupdocs.search.common/delegate) | Le premier délégué à combiner. |
|
|  | b | [Delegate](../../com.groupdocs.search.common/delegate) | Le deuxième délégué à combiner. |
|

**Returns:**
[Delegate](../../com.groupdocs.search.common/delegate) - A new combined delegate.

### combine(Delegate[] delegates) {#combine-com.groupdocs.search.common.Delegate...-}
```
public static Delegate combine(Delegate[] delegates)
```


Combine plusieurs délégués en un seul.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | delegates | [Delegate\[\]](../../com.groupdocs.search.common/delegate) | Les délégués à combiner. |
|

**Returns:**
[Delegate](../../com.groupdocs.search.common/delegate) - A new combined delegate.

### remove(Delegate source, Delegate value) {#remove-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-}
```
public static Delegate remove(Delegate source, Delegate value)
```


Supprime le délégué de valeur du délégué source.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | source | [Delegate](../../com.groupdocs.search.common/delegate) | Le délégué source. |
|
|  | value | [Delegate](../../com.groupdocs.search.common/delegate) | Le délégué de valeur. |
|

**Returns:**
[Delegate](../../com.groupdocs.search.common/delegate) - A new delegate that is a result of removing.

### removeAll(Delegate source, Delegate value) {#removeAll-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-}
```
public static Delegate removeAll(Delegate source, Delegate value)
```


Supprime le délégué de valeur du délégué source.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | source | [Delegate](../../com.groupdocs.search.common/delegate) | Le délégué source. |
|
|  | value | [Delegate](../../com.groupdocs.search.common/delegate) | Le délégué de valeur. |
|

**Returns:**
[Delegate](../../com.groupdocs.search.common/delegate) - A new delegate that is a result of removing.

### op_Equality(Delegate d1, Delegate d2) {#op-Equality-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-}
```
public static boolean op_Equality(Delegate d1, Delegate d2)
```


Vérifie l'égalité de deux délégués.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | d1 | [Delegate](../../com.groupdocs.search.common/delegate) | Le premier délégué. |
|
|  | d2 | [Delegate](../../com.groupdocs.search.common/delegate) | Le deuxième délégué. |
|

**Returns:**
boolean - Le résultat de la vérification de l'égalité de deux délégués.

### op_Inequality(Delegate d1, Delegate d2) {#op-Inequality-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-}
```
public static boolean op_Inequality(Delegate d1, Delegate d2)
```


Vérifie la différence de deux délégués.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | d1 | [Delegate](../../com.groupdocs.search.common/delegate) | Le premier délégué. |
|
|  | d2 | [Delegate](../../com.groupdocs.search.common/delegate) | Le deuxième délégué. |
|

**Returns:**
boolean - Le résultat de la vérification de l'inégalité de deux délégués.

