---
title: "SynchronizeOptions"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "同期操作のオプションを提供します。"
type: docs
weight: 39
url: /ja/java/com.groupdocs.search.options/synchronizeoptions/
---
**Inheritance:**
java.lang.Object
```
public class SynchronizeOptions
```

同期操作のオプションを提供します。

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [SynchronizeOptions()](#SynchronizeOptions--) | SynchronizeOptions クラスの新しいインスタンスを初期化します。 |
|
|  | [SynchronizeOptions(Object data)](#SynchronizeOptions-java.lang.Object-) | SynchronizeOptions クラスの新しいインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [isAsync()](#isAsync--) | 操作を非同期で実行するフラグを取得します。 |
|
|  | [setAsync(boolean value)](#setAsync-boolean-) | 操作を非同期で実行するフラグを設定します。 |
|
| [getCore()](#getCore--) |  |
### SynchronizeOptions() {#SynchronizeOptions--}
```
public SynchronizeOptions()
```


SynchronizeOptions クラスの新しいインスタンスを初期化します。


### SynchronizeOptions(Object data) {#SynchronizeOptions-java.lang.Object-}
```
public SynchronizeOptions(Object data)
```


SynchronizeOptions クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | データ | java.lang.Object | シリアライズされたデータ。 |
|

### isAsync() {#isAsync--}
```
public boolean isAsync()
```


操作を非同期で実行するフラグを取得します。デフォルト値は false です。


**Returns:**
boolean - 操作を非同期で実行するフラグ。

### setAsync(boolean value) {#setAsync-boolean-}
```
public void setAsync(boolean value)
```


操作を非同期で実行するフラグを設定します。デフォルト値は false です。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 値 | boolean | 操作を非同期で実行するフラグ。 |
|

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
