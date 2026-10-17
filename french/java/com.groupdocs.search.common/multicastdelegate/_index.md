---
title: "MulticastDelegate"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Représente un délégué qui fait référence à des instances de classe possédant une méthode à invoquer."
type: docs
weight: 26
url: /fr/java/com.groupdocs.search.common/multicastdelegate/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.Delegate](../../com.groupdocs.search.common/delegate)
```
public abstract class MulticastDelegate extends Delegate
```

Représente un délégué, qui fait référence à des instances de classe possédant une méthode à invoquer.

## Constructeurs

| Constructeur | Description |
| --- | --- |
| [MulticastDelegate()](#MulticastDelegate--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getInvocationList()](#getInvocationList--) | Renvoie une liste d'invocation. |
|
|  | [getDelegateId()](#getDelegateId--) | Renvoie un ID de délégué. |
|
|  | [op_Equality(MulticastDelegate d1, MulticastDelegate d2)](#op-Equality-com.groupdocs.search.common.MulticastDelegate-com.groupdocs.search.common.MulticastDelegate-) | Vérifie l'égalité de deux délégués. |
|
|  | [op_Inequality(MulticastDelegate d1, MulticastDelegate d2)](#op-Inequality-com.groupdocs.search.common.MulticastDelegate-com.groupdocs.search.common.MulticastDelegate-) | Vérifie la différence de deux délégués. |
|
### MulticastDelegate() {#MulticastDelegate--}
```
public MulticastDelegate()
```


### getInvocationList() {#getInvocationList--}
```
public final Delegate[] getInvocationList()
```


Renvoie une liste d'invocation.


**Returns:**
com.groupdocs.search.common.Delegate[] - Une liste d'invocation.

### getDelegateId() {#getDelegateId--}
```
public String getDelegateId()
```


Renvoie un ID de délégué.


**Returns:**
java.lang.String - Un ID de délégué.

### op_Equality(MulticastDelegate d1, MulticastDelegate d2) {#op-Equality-com.groupdocs.search.common.MulticastDelegate-com.groupdocs.search.common.MulticastDelegate-}
```
public static boolean op_Equality(MulticastDelegate d1, MulticastDelegate d2)
```


Vérifie l'égalité de deux délégués.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | d1 | [MulticastDelegate](../../com.groupdocs.search.common/multicastdelegate) | Le premier délégué. |
|
|  | d2 | [MulticastDelegate](../../com.groupdocs.search.common/multicastdelegate) | Le deuxième délégué. |
|

**Returns:**
boolean - Le résultat de la vérification de l'égalité de deux délégués.

### op_Inequality(MulticastDelegate d1, MulticastDelegate d2) {#op-Inequality-com.groupdocs.search.common.MulticastDelegate-com.groupdocs.search.common.MulticastDelegate-}
```
public static boolean op_Inequality(MulticastDelegate d1, MulticastDelegate d2)
```


Vérifie la différence de deux délégués.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | d1 | [MulticastDelegate](../../com.groupdocs.search.common/multicastdelegate) | Le premier délégué. |
|
|  | d2 | [MulticastDelegate](../../com.groupdocs.search.common/multicastdelegate) | Le deuxième délégué. |
|

**Returns:**
boolean - Le résultat de la vérification de l'inégalité de deux délégués.

