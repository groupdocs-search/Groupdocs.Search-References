---
title: "MulticastDelegate"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Stellt einen Delegaten dar, der sich auf Klasseninstanzen bezieht, die eine aufzurufende Methode besitzen."
type: docs
weight: 26
url: /de/java/com.groupdocs.search.common/multicastdelegate/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.Delegate](../../com.groupdocs.search.common/delegate)
```
public abstract class MulticastDelegate extends Delegate
```

Stellt einen Delegaten dar, der auf Klasseninstanzen verweist, die eine aufzurufende Methode haben.

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [MulticastDelegate()](#MulticastDelegate--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getInvocationList()](#getInvocationList--) | Gibt eine Aufrufliste zurück. |
|
|  | [getDelegateId()](#getDelegateId--) | Gibt eine Delegaten-ID zurück. |
|
|  | [op_Equality(MulticastDelegate d1, MulticastDelegate d2)](#op-Equality-com.groupdocs.search.common.MulticastDelegate-com.groupdocs.search.common.MulticastDelegate-) | Überprüft zwei Delegaten auf Gleichheit. |
|
|  | [op_Inequality(MulticastDelegate d1, MulticastDelegate d2)](#op-Inequality-com.groupdocs.search.common.MulticastDelegate-com.groupdocs.search.common.MulticastDelegate-) | Überprüft zwei Delegaten auf Ungleichheit. |
|
### MulticastDelegate() {#MulticastDelegate--}
```
public MulticastDelegate()
```


### getInvocationList() {#getInvocationList--}
```
public final Delegate[] getInvocationList()
```


Gibt eine Aufrufliste zurück.


**Returns:**
com.groupdocs.search.common.Delegate[] - Eine Aufrufliste.

### getDelegateId() {#getDelegateId--}
```
public String getDelegateId()
```


Gibt eine Delegaten-ID zurück.


**Returns:**
java.lang.String - Eine Delegaten-ID.

### op_Equality(MulticastDelegate d1, MulticastDelegate d2) {#op-Equality-com.groupdocs.search.common.MulticastDelegate-com.groupdocs.search.common.MulticastDelegate-}
```
public static boolean op_Equality(MulticastDelegate d1, MulticastDelegate d2)
```


Überprüft zwei Delegaten auf Gleichheit.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | d1 | [MulticastDelegate](../../com.groupdocs.search.common/multicastdelegate) | Der erste Delegat. |
|
|  | d2 | [MulticastDelegate](../../com.groupdocs.search.common/multicastdelegate) | Der zweite Delegat. |
|

**Returns:**
boolean - Das Ergebnis der Überprüfung zweier Delegaten auf Gleichheit.

### op_Inequality(MulticastDelegate d1, MulticastDelegate d2) {#op-Inequality-com.groupdocs.search.common.MulticastDelegate-com.groupdocs.search.common.MulticastDelegate-}
```
public static boolean op_Inequality(MulticastDelegate d1, MulticastDelegate d2)
```


Überprüft zwei Delegaten auf Ungleichheit.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | d1 | [MulticastDelegate](../../com.groupdocs.search.common/multicastdelegate) | Der erste Delegat. |
|
|  | d2 | [MulticastDelegate](../../com.groupdocs.search.common/multicastdelegate) | Der zweite Delegat. |
|

**Returns:**
boolean - Das Ergebnis der Überprüfung zweier Delegaten auf Ungleichheit.

