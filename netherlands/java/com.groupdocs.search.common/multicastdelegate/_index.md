---
title: "MulticastDelegate"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Stelt een delegate voor die verwijst naar klasse‑instanties die een methode hebben die moet worden aangeroepen."
type: docs
weight: 26
url: /nl/java/com.groupdocs.search.common/multicastdelegate/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.Delegate](../../com.groupdocs.search.common/delegate)
```
public abstract class MulticastDelegate extends Delegate
```

Stelt een delegate voor, die verwijst naar klasse‑instanties met een methode die moet worden aangeroepen.

## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [MulticastDelegate()](#MulticastDelegate--) |  |
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getInvocationList()](#getInvocationList--) | Retourneert een aanroeplijst. |
|
|  | [getDelegateId()](#getDelegateId--) | Retourneert een delegate‑ID. |
|
|  | [op_Equality(MulticastDelegate d1, MulticastDelegate d2)](#op-Equality-com.groupdocs.search.common.MulticastDelegate-com.groupdocs.search.common.MulticastDelegate-) | Controleert twee delegates op gelijkheid. |
|
|  | [op_Inequality(MulticastDelegate d1, MulticastDelegate d2)](#op-Inequality-com.groupdocs.search.common.MulticastDelegate-com.groupdocs.search.common.MulticastDelegate-) | Controleert twee delegates op ongelijkheid. |
|
### MulticastDelegate() {#MulticastDelegate--}
```
public MulticastDelegate()
```


### getInvocationList() {#getInvocationList--}
```
public final Delegate[] getInvocationList()
```


Retourneert een aanroeplijst.


**Returns:**
com.groupdocs.search.common.Delegate[] - Een aanroeplijst.

### getDelegateId() {#getDelegateId--}
```
public String getDelegateId()
```


Retourneert een delegate‑ID.


**Returns:**
java.lang.String - Een delegate‑ID.

### op_Equality(MulticastDelegate d1, MulticastDelegate d2) {#op-Equality-com.groupdocs.search.common.MulticastDelegate-com.groupdocs.search.common.MulticastDelegate-}
```
public static boolean op_Equality(MulticastDelegate d1, MulticastDelegate d2)
```


Controleert twee delegates op gelijkheid.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | d1 | [MulticastDelegate](../../com.groupdocs.search.common/multicastdelegate) | De eerste delegate. |
|
|  | d2 | [MulticastDelegate](../../com.groupdocs.search.common/multicastdelegate) | De tweede delegate. |
|

**Returns:**
boolean - Het resultaat van het controleren van twee delegates op gelijkheid.

### op_Inequality(MulticastDelegate d1, MulticastDelegate d2) {#op-Inequality-com.groupdocs.search.common.MulticastDelegate-com.groupdocs.search.common.MulticastDelegate-}
```
public static boolean op_Inequality(MulticastDelegate d1, MulticastDelegate d2)
```


Controleert twee delegates op ongelijkheid.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | d1 | [MulticastDelegate](../../com.groupdocs.search.common/multicastdelegate) | De eerste delegate. |
|
|  | d2 | [MulticastDelegate](../../com.groupdocs.search.common/multicastdelegate) | De tweede delegate. |
|

**Returns:**
boolean - Het resultaat van het controleren van twee delegates op ongelijkheid.

