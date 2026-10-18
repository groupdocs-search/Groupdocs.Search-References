---
title: "DocumentImage"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "ドキュメント画像データを表します。"
type: docs
weight: 16
url: /ja/java/com.groupdocs.search.common/documentimage/
---
**Inheritance:**
java.lang.Object
```
public abstract class DocumentImage
```

ドキュメント画像データを表します。

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [DocumentImage()](#DocumentImage--) |  |
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getImageIndex()](#getImageIndex--) | ドキュメント内の画像の順序番号を取得します。 |
|
|  | [getFields()](#getFields--) | 抽出されたフィールドを取得します。 |
|
|  | [getFrames()](#getFrames--) | 画像フレームを取得します。 |
|
### DocumentImage() {#DocumentImage--}
```
public DocumentImage()
```


### getImageIndex() {#getImageIndex--}
```
public abstract int getImageIndex()
```


ドキュメント内の画像の順序番号を取得します。


**Returns:**
int - ドキュメント内の画像の順序番号。

### getFields() {#getFields--}
```
public abstract DocumentField[] getFields()
```


抽出されたフィールドを取得します。


**Returns:**
com.groupdocs.search.common.DocumentField[] - 抽出されたフィールド。

### getFrames() {#getFrames--}
```
public abstract ImageFrame[] getFrames()
```


画像フレームを取得します。


**Returns:**
com.groupdocs.search.common.ImageFrame[] - 画像フレーム。

