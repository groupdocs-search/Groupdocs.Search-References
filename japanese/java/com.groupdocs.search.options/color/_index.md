---
title: "Color"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "ARGB（アルファ、赤、緑、青）カラーを表します。"
type: docs
weight: 11
url: /ja/java/com.groupdocs.search.options/color/
---
**Inheritance:**
java.lang.Object
```
public class Color
```

ARGB（アルファ、赤、緑、青）カラーを表します。

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [Color(int alpha, int red, int green, int blue)](#Color-int-int-int-int-) | Color クラスの新しいインスタンスを初期化します。 |
|
|  | [Color(int red, int green, int blue)](#Color-int-int-int-) | Color クラスの新しいインスタンスを初期化します。 |
|
|  | [Color(Object data)](#Color-java.lang.Object-) | Color クラスの新しいインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getAlpha()](#getAlpha--) | このインスタンスのアルファコンポーネント値を取得します。 |
|
|  | [getRed()](#getRed--) | このインスタンスの赤コンポーネント値を取得します。 |
|
|  | [getGreen()](#getGreen--) | このインスタンスの緑コンポーネント値を取得します。 |
|
|  | [getBlue()](#getBlue--) | このインスタンスの青コンポーネント値を取得します。 |
|
|  | [toString()](#toString--) | 現在の Color を表す String を返します。 |
|
| [getCore()](#getCore--) |  |
### Color(int alpha, int red, int green, int blue) {#Color-int-int-int-int-}
```
public Color(int alpha, int red, int green, int blue)
```


Color クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | alpha | int | 0 から 255 までのアルファコンポーネントです。 |
|
|  | red | int | 0 から 255 までの赤成分です。 |
|
|  | 緑 | int | 0 から 255 までの緑成分です。 |
|
|  | 青 | int | 0 から 255 までの青成分です。 |
|

### Color(int red, int green, int blue) {#Color-int-int-int-}
```
public Color(int red, int green, int blue)
```


Color クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | red | int | 0 から 255 までの赤成分です。 |
|
|  | 緑 | int | 0 から 255 までの緑成分です。 |
|
|  | 青 | int | 0 から 255 までの青成分です。 |
|

### Color(Object data) {#Color-java.lang.Object-}
```
public Color(Object data)
```


Color クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | データ | java.lang.Object | シリアライズされたデータ。 |
|

### getAlpha() {#getAlpha--}
```
public int getAlpha()
```


このインスタンスのアルファコンポーネント値を取得します。


**Returns:**
int - このインスタンスのアルファ成分の値です。

### getRed() {#getRed--}
```
public int getRed()
```


このインスタンスの赤コンポーネント値を取得します。


**Returns:**
int - このインスタンスの赤成分の値です。

### getGreen() {#getGreen--}
```
public int getGreen()
```


このインスタンスの緑コンポーネント値を取得します。


**Returns:**
int - このインスタンスの緑成分の値です。

### getBlue() {#getBlue--}
```
public int getBlue()
```


このインスタンスの青コンポーネント値を取得します。


**Returns:**
int - このインスタンスの青成分の値です。

### toString() {#toString--}
```
public String toString()
```


現在の Color を表す String を返します。


**Returns:**
java.lang.String - 現在の Color を表す文字列です。

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
