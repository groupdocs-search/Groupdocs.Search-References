---
title: "Event"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "このクラスはイベントをサブスクライブする際に継承されることを意図しています。"
type: docs
weight: 11
url: /ja/java/com.groupdocs.search.events/event/
---
**Inheritance:**
java.lang.Object
```
public abstract class Event<T>
```

このクラスはイベントをサブスクライブする際に継承されることを意図しています。

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [Event()](#Event--) | Event クラスの新しいインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [add(T delegate)](#add-T-) | イベントのリスナーを追加します。 |
|
|  | [remove(T delegate)](#remove-T-) | イベントのリスナーを削除します。 |
|
|  | [isEmpty()](#isEmpty--) | 少なくとも1つのリスナーが存在するか確認します。 |
|
### Event() {#Event--}
```
public Event()
```


Event クラスの新しいインスタンスを初期化します。


### add(T delegate) {#add-T-}
```
public final synchronized void add(T delegate)
```


イベントのリスナーを追加します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | delegate | T | イベントを追加するリスナー。 |
|

### remove(T delegate) {#remove-T-}
```
public final synchronized void remove(T delegate)
```


イベントのリスナーを削除します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | delegate | T | イベントを削除するリスナー。 |
|

### isEmpty() {#isEmpty--}
```
public synchronized boolean isEmpty()
```


少なくとも1つのリスナーが存在するか確認します。


**Returns:**
boolean - イベントに少なくとも1つのリスナーが追加されたことを示す値。

