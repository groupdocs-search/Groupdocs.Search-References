---
title: "TextStorageSettings"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "テキスト保存設定を表します。"
type: docs
weight: 42
url: /ja/java/com.groupdocs.search.options/textstoragesettings/
---
**Inheritance:**
java.lang.Object
```
public class TextStorageSettings
```

テキスト保存設定を表します。


**Learn more**

* [Storing text of indexed documents](../https://docs.groupdocs.com/display/searchjava/Storing+text+of+indexed+documents)
* [Search index settings](../https://docs.groupdocs.com/display/searchjava/Search+index+settings)

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [TextStorageSettings(Compression compression)](#TextStorageSettings-com.groupdocs.search.options.Compression-) | TextStorageSettings クラスの新しいインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getCompression()](#getCompression--) | テキストストレージの圧縮設定を取得します。 |
|
|  | [setCompression(Compression value)](#setCompression-com.groupdocs.search.options.Compression-) | テキストストレージの圧縮設定を設定します。 |
|
### TextStorageSettings(Compression compression) {#TextStorageSettings-com.groupdocs.search.options.Compression-}
```
public TextStorageSettings(Compression compression)
```


TextStorageSettings クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | compression | [Compression](../../com.groupdocs.search.options/compression) | テキストストレージの圧縮設定です。 |
|

### getCompression() {#getCompression--}
```
public final Compression getCompression()
```


テキストストレージの圧縮設定を取得します。デフォルト値は Compression.Normal です。


**Returns:**
[Compression](../../com.groupdocs.search.options/compression) - The compression of text storage.

### setCompression(Compression value) {#setCompression-com.groupdocs.search.options.Compression-}
```
public final void setCompression(Compression value)
```


テキストストレージの圧縮設定を設定します。デフォルト値は Compression.Normal です。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | value | [Compression](../../com.groupdocs.search.options/compression) | テキストストレージの圧縮設定です。 |
|

