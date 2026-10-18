---
title: "OcrContext"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "OCR処理コンテキストを表します。"
type: docs
weight: 30
url: /ja/java/com.groupdocs.search.options/ocrcontext/
---
**Inheritance:**
java.lang.Object
```
public class OcrContext
```

OCR処理コンテキストを表します。

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [OcrContext(InputStream imageStream, ImageLocation imageLocation, String imageFileExtension)](#OcrContext-java.io.InputStream-com.groupdocs.search.options.ImageLocation-java.lang.String-) | 新しいインスタンスを初期化します |
OcrContext
クラス。
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getImageStream()](#getImageStream--) | 処理対象の画像を含むストリームを取得します。 |
|
|  | [getImageLocation()](#getImageLocation--) | 画像の場所を取得します。 |
|
|  | [getImageFileExtension()](#getImageFileExtension--) | 画像のファイル拡張子を取得します。 |
|
### OcrContext(InputStream imageStream, ImageLocation imageLocation, String imageFileExtension) {#OcrContext-java.io.InputStream-com.groupdocs.search.options.ImageLocation-java.lang.String-}
```
public OcrContext(InputStream imageStream, ImageLocation imageLocation, String imageFileExtension)
```


新しいインスタンスを初期化します
OcrContext
クラス。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | imageStream | java.io.InputStream | 処理対象の画像を含むストリームです。 |
|
|  | imageLocation | [ImageLocation](../../com.groupdocs.search.options/imagelocation) | 画像の場所です。 |
|
|  | imageFileExtension | java.lang.String | 画像のファイル拡張子です。 |
|

### getImageStream() {#getImageStream--}
```
public final InputStream getImageStream()
```


処理対象の画像を含むストリームを取得します。


**Returns:**
java.io.InputStream - 処理対象の画像を含むストリームです。

### getImageLocation() {#getImageLocation--}
```
public final ImageLocation getImageLocation()
```


画像の場所を取得します。


**Returns:**
[ImageLocation](../../com.groupdocs.search.options/imagelocation) - The location of the image.

### getImageFileExtension() {#getImageFileExtension--}
```
public final String getImageFileExtension()
```


画像のファイル拡張子を取得します。
この値は画像のタイプを判別するために使用できます。


**Returns:**
java.lang.String - 画像のファイル拡張子です。

