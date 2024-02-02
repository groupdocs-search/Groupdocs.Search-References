---
title: Delegate
second_title: GroupDocs.Search for Java API Reference
description: Represents a delegate which refers to a class instance that has a method to be invoked.
type: docs
weight: 14
url: /java/com.groupdocs.search.common/delegate/
---
**Inheritance:**
java.lang.Object
```
public abstract class Delegate
```

Represents a delegate, which refers to a class instance that has a method to be invoked.
## Constructors

| Constructor | Description |
| --- | --- |
| [Delegate()](#Delegate--) |  |
## Methods

| Method | Description |
| --- | --- |
| [getInvocationList()](#getInvocationList--) | Returns an invocation list. |
| [combine(Delegate a, Delegate b)](#combine-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-) | Combines two delegates into one. |
| [combine(Delegate[] delegates)](#combine-com.groupdocs.search.common.Delegate...-) | Combines several delegates into one. |
| [remove(Delegate source, Delegate value)](#remove-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-) | Removes the value delegate from the source delegate. |
| [removeAll(Delegate source, Delegate value)](#removeAll-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-) | Removes the value delegate from the source delegate. |
| [op_Equality(Delegate d1, Delegate d2)](#op-Equality-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-) | Checks two delegates for equality. |
| [op_Inequality(Delegate d1, Delegate d2)](#op-Inequality-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-) | Checks two delegates for inequality. |
### Delegate() {#Delegate--}
```
public Delegate()
```


### getInvocationList() {#getInvocationList--}
```
public Delegate[] getInvocationList()
```


Returns an invocation list.

**Returns:**
com.groupdocs.search.common.Delegate[] - An invocation list.
### combine(Delegate a, Delegate b) {#combine-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-}
```
public static Delegate combine(Delegate a, Delegate b)
```


Combines two delegates into one.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| a | [Delegate](../../com.groupdocs.search.common/delegate) | The first delegate to combine. |
| b | [Delegate](../../com.groupdocs.search.common/delegate) | The second delegate to combine. |

**Returns:**
[Delegate](../../com.groupdocs.search.common/delegate) - A new combined delegate.
### combine(Delegate[] delegates) {#combine-com.groupdocs.search.common.Delegate...-}
```
public static Delegate combine(Delegate[] delegates)
```


Combines several delegates into one.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| delegates | [Delegate\[\]](../../com.groupdocs.search.common/delegate) | The delegates to combine. |

**Returns:**
[Delegate](../../com.groupdocs.search.common/delegate) - A new combined delegate.
### remove(Delegate source, Delegate value) {#remove-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-}
```
public static Delegate remove(Delegate source, Delegate value)
```


Removes the value delegate from the source delegate.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| source | [Delegate](../../com.groupdocs.search.common/delegate) | The source delegate. |
| value | [Delegate](../../com.groupdocs.search.common/delegate) | The value delegate. |

**Returns:**
[Delegate](../../com.groupdocs.search.common/delegate) - A new delegate that is a result of removing.
### removeAll(Delegate source, Delegate value) {#removeAll-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-}
```
public static Delegate removeAll(Delegate source, Delegate value)
```


Removes the value delegate from the source delegate.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| source | [Delegate](../../com.groupdocs.search.common/delegate) | The source delegate. |
| value | [Delegate](../../com.groupdocs.search.common/delegate) | The value delegate. |

**Returns:**
[Delegate](../../com.groupdocs.search.common/delegate) - A new delegate that is a result of removing.
### op_Equality(Delegate d1, Delegate d2) {#op-Equality-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-}
```
public static boolean op_Equality(Delegate d1, Delegate d2)
```


Checks two delegates for equality.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| d1 | [Delegate](../../com.groupdocs.search.common/delegate) | The first delegate. |
| d2 | [Delegate](../../com.groupdocs.search.common/delegate) | The second delegate. |

**Returns:**
boolean - The result of checking two delegates for equality.
### op_Inequality(Delegate d1, Delegate d2) {#op-Inequality-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-}
```
public static boolean op_Inequality(Delegate d1, Delegate d2)
```


Checks two delegates for inequality.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| d1 | [Delegate](../../com.groupdocs.search.common/delegate) | The first delegate. |
| d2 | [Delegate](../../com.groupdocs.search.common/delegate) | The second delegate. |

**Returns:**
boolean - The result of checking two delegates for inequality.
