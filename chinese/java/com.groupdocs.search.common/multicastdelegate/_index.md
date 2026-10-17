---
title: "MulticastDelegate"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "表示一个委托，该委托引用具有可调用方法的类实例。"
type: docs
weight: 26
url: /zh/java/com.groupdocs.search.common/multicastdelegate/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.Delegate](../../com.groupdocs.search.common/delegate)
```
public abstract class MulticastDelegate extends Delegate
```

表示委托，引用具有可调用方法的类实例。

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [MulticastDelegate()](#MulticastDelegate--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getInvocationList()](#getInvocationList--) | 返回调用列表。 |
|
|  | [getDelegateId()](#getDelegateId--) | 返回委托 ID。 |
|
|  | [op_Equality(MulticastDelegate d1, MulticastDelegate d2)](#op-Equality-com.groupdocs.search.common.MulticastDelegate-com.groupdocs.search.common.MulticastDelegate-) | 检查两个委托是否相等。 |
|
|  | [op_Inequality(MulticastDelegate d1, MulticastDelegate d2)](#op-Inequality-com.groupdocs.search.common.MulticastDelegate-com.groupdocs.search.common.MulticastDelegate-) | 检查两个委托是否不相等。 |
|
### MulticastDelegate() {#MulticastDelegate--}
```
public MulticastDelegate()
```


### getInvocationList() {#getInvocationList--}
```
public final Delegate[] getInvocationList()
```


返回调用列表。


**Returns:**
com.groupdocs.search.common.Delegate[] - 调用列表。

### getDelegateId() {#getDelegateId--}
```
public String getDelegateId()
```


返回委托 ID。


**Returns:**
java.lang.String - 委托 ID。

### op_Equality(MulticastDelegate d1, MulticastDelegate d2) {#op-Equality-com.groupdocs.search.common.MulticastDelegate-com.groupdocs.search.common.MulticastDelegate-}
```
public static boolean op_Equality(MulticastDelegate d1, MulticastDelegate d2)
```


检查两个委托是否相等。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | d1 | [MulticastDelegate](../../com.groupdocs.search.common/multicastdelegate) | 第一个委托。 |
|
|  | d2 | [MulticastDelegate](../../com.groupdocs.search.common/multicastdelegate) | 第二个委托。 |
|

**Returns:**
boolean - 检查两个委托是否相等的结果。

### op_Inequality(MulticastDelegate d1, MulticastDelegate d2) {#op-Inequality-com.groupdocs.search.common.MulticastDelegate-com.groupdocs.search.common.MulticastDelegate-}
```
public static boolean op_Inequality(MulticastDelegate d1, MulticastDelegate d2)
```


检查两个委托是否不相等。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | d1 | [MulticastDelegate](../../com.groupdocs.search.common/multicastdelegate) | 第一个委托。 |
|
|  | d2 | [MulticastDelegate](../../com.groupdocs.search.common/multicastdelegate) | 第二个委托。 |
|

**Returns:**
boolean - 检查两个委托是否不相等的结果。

