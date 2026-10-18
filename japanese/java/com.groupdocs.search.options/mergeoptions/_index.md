---
title: "MergeOptions"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "マージ操作のオプションを提供します。"
type: docs
weight: 28
url: /ja/java/com.groupdocs.search.options/mergeoptions/
---
**Inheritance:**
java.lang.Object
```
public class MergeOptions
```

マージ操作のオプションを提供します。


**Learn more**

* [Merge indexes](../https://docs.groupdocs.com/display/searchjava/Merge+indexes)
* [Optimize index](../https://docs.groupdocs.com/display/searchjava/Optimize+index)

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [MergeOptions()](#MergeOptions--) | MergeOptions クラスの新しいインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [isAsync()](#isAsync--) | 操作を非同期で実行するフラグを取得します。 |
|
|  | [setAsync(boolean value)](#setAsync-boolean-) | 操作を非同期で実行するフラグを設定します。 |
|
|  | [getCancellation()](#getCancellation--) | 操作のキャンセルオブジェクトを取得します。 |
|
|  | [setCancellation(Cancellation value)](#setCancellation-com.groupdocs.search.common.Cancellation-) | 操作のキャンセルオブジェクトを設定します。 |
|
### MergeOptions() {#MergeOptions--}
```
public MergeOptions()
```


MergeOptions クラスの新しいインスタンスを初期化します。


### isAsync() {#isAsync--}
```
public final boolean isAsync()
```


操作を非同期で実行するフラグを取得します。デフォルト値は false です。


**Returns:**
boolean - 操作を非同期で実行するフラグ。

### setAsync(boolean value) {#setAsync-boolean-}
```
public final void setAsync(boolean value)
```


操作を非同期で実行するフラグを設定します。デフォルト値は false です。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 値 | boolean | 操作を非同期で実行するフラグ。 |
|

### getCancellation() {#getCancellation--}
```
public final Cancellation getCancellation()
```


操作のキャンセルオブジェクトを取得します。デフォルト値は null です。


**Returns:**
[Cancellation](../../com.groupdocs.search.common/cancellation) - The operation cancellation object.

### setCancellation(Cancellation value) {#setCancellation-com.groupdocs.search.common.Cancellation-}
```
public final void setCancellation(Cancellation value)
```


操作のキャンセルオブジェクトを設定します。デフォルト値は null です。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | value | [Cancellation](../../com.groupdocs.search.common/cancellation) | 操作のキャンセルオブジェクト。 |
|

