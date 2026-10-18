---
title: "SearchImage"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "検索対象の画像を表します。"
type: docs
weight: 29
url: /ja/java/com.groupdocs.search.common/searchimage/
---
**Inheritance:**
java.lang.Object
```
public abstract class SearchImage
```

検索対象の画像を表します。

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [SearchImage()](#SearchImage--) |  |
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [create(String filePath)](#create-java.lang.String-) | 検索用にファイルから画像を作成します。 |
|
|  | [create(String filePath, int imageIndex)](#create-java.lang.String-int-) | 検索用にファイルから画像を作成します。 |
|
|  | [create(InputStream stream)](#create-java.io.InputStream-) | 検索用にストリームから画像を作成します。 |
|
|  | [create(InputStream stream, int imageIndex)](#create-java.io.InputStream-int-) | 検索用にストリームから画像を作成します。 |
|
### SearchImage() {#SearchImage--}
```
public SearchImage()
```


### create(String filePath) {#create-java.lang.String-}
```
public static SearchImage create(String filePath)
```


検索用にファイルから画像を作成します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | filePath | java.lang.String | 画像ファイルのパス。 |
|

**Returns:**
[SearchImage](../../com.groupdocs.search.common/searchimage) - An image to search.

### create(String filePath, int imageIndex) {#create-java.lang.String-int-}
```
public static SearchImage create(String filePath, int imageIndex)
```


検索用にファイルから画像を作成します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | filePath | java.lang.String | 画像ファイルのパス。 |
|
|  | imageIndex | int | マルチページ画像における画像インデックス。 |
|

**Returns:**
[SearchImage](../../com.groupdocs.search.common/searchimage) - An image to search.

### create(InputStream stream) {#create-java.io.InputStream-}
```
public static SearchImage create(InputStream stream)
```


検索用にストリームから画像を作成します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | stream | java.io.InputStream | 画像ストリーム。 |
|

**Returns:**
[SearchImage](../../com.groupdocs.search.common/searchimage) - An image to search.

### create(InputStream stream, int imageIndex) {#create-java.io.InputStream-int-}
```
public static SearchImage create(InputStream stream, int imageIndex)
```


検索用にストリームから画像を作成します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | stream | java.io.InputStream | 画像ストリーム。 |
|
|  | imageIndex | int | マルチページ画像における画像インデックス。 |
|

**Returns:**
[SearchImage](../../com.groupdocs.search.common/searchimage) - An image to search.

