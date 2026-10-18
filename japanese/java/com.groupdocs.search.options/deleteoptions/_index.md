---
title: "DeleteOptions"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "削除操作のオプションを提供します。"
type: docs
weight: 16
url: /ja/java/com.groupdocs.search.options/deleteoptions/
---
**Inheritance:**
java.lang.Object
```
public class DeleteOptions
```

削除操作のオプションを提供します。

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [DeleteOptions()](#DeleteOptions--) | DeleteOptions クラスの新しいインスタンスを初期化します。 |
|
|  | [DeleteOptions(Object data)](#DeleteOptions-java.lang.Object-) | DeleteOptions クラスの新しいインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [isAsync()](#isAsync--) | 操作を非同期で実行するフラグを取得します。 |
|
|  | [setAsync(boolean value)](#setAsync-boolean-) | 操作を非同期で実行するフラグを設定します。 |
|
| [getCore()](#getCore--) |  |
### DeleteOptions() {#DeleteOptions--}
```
public DeleteOptions()
```


DeleteOptions クラスの新しいインスタンスを初期化します。


### DeleteOptions(Object data) {#DeleteOptions-java.lang.Object-}
```
public DeleteOptions(Object data)
```


DeleteOptions クラスの新しいインスタンスを初期化します。


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
