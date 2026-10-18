---
title: "Metered"
second_title: "GroupDocs.Search 用 Java API Reference"
description: 
type: docs
weight: 11
url: /ja/java/com.groupdocs.search.licenses/metered/
---
**Inheritance:**
java.lang.Object
```
public class Metered
```
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [Metered()](#Metered--) | このクラスの新しいインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [setMeteredKey(String publicKey, String privateKey)](#setMeteredKey-java.lang.String-java.lang.String-) | Metered キーで製品を有効化します。 |
|
|  | [getConsumptionQuantity()](#getConsumptionQuantity--) | 処理された MB の量を取得します。 |
|
|  | [getConsumptionCredit()](#getConsumptionCredit--) | 消費されたクレジットの数を取得します。 |
|
| [increaseBytesCount(double length)](#increaseBytesCount-double-) |  |
| [increaseCreditsByBytesCount(double length)](#increaseCreditsByBytesCount-double-) |  |
| [increaseCreditsByOne()](#increaseCreditsByOne--) |  |
### Metered() {#Metered--}
```
public Metered()
```


このクラスの新しいインスタンスを初期化します。


### setMeteredKey(String publicKey, String privateKey) {#setMeteredKey-java.lang.String-java.lang.String-}
```
public final void setMeteredKey(String publicKey, String privateKey)
```


Metered キーで製品を有効化します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | publicKey | java.lang.String | 公開キー |
|
|  | privateKey | java.lang.String | プライベートキー |
|

### getConsumptionQuantity() {#getConsumptionQuantity--}
```
public static double getConsumptionQuantity()
```


処理された MB の量を取得します。


**Returns:**
double - 消費量

### getConsumptionCredit() {#getConsumptionCredit--}
```
public static double getConsumptionCredit()
```


消費されたクレジットの数を取得します。


**Returns:**
double - 消費クレジット

### increaseBytesCount(double length) {#increaseBytesCount-double-}
```
public static void increaseBytesCount(double length)
```




**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
| 長さ | double |  |

### increaseCreditsByBytesCount(double length) {#increaseCreditsByBytesCount-double-}
```
public static void increaseCreditsByBytesCount(double length)
```




**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
| 長さ | double |  |

### increaseCreditsByOne() {#increaseCreditsByOne--}
```
public static void increaseCreditsByOne()
```




