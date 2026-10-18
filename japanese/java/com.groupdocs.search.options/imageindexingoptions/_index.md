---
title: "ImageIndexingOptions"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "逆画像検索の画像インデックスオプションを提供します。"
type: docs
weight: 23
url: /ja/java/com.groupdocs.search.options/imageindexingoptions/
---
**Inheritance:**
java.lang.Object
```
public abstract class ImageIndexingOptions
```

逆画像検索の画像インデックスオプションを提供します。

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [ImageIndexingOptions()](#ImageIndexingOptions--) |  |
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getEnabledForSeparateImages()](#getEnabledForSeparateImages--) | 個別の画像ファイルをインデックス付けするかどうかを示す値を取得します。 |
|
|  | [setEnabledForSeparateImages(boolean value)](#setEnabledForSeparateImages-boolean-) | 個別の画像ファイルをインデックス付けするかどうかを示す値を設定します。 |
|
|  | [getEnabledForContainerItemImages()](#getEnabledForContainerItemImages--) | コンテナ内の項目である画像（例: ZIP アーカイブ内の画像）をインデックス付けするかどうかを示す値を取得します。 |
|
|  | [setEnabledForContainerItemImages(boolean value)](#setEnabledForContainerItemImages-boolean-) | コンテナ内の項目である画像（例: ZIP アーカイブ内の画像）をインデックス付けするかどうかを示す値を設定します。 |
|
|  | [getEnabledForEmbeddedImages()](#getEnabledForEmbeddedImages--) | 埋め込み画像（例: DOCX ドキュメント内の画像）をインデックス付けするかどうかを示す値を取得します。 |
|
|  | [setEnabledForEmbeddedImages(boolean value)](#setEnabledForEmbeddedImages-boolean-) | 埋め込み画像（例: DOCX ドキュメント内の画像）をインデックス付けするかどうかを示す値を設定します。 |
|
### ImageIndexingOptions() {#ImageIndexingOptions--}
```
public ImageIndexingOptions()
```


### getEnabledForSeparateImages() {#getEnabledForSeparateImages--}
```
public abstract boolean getEnabledForSeparateImages()
```


個別の画像ファイルをインデックス付けするかどうかを示す値を取得します。デフォルト値は false です。


**Returns:**
boolean - 個別の画像ファイルをインデックス付けするかどうかを示す値。

### setEnabledForSeparateImages(boolean value) {#setEnabledForSeparateImages-boolean-}
```
public abstract void setEnabledForSeparateImages(boolean value)
```


個別の画像ファイルをインデックス付けするかどうかを示す値を設定します。デフォルト値は false です。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 値 | boolean | 個別の画像ファイルをインデックス付けするかどうかを示す値。 |
|

### getEnabledForContainerItemImages() {#getEnabledForContainerItemImages--}
```
public abstract boolean getEnabledForContainerItemImages()
```


コンテナ内の項目である画像（例: ZIP アーカイブ内の画像）をインデックス付けするかどうかを示す値を取得します。デフォルト値は false です。


**Returns:**
boolean - コンテナ内の項目である画像をインデックス付けするかどうかを示す値。

### setEnabledForContainerItemImages(boolean value) {#setEnabledForContainerItemImages-boolean-}
```
public abstract void setEnabledForContainerItemImages(boolean value)
```


コンテナ内の項目である画像（例: ZIP アーカイブ内の画像）をインデックス付けするかどうかを示す値を設定します。デフォルト値は false です。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 値 | boolean | コンテナ内の項目である画像をインデックス付けするかどうかを示す値。 |
|

### getEnabledForEmbeddedImages() {#getEnabledForEmbeddedImages--}
```
public abstract boolean getEnabledForEmbeddedImages()
```


埋め込み画像（例: DOCX ドキュメント内の画像）をインデックス付けするかどうかを示す値を取得します。デフォルト値は false です。


**Returns:**
boolean - 埋め込み画像をインデックス付けするかどうかを示す値。

### setEnabledForEmbeddedImages(boolean value) {#setEnabledForEmbeddedImages-boolean-}
```
public abstract void setEnabledForEmbeddedImages(boolean value)
```


埋め込み画像（例: DOCX ドキュメント内の画像）をインデックス付けするかどうかを示す値を設定します。デフォルト値は false です。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 値 | boolean | 埋め込み画像をインデックス付けするかどうかを示す値。 |
|

