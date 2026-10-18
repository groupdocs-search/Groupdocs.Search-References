---
title: "FoundImageFrame"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "見つかった画像フレームを表します。"
type: docs
weight: 16
url: /ja/java/com.groupdocs.search.results/foundimageframe/
---
**Inheritance:**
java.lang.Object
```
public abstract class FoundImageFrame
```

見つかった画像フレームを表します。

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [FoundImageFrame()](#FoundImageFrame--) |  |
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getDocumentInfo()](#getDocumentInfo--) | ドキュメント情報を取得します。 |
|
|  | [getImageIndex()](#getImageIndex--) | ドキュメント内の画像の順序番号を取得します。 |
|
|  | [getFrameIndex()](#getFrameIndex--) | 画像内のフレームのインデックスを取得します。 |
|
|  | [getHashDifferences()](#getHashDifferences--) | 画像ハッシュの不一致ビット数を取得します。 |
|
|  | [toString()](#toString--) | 現在の  FoundImageFrame を表す  System.String を返します。 |
|
### FoundImageFrame() {#FoundImageFrame--}
```
public FoundImageFrame()
```


### getDocumentInfo() {#getDocumentInfo--}
```
public abstract DocumentInfo getDocumentInfo()
```


ドキュメント情報を取得します。


**Returns:**
[DocumentInfo](../../com.groupdocs.search.results/documentinfo) - The document info.

### getImageIndex() {#getImageIndex--}
```
public abstract int getImageIndex()
```


ドキュメント内の画像の順序番号を取得します。


**Returns:**
int - ドキュメント内の画像の順序番号。

### getFrameIndex() {#getFrameIndex--}
```
public abstract int getFrameIndex()
```


画像内のフレームのインデックスを取得します。


**Returns:**
int - 画像内のフレームのインデックス。

### getHashDifferences() {#getHashDifferences--}
```
public abstract int getHashDifferences()
```


画像ハッシュの不一致ビット数を取得します。


**Returns:**
int - 画像ハッシュの不一致ビット数。

### toString() {#toString--}
```
public abstract String toString()
```


現在の  FoundImageFrame を表す  System.String を返します。


**Returns:**
java.lang.String - 現在の  FoundImageFrame を表す  System.String 。

