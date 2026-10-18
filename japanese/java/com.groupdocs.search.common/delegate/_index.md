---
title: "Delegate"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "呼び出されるメソッドを持つクラスインスタンスを参照するデリゲートを表します。"
type: docs
weight: 14
url: /ja/java/com.groupdocs.search.common/delegate/
---
**Inheritance:**
java.lang.Object
```
public abstract class Delegate
```

呼び出されるメソッドを持つクラスインスタンスを参照するデリゲートを表します。

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [Delegate()](#Delegate--) |  |
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getInvocationList()](#getInvocationList--) | 呼び出しリストを返します。 |
|
|  | [combine(Delegate a, Delegate b)](#combine-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-) | 2つのデリゲートを1つに結合します。 |
|
|  | [combine(Delegate[] delegates)](#combine-com.groupdocs.search.common.Delegate...-) | 複数のデリゲートを1つに結合します。 |
|
|  | [remove(Delegate source, Delegate value)](#remove-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-) | ソースデリゲートから値デリゲートを削除します。 |
|
|  | [removeAll(Delegate source, Delegate value)](#removeAll-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-) | ソースデリゲートから値デリゲートを削除します。 |
|
|  | [op_Equality(Delegate d1, Delegate d2)](#op-Equality-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-) | 2つのデリゲートが等しいかチェックします。 |
|
|  | [op_Inequality(Delegate d1, Delegate d2)](#op-Inequality-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-) | 2つのデリゲートが等しくないかチェックします。 |
|
### Delegate() {#Delegate--}
```
public Delegate()
```


### getInvocationList() {#getInvocationList--}
```
public Delegate[] getInvocationList()
```


呼び出しリストを返します。


**Returns:**
com.groupdocs.search.common.Delegate[] - 呼び出しリスト。

### combine(Delegate a, Delegate b) {#combine-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-}
```
public static Delegate combine(Delegate a, Delegate b)
```


2つのデリゲートを1つに結合します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | a | [Delegate](../../com.groupdocs.search.common/delegate) | 結合する最初のデリゲート。 |
|
|  | b | [Delegate](../../com.groupdocs.search.common/delegate) | 結合する2番目のデリゲート。 |
|

**Returns:**
[Delegate](../../com.groupdocs.search.common/delegate) - A new combined delegate.

### combine(Delegate[] delegates) {#combine-com.groupdocs.search.common.Delegate...-}
```
public static Delegate combine(Delegate[] delegates)
```


複数のデリゲートを1つに結合します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | delegates | [Delegate\[\]](../../com.groupdocs.search.common/delegate) | 結合するデリゲート。 |
|

**Returns:**
[Delegate](../../com.groupdocs.search.common/delegate) - A new combined delegate.

### remove(Delegate source, Delegate value) {#remove-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-}
```
public static Delegate remove(Delegate source, Delegate value)
```


ソースデリゲートから値デリゲートを削除します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | source | [Delegate](../../com.groupdocs.search.common/delegate) | ソースデリゲート。 |
|
|  | value | [Delegate](../../com.groupdocs.search.common/delegate) | 値デリゲート。 |
|

**Returns:**
[Delegate](../../com.groupdocs.search.common/delegate) - A new delegate that is a result of removing.

### removeAll(Delegate source, Delegate value) {#removeAll-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-}
```
public static Delegate removeAll(Delegate source, Delegate value)
```


ソースデリゲートから値デリゲートを削除します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | source | [Delegate](../../com.groupdocs.search.common/delegate) | ソースデリゲート。 |
|
|  | value | [Delegate](../../com.groupdocs.search.common/delegate) | 値デリゲート。 |
|

**Returns:**
[Delegate](../../com.groupdocs.search.common/delegate) - A new delegate that is a result of removing.

### op_Equality(Delegate d1, Delegate d2) {#op-Equality-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-}
```
public static boolean op_Equality(Delegate d1, Delegate d2)
```


2つのデリゲートが等しいかチェックします。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | d1 | [Delegate](../../com.groupdocs.search.common/delegate) | 最初のデリゲート。 |
|
|  | d2 | [Delegate](../../com.groupdocs.search.common/delegate) | 2番目のデリゲート。 |
|

**Returns:**
boolean - 2つのデリゲートが等しいかチェックした結果。

### op_Inequality(Delegate d1, Delegate d2) {#op-Inequality-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-}
```
public static boolean op_Inequality(Delegate d1, Delegate d2)
```


2つのデリゲートが等しくないかチェックします。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | d1 | [Delegate](../../com.groupdocs.search.common/delegate) | 最初のデリゲート。 |
|
|  | d2 | [Delegate](../../com.groupdocs.search.common/delegate) | 2番目のデリゲート。 |
|

**Returns:**
boolean - 2つのデリゲートの不等価性をチェックした結果。

