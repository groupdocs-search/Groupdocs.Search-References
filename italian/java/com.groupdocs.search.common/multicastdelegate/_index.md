---
title: "MulticastDelegate"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Rappresenta un delegato che si riferisce a istanze di classe che hanno un metodo da invocare."
type: docs
weight: 26
url: /it/java/com.groupdocs.search.common/multicastdelegate/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.Delegate](../../com.groupdocs.search.common/delegate)
```
public abstract class MulticastDelegate extends Delegate
```

Rappresenta un delegato, che si riferisce a istanze di classe che hanno un metodo da invocare.

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [MulticastDelegate()](#MulticastDelegate--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getInvocationList()](#getInvocationList--) | Restituisce un elenco di invocazioni. |
|
|  | [getDelegateId()](#getDelegateId--) | Restituisce un ID delegato. |
|
|  | [op_Equality(MulticastDelegate d1, MulticastDelegate d2)](#op-Equality-com.groupdocs.search.common.MulticastDelegate-com.groupdocs.search.common.MulticastDelegate-) | Verifica l'uguaglianza di due delegati. |
|
|  | [op_Inequality(MulticastDelegate d1, MulticastDelegate d2)](#op-Inequality-com.groupdocs.search.common.MulticastDelegate-com.groupdocs.search.common.MulticastDelegate-) | Verifica la disuguaglianza di due delegati. |
|
### MulticastDelegate() {#MulticastDelegate--}
```
public MulticastDelegate()
```


### getInvocationList() {#getInvocationList--}
```
public final Delegate[] getInvocationList()
```


Restituisce un elenco di invocazioni.


**Returns:**
com.groupdocs.search.common.Delegate[] - Un elenco di invocazioni.

### getDelegateId() {#getDelegateId--}
```
public String getDelegateId()
```


Restituisce un ID delegato.


**Returns:**
java.lang.String - Un ID delegato.

### op_Equality(MulticastDelegate d1, MulticastDelegate d2) {#op-Equality-com.groupdocs.search.common.MulticastDelegate-com.groupdocs.search.common.MulticastDelegate-}
```
public static boolean op_Equality(MulticastDelegate d1, MulticastDelegate d2)
```


Verifica l'uguaglianza di due delegati.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | d1 | [MulticastDelegate](../../com.groupdocs.search.common/multicastdelegate) | Il primo delegato. |
|
|  | d2 | [MulticastDelegate](../../com.groupdocs.search.common/multicastdelegate) | Il secondo delegato. |
|

**Returns:**
boolean - Il risultato del controllo di due delegati per uguaglianza.

### op_Inequality(MulticastDelegate d1, MulticastDelegate d2) {#op-Inequality-com.groupdocs.search.common.MulticastDelegate-com.groupdocs.search.common.MulticastDelegate-}
```
public static boolean op_Inequality(MulticastDelegate d1, MulticastDelegate d2)
```


Verifica la disuguaglianza di due delegati.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | d1 | [MulticastDelegate](../../com.groupdocs.search.common/multicastdelegate) | Il primo delegato. |
|
|  | d2 | [MulticastDelegate](../../com.groupdocs.search.common/multicastdelegate) | Il secondo delegato. |
|

**Returns:**
boolean - Il risultato del controllo di due delegati per disuguaglianza.

