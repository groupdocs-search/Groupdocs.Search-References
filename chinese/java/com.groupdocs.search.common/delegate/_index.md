---
title: "Delegate"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "表示引用具有可调用方法的类实例的委托。"
type: docs
weight: 14
url: /zh/java/com.groupdocs.search.common/delegate/
---
**Inheritance:**
java.lang.Object
```
public abstract class Delegate
```

表示委托，引用具有可调用方法的类实例。

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [Delegate()](#Delegate--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getInvocationList()](#getInvocationList--) | 返回调用列表。 |
|
|  | [combine(Delegate a, Delegate b)](#combine-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-) | 将两个委托合并为一个。 |
|
|  | [combine(Delegate[] delegates)](#combine-com.groupdocs.search.common.Delegate...-) | 将多个委托合并为一个。 |
|
|  | [remove(Delegate source, Delegate value)](#remove-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-) | 从源委托中移除值委托。 |
|
|  | [removeAll(Delegate source, Delegate value)](#removeAll-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-) | 从源委托中移除值委托。 |
|
|  | [op_Equality(Delegate d1, Delegate d2)](#op-Equality-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-) | 检查两个委托是否相等。 |
|
|  | [op_Inequality(Delegate d1, Delegate d2)](#op-Inequality-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-) | 检查两个委托是否不相等。 |
|
### Delegate() {#Delegate--}
```
public Delegate()
```


### getInvocationList() {#getInvocationList--}
```
public Delegate[] getInvocationList()
```


返回调用列表。


**Returns:**
com.groupdocs.search.common.Delegate[] - 调用列表。

### combine(Delegate a, Delegate b) {#combine-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-}
```
public static Delegate combine(Delegate a, Delegate b)
```


将两个委托合并为一个。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | a | [Delegate](../../com.groupdocs.search.common/delegate) | 要合并的第一个委托。 |
|
|  | b | [Delegate](../../com.groupdocs.search.common/delegate) | 第二个要合并的委托。 |
|

**Returns:**
[Delegate](../../com.groupdocs.search.common/delegate) - A new combined delegate.

### combine(Delegate[] delegates) {#combine-com.groupdocs.search.common.Delegate...-}
```
public static Delegate combine(Delegate[] delegates)
```


将多个委托合并为一个。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | delegates | [Delegate\[\]](../../com.groupdocs.search.common/delegate) | 要合并的委托。 |
|

**Returns:**
[Delegate](../../com.groupdocs.search.common/delegate) - A new combined delegate.

### remove(Delegate source, Delegate value) {#remove-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-}
```
public static Delegate remove(Delegate source, Delegate value)
```


从源委托中移除值委托。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | source | [Delegate](../../com.groupdocs.search.common/delegate) | 源委托。 |
|
|  | value | [Delegate](../../com.groupdocs.search.common/delegate) | 值委托。 |
|

**Returns:**
[Delegate](../../com.groupdocs.search.common/delegate) - A new delegate that is a result of removing.

### removeAll(Delegate source, Delegate value) {#removeAll-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-}
```
public static Delegate removeAll(Delegate source, Delegate value)
```


从源委托中移除值委托。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | source | [Delegate](../../com.groupdocs.search.common/delegate) | 源委托。 |
|
|  | value | [Delegate](../../com.groupdocs.search.common/delegate) | 值委托。 |
|

**Returns:**
[Delegate](../../com.groupdocs.search.common/delegate) - A new delegate that is a result of removing.

### op_Equality(Delegate d1, Delegate d2) {#op-Equality-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-}
```
public static boolean op_Equality(Delegate d1, Delegate d2)
```


检查两个委托是否相等。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | d1 | [Delegate](../../com.groupdocs.search.common/delegate) | 第一个委托。 |
|
|  | d2 | [Delegate](../../com.groupdocs.search.common/delegate) | 第二个委托。 |
|

**Returns:**
boolean - 检查两个委托是否相等的结果。

### op_Inequality(Delegate d1, Delegate d2) {#op-Inequality-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-}
```
public static boolean op_Inequality(Delegate d1, Delegate d2)
```


检查两个委托是否不相等。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | d1 | [Delegate](../../com.groupdocs.search.common/delegate) | 第一个委托。 |
|
|  | d2 | [Delegate](../../com.groupdocs.search.common/delegate) | 第二个委托。 |
|

**Returns:**
boolean - 检查两个委托是否不相等的结果。

