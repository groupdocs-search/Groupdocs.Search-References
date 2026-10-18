---
title: "MulticastDelegate"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Representa un delegado que se refiere a instancias de clase que poseen un método que será invocado."
type: docs
weight: 26
url: /es/java/com.groupdocs.search.common/multicastdelegate/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.Delegate](../../com.groupdocs.search.common/delegate)
```
public abstract class MulticastDelegate extends Delegate
```

Representa un delegado, que se refiere a instancias de clase que tienen un método que será invocado.

## Constructores

| Constructor | Descripción |
| --- | --- |
| [MulticastDelegate()](#MulticastDelegate--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getInvocationList()](#getInvocationList--) | Devuelve una lista de invocación. |
|
|  | [getDelegateId()](#getDelegateId--) | Devuelve un ID de delegado. |
|
|  | [op_Equality(MulticastDelegate d1, MulticastDelegate d2)](#op-Equality-com.groupdocs.search.common.MulticastDelegate-com.groupdocs.search.common.MulticastDelegate-) | Comprueba la igualdad de dos delegados. |
|
|  | [op_Inequality(MulticastDelegate d1, MulticastDelegate d2)](#op-Inequality-com.groupdocs.search.common.MulticastDelegate-com.groupdocs.search.common.MulticastDelegate-) | Comprueba la desigualdad de dos delegados. |
|
### MulticastDelegate() {#MulticastDelegate--}
```
public MulticastDelegate()
```


### getInvocationList() {#getInvocationList--}
```
public final Delegate[] getInvocationList()
```


Devuelve una lista de invocación.


**Returns:**
com.groupdocs.search.common.Delegate[] - Una lista de invocación.

### getDelegateId() {#getDelegateId--}
```
public String getDelegateId()
```


Devuelve un ID de delegado.


**Returns:**
java.lang.String - Un ID de delegado.

### op_Equality(MulticastDelegate d1, MulticastDelegate d2) {#op-Equality-com.groupdocs.search.common.MulticastDelegate-com.groupdocs.search.common.MulticastDelegate-}
```
public static boolean op_Equality(MulticastDelegate d1, MulticastDelegate d2)
```


Comprueba la igualdad de dos delegados.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | d1 | [MulticastDelegate](../../com.groupdocs.search.common/multicastdelegate) | El primer delegado. |
|
|  | d2 | [MulticastDelegate](../../com.groupdocs.search.common/multicastdelegate) | El segundo delegado. |
|

**Returns:**
boolean - El resultado de comprobar la igualdad de dos delegados.

### op_Inequality(MulticastDelegate d1, MulticastDelegate d2) {#op-Inequality-com.groupdocs.search.common.MulticastDelegate-com.groupdocs.search.common.MulticastDelegate-}
```
public static boolean op_Inequality(MulticastDelegate d1, MulticastDelegate d2)
```


Comprueba la desigualdad de dos delegados.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | d1 | [MulticastDelegate](../../com.groupdocs.search.common/multicastdelegate) | El primer delegado. |
|
|  | d2 | [MulticastDelegate](../../com.groupdocs.search.common/multicastdelegate) | El segundo delegado. |
|

**Returns:**
boolean - El resultado de comprobar la desigualdad de dos delegados.

