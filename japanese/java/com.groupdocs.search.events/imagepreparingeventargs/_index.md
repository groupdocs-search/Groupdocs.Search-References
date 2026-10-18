---
title: "ImagePreparingEventArgs"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "画像の準備開始イベントの引数を表します。"
type: docs
weight: 15
url: /ja/java/com.groupdocs.search.events/imagepreparingeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class ImagePreparingEventArgs extends BaseIndexEventArgs
```

画像の準備開始イベントの引数を表します。


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getDocumentKey()](#getDocumentKey--) | ドキュメントキーを取得します。 |
|
|  | [getInnerPath()](#getInnerPath--) | ネストされたドキュメントの内部パスを取得します。 |
|
|  | [getImageIndex()](#getImageIndex--) | ドキュメント内の画像の順序番号を取得します。 |
|
|  | [getImageFrames()](#getImageFrames--) | 画像フレームを取得します。 |
|
|  | [getImageStream()](#getImageStream--) | 画像ストリームを取得します。 |
|
### getDocumentKey() {#getDocumentKey--}
```
public final String getDocumentKey()
```


ドキュメントキーを取得します。


**Returns:**
java.lang.String - ドキュメントキー。

### getInnerPath() {#getInnerPath--}
```
public final String[] getInnerPath()
```


ネストされたドキュメントの内部パスを取得します。


**Returns:**
java.lang.String[] - ネストされたドキュメントの内部パス。

### getImageIndex() {#getImageIndex--}
```
public final int getImageIndex()
```


ドキュメント内の画像の順序番号を取得します。


**Returns:**
int - ドキュメント内の画像の順序番号。

### getImageFrames() {#getImageFrames--}
```
public final ImageFrame[] getImageFrames()
```


画像フレームを取得します。


**Returns:**
com.groupdocs.search.common.ImageFrame[] - 画像フレーム。

### getImageStream() {#getImageStream--}
```
public final InputStream getImageStream()
```


画像ストリームを取得します。


**Returns:**
java.io.InputStream - 画像ストリーム。

