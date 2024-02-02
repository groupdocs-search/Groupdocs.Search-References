---
title: MulticastDelegate
second_title: GroupDocs.Search for Java API Reference
description: Represents a delegate which refers to class instances that have method to be invoked.
type: docs
weight: 26
url: /java/com.groupdocs.search.common/multicastdelegate/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.Delegate](../../com.groupdocs.search.common/delegate)
```
public abstract class MulticastDelegate extends Delegate
```

Represents a delegate, which refers to class instances that have method to be invoked.
## Constructors

| Constructor | Description |
| --- | --- |
| [MulticastDelegate()](#MulticastDelegate--) |  |
## Methods

| Method | Description |
| --- | --- |
| [getInvocationList()](#getInvocationList--) | Returns an invocation list. |
| [getDelegateId()](#getDelegateId--) | Returns a delegate ID. |
| [op_Equality(MulticastDelegate d1, MulticastDelegate d2)](#op-Equality-com.groupdocs.search.common.MulticastDelegate-com.groupdocs.search.common.MulticastDelegate-) | Checks two delegates for equality. |
| [op_Inequality(MulticastDelegate d1, MulticastDelegate d2)](#op-Inequality-com.groupdocs.search.common.MulticastDelegate-com.groupdocs.search.common.MulticastDelegate-) | Checks two delegates for inequality. |
### MulticastDelegate() {#MulticastDelegate--}
```
public MulticastDelegate()
```


### getInvocationList() {#getInvocationList--}
```
public final Delegate[] getInvocationList()
```


Returns an invocation list.

**Returns:**
com.groupdocs.search.common.Delegate[] - An invocation list.
### getDelegateId() {#getDelegateId--}
```
public String getDelegateId()
```


Returns a delegate ID.

**Returns:**
java.lang.String - A delegate ID.
### op_Equality(MulticastDelegate d1, MulticastDelegate d2) {#op-Equality-com.groupdocs.search.common.MulticastDelegate-com.groupdocs.search.common.MulticastDelegate-}
```
public static boolean op_Equality(MulticastDelegate d1, MulticastDelegate d2)
```


Checks two delegates for equality.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| d1 | [MulticastDelegate](../../com.groupdocs.search.common/multicastdelegate) | The first delegate. |
| d2 | [MulticastDelegate](../../com.groupdocs.search.common/multicastdelegate) | The second delegate. |

**Returns:**
boolean - The result of checking two delegates for equality.
### op_Inequality(MulticastDelegate d1, MulticastDelegate d2) {#op-Inequality-com.groupdocs.search.common.MulticastDelegate-com.groupdocs.search.common.MulticastDelegate-}
```
public static boolean op_Inequality(MulticastDelegate d1, MulticastDelegate d2)
```


Checks two delegates for inequality.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| d1 | [MulticastDelegate](../../com.groupdocs.search.common/multicastdelegate) | The first delegate. |
| d2 | [MulticastDelegate](../../com.groupdocs.search.common/multicastdelegate) | The second delegate. |

**Returns:**
boolean - The result of checking two delegates for inequality.
