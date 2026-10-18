---
title: "キャンセル"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "操作のキャンセル要求用オブジェクトを表します。"
type: docs
weight: 11
url: /ja/java/com.groupdocs.search.common/cancellation/
---
**Inheritance:**
java.lang.Object
```
public class Cancellation
```

操作のキャンセル要求用オブジェクトを表します。


**Learn more**

* [Indexing options](../https://docs.groupdocs.com/display/searchjava/Indexing+options)
* [Search options](../https://docs.groupdocs.com/display/searchjava/Search+options)

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [Cancellation()](#Cancellation--) | 新しいインスタンスを初期化します |
キャンセル
クラス。
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [isCancelled()](#isCancelled--) | キャンセルが要求されたことを示す値を取得します。 |
|
|  | [cancel()](#cancel--) | キャンセルの要求を行います。 |
|
|  | [cancelAfter(int milliseconds)](#cancelAfter-int-) | 指定されたミリ秒数の期限が切れた後にキャンセルの要求を行います。 |
|
### Cancellation() {#Cancellation--}
```
public Cancellation()
```


新しいインスタンスを初期化します
キャンセル
クラス。


### isCancelled() {#isCancelled--}
```
public final boolean isCancelled()
```


キャンセルが要求されたことを示す値を取得します。


**Returns:**
boolean - キャンセルが要求されたことを示す値。

### cancel() {#cancel--}
```
public final void cancel()
```


キャンセルの要求を行います。


### cancelAfter(int milliseconds) {#cancelAfter-int-}
```
public final void cancelAfter(int milliseconds)
```


指定されたミリ秒数の期限が切れた後にキャンセルの要求を行います。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | ミリ秒 | int | 操作がキャンセルされるまでのミリ秒数。 |
|

