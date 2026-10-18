---
title: "ExtractedData"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "ドキュメントから取得され、インデックス作成のために準備されたデータを表します。"
type: docs
weight: 15
url: /ja/java/com.groupdocs.search/extracteddata/
---
**Inheritance:**
java.lang.Object
```
public class ExtractedData
```

ドキュメントから取得され、インデックス作成のために準備されたデータを表します。

## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [serialize()](#serialize--) | 現在のインスタンスをバイト配列にシリアライズします。 |
|
|  | [deserialize(byte[] array)](#deserialize-byte---) | バイト配列からインスタンスをデシリアライズします。 |
|
### serialize() {#serialize--}
```
public final byte[] serialize()
```


現在のインスタンスをバイト配列にシリアライズします。


**Returns:**
byte[] - 現在のインスタンスを表すバイト配列です。

### deserialize(byte[] array) {#deserialize-byte---}
```
public static ExtractedData deserialize(byte[] array)
```


バイト配列からインスタンスをデシリアライズします。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 配列 | byte[] | デシリアライズ元のバイト配列です。 |
|

**Returns:**
[ExtractedData](../../com.groupdocs.search/extracteddata) - An instance deserialized from a byte array.

