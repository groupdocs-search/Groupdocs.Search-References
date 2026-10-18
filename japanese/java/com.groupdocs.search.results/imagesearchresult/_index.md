---
title: "ImageSearchResult"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "逆画像検索の結果を表します。"
type: docs
weight: 17
url: /ja/java/com.groupdocs.search.results/imagesearchresult/
---
**Inheritance:**
java.lang.Object
```
public abstract class ImageSearchResult
```

逆画像検索の結果を表します。

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [ImageSearchResult()](#ImageSearchResult--) |  |
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getImageCount()](#getImageCount--) | 見つかった画像の数を取得します。 |
|
|  | [getFoundImage(int index)](#getFoundImage-int-) | インデックスで取得した画像を取得します。 |
|
### ImageSearchResult() {#ImageSearchResult--}
```
public ImageSearchResult()
```


### getImageCount() {#getImageCount--}
```
public abstract int getImageCount()
```


見つかった画像の数を取得します。


**Returns:**
int - 見つかった画像の数。

### getFoundImage(int index) {#getFoundImage-int-}
```
public abstract FoundImageFrame getFoundImage(int index)
```


インデックスで取得した画像を取得します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | インデックス | int | 見つかった画像のインデックス。 |
|

**Returns:**
[FoundImageFrame](../../com.groupdocs.search.results/foundimageframe) - The found image.

