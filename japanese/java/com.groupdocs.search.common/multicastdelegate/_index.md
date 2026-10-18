---
title: "MulticastDelegate"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "呼び出されるメソッドを持つクラスインスタンスを参照するデリゲートを表します。"
type: docs
weight: 26
url: /ja/java/com.groupdocs.search.common/multicastdelegate/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.Delegate](../../com.groupdocs.search.common/delegate)
```
public abstract class MulticastDelegate extends Delegate
```

呼び出されるメソッドを持つクラスインスタンスを参照するデリゲートを表します。

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [MulticastDelegate()](#MulticastDelegate--) |  |
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getInvocationList()](#getInvocationList--) | 呼び出しリストを返します。 |
|
|  | [getDelegateId()](#getDelegateId--) | デリゲート ID を返します。 |
|
|  | [op_Equality(MulticastDelegate d1, MulticastDelegate d2)](#op-Equality-com.groupdocs.search.common.MulticastDelegate-com.groupdocs.search.common.MulticastDelegate-) | 2つのデリゲートが等しいかチェックします。 |
|
|  | [op_Inequality(MulticastDelegate d1, MulticastDelegate d2)](#op-Inequality-com.groupdocs.search.common.MulticastDelegate-com.groupdocs.search.common.MulticastDelegate-) | 2つのデリゲートが等しくないかチェックします。 |
|
### MulticastDelegate() {#MulticastDelegate--}
```
public MulticastDelegate()
```


### getInvocationList() {#getInvocationList--}
```
public final Delegate[] getInvocationList()
```


呼び出しリストを返します。


**Returns:**
com.groupdocs.search.common.Delegate[] - 呼び出しリスト。

### getDelegateId() {#getDelegateId--}
```
public String getDelegateId()
```


デリゲート ID を返します。


**Returns:**
java.lang.String - デリゲート ID。

### op_Equality(MulticastDelegate d1, MulticastDelegate d2) {#op-Equality-com.groupdocs.search.common.MulticastDelegate-com.groupdocs.search.common.MulticastDelegate-}
```
public static boolean op_Equality(MulticastDelegate d1, MulticastDelegate d2)
```


2つのデリゲートが等しいかチェックします。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | d1 | [MulticastDelegate](../../com.groupdocs.search.common/multicastdelegate) | 最初のデリゲート。 |
|
|  | d2 | [MulticastDelegate](../../com.groupdocs.search.common/multicastdelegate) | 2番目のデリゲート。 |
|

**Returns:**
boolean - 2つのデリゲートが等しいかチェックした結果。

### op_Inequality(MulticastDelegate d1, MulticastDelegate d2) {#op-Inequality-com.groupdocs.search.common.MulticastDelegate-com.groupdocs.search.common.MulticastDelegate-}
```
public static boolean op_Inequality(MulticastDelegate d1, MulticastDelegate d2)
```


2つのデリゲートが等しくないかチェックします。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | d1 | [MulticastDelegate](../../com.groupdocs.search.common/multicastdelegate) | 最初のデリゲート。 |
|
|  | d2 | [MulticastDelegate](../../com.groupdocs.search.common/multicastdelegate) | 2番目のデリゲート。 |
|

**Returns:**
boolean - 2つのデリゲートの不等価性をチェックした結果。

