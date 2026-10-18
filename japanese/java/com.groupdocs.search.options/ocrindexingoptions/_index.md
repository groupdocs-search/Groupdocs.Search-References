---
title: "OcrIndexingOptions"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "OCR処理と認識テキストのインデックス作成のオプションを提供します。"
type: docs
weight: 31
url: /ja/java/com.groupdocs.search.options/ocrindexingoptions/
---
**Inheritance:**
java.lang.Object
```
public abstract class OcrIndexingOptions
```

OCR処理と認識テキストのインデックス作成のオプションを提供します。

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [OcrIndexingOptions()](#OcrIndexingOptions--) |  |
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getEnabledForSeparateImages()](#getEnabledForSeparateImages--) | 個別の画像ファイルでテキストを認識するかどうかを示す値を取得します。 |
|
|  | [setEnabledForSeparateImages(boolean value)](#setEnabledForSeparateImages-boolean-) | 個別の画像ファイルでテキストを認識するかどうかを示す値を設定します。 |
|
|  | [getEnabledForContainerItemImages()](#getEnabledForContainerItemImages--) | コンテナ内の項目である画像（例: ZIP アーカイブ内の画像）でテキストを認識するかどうかを示す値を取得します。 |
|
|  | [setEnabledForContainerItemImages(boolean value)](#setEnabledForContainerItemImages-boolean-) | コンテナ内の項目である画像（例: ZIP アーカイブ内の画像）でテキストを認識するかどうかを示す値を設定します。 |
|
|  | [getEnabledForEmbeddedImages()](#getEnabledForEmbeddedImages--) | 埋め込み画像（例: DOCX ドキュメント内の画像）でテキストを認識するかどうかを示す値を取得します。 |
|
|  | [setEnabledForEmbeddedImages(boolean value)](#setEnabledForEmbeddedImages-boolean-) | 埋め込み画像（例: DOCX ドキュメント内の画像）でテキストを認識するかどうかを示す値を設定します。 |
|
|  | [getOcrConnector()](#getOcrConnector--) | OCR 処理に使用される OCR コネクタを取得します。 |
|
|  | [setOcrConnector(IOcrConnector value)](#setOcrConnector-com.groupdocs.search.options.IOcrConnector-) | OCR 処理に使用される OCR コネクタを設定します。 |
|
### OcrIndexingOptions() {#OcrIndexingOptions--}
```
public OcrIndexingOptions()
```


### getEnabledForSeparateImages() {#getEnabledForSeparateImages--}
```
public abstract boolean getEnabledForSeparateImages()
```


個別の画像ファイルでテキストを認識するかどうかを示す値を取得します。デフォルト値は false です。


**Returns:**
boolean - 個別の画像ファイルでテキストを認識するかどうかを示す値です。

### setEnabledForSeparateImages(boolean value) {#setEnabledForSeparateImages-boolean-}
```
public abstract void setEnabledForSeparateImages(boolean value)
```


個別の画像ファイルでテキストを認識するかどうかを示す値を設定します。デフォルト値は false です。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 値 | boolean | 個別の画像ファイルでテキストを認識するかどうかを示す値です。 |
|

### getEnabledForContainerItemImages() {#getEnabledForContainerItemImages--}
```
public abstract boolean getEnabledForContainerItemImages()
```


コンテナ内の項目である画像（例: ZIP アーカイブ内の画像）でテキストを認識するかどうかを示す値を取得します。デフォルト値は false です。


**Returns:**
boolean - コンテナ内の項目である画像でテキストを認識するかどうかを示す値です。

### setEnabledForContainerItemImages(boolean value) {#setEnabledForContainerItemImages-boolean-}
```
public abstract void setEnabledForContainerItemImages(boolean value)
```


コンテナ内の項目である画像（例: ZIP アーカイブ内の画像）でテキストを認識するかどうかを示す値を設定します。デフォルト値は false です。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 値 | boolean | コンテナ内の項目である画像でテキストを認識するかどうかを示す値です。 |
|

### getEnabledForEmbeddedImages() {#getEnabledForEmbeddedImages--}
```
public abstract boolean getEnabledForEmbeddedImages()
```


埋め込み画像（例: DOCX ドキュメント内の画像）でテキストを認識するかどうかを示す値を取得します。デフォルト値は false です。


**Returns:**
boolean - 埋め込み画像でテキストを認識するかどうかを示す値です。

### setEnabledForEmbeddedImages(boolean value) {#setEnabledForEmbeddedImages-boolean-}
```
public abstract void setEnabledForEmbeddedImages(boolean value)
```


埋め込み画像（例: DOCX ドキュメント内の画像）でテキストを認識するかどうかを示す値を設定します。デフォルト値は false です。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 値 | boolean | 埋め込み画像でテキストを認識するかどうかを示す値です。 |
|

### getOcrConnector() {#getOcrConnector--}
```
public abstract IOcrConnector getOcrConnector()
```


OCR 処理に使用される OCR コネクタを取得します。デフォルト値は null で、OCR が使用されないことを意味します。


**Returns:**
[IOcrConnector](../../com.groupdocs.search.options/iocrconnector) - An OCR connector that is used for OCR processing.

### setOcrConnector(IOcrConnector value) {#setOcrConnector-com.groupdocs.search.options.IOcrConnector-}
```
public abstract void setOcrConnector(IOcrConnector value)
```


OCR 処理に使用される OCR コネクタを設定します。デフォルト値は null で、OCR が使用されないことを意味します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | value | [IOcrConnector](../../com.groupdocs.search.options/iocrconnector) | OCR 処理に使用される OCR コネクタです。 |
|

