---
title: "ExtractionOptions"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "文書からデータを抽出するオプションを提供します。"
type: docs
weight: 18
url: /ja/java/com.groupdocs.search.options/extractionoptions/
---
**Inheritance:**
java.lang.Object
```
public class ExtractionOptions
```

文書からデータを抽出するオプションを提供します。

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [ExtractionOptions()](#ExtractionOptions--) | ExtractionOptions クラスの新しいインスタンスを初期化します。 |
|
|  | [ExtractionOptions(Object data)](#ExtractionOptions-java.lang.Object-) | ExtractionOptions クラスの新しいインスタンスを初期化します。 |
|
|  | [ExtractionOptions(IndexingOptions options, IFieldExtractor customExtractor, IOcrConnector ocrConnector)](#ExtractionOptions-com.groupdocs.search.options.IndexingOptions-com.groupdocs.search.common.IFieldExtractor-com.groupdocs.search.options.IOcrConnector-) | ExtractionOptions クラスの新しいインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getCustomExtractor()](#getCustomExtractor--) | カスタムテキスト抽出機能を取得します。 |
|
|  | [setCustomExtractor(IFieldExtractor value)](#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-) | カスタムテキスト抽出機能を設定します。 |
|
|  | [getAutoDetectEncoding()](#getAutoDetectEncoding--) | エンコーディングを自動検出するかどうかを示す値を取得します。 |
|
|  | [setAutoDetectEncoding(boolean value)](#setAutoDetectEncoding-boolean-) | エンコーディングを自動検出するかどうかを示す値を設定します。 |
|
|  | [getEncoding()](#getEncoding--) | テキストドキュメントからテキストを抽出する際に使用されるエンコーディングを取得します。 |
|
|  | [setEncoding(String value)](#setEncoding-java.lang.String-) | テキストドキュメントからテキストを抽出する際に使用されるエンコーディングを設定します。 |
|
|  | [getUseRawTextExtraction()](#getUseRawTextExtraction--) | 可能な場合にテキスト抽出でローモードを使用するかどうかを示す値を取得します。 |
|
|  | [setUseRawTextExtraction(boolean value)](#setUseRawTextExtraction-boolean-) | 可能な場合にテキスト抽出でローモードを使用するかどうかを示す値を設定します。 |
|
|  | [getMetadataIndexingOptions()](#getMetadataIndexingOptions--) | メタデータフィールドのインデックス作成オプションを取得します。 |
|
|  | [getOcrIndexingOptions()](#getOcrIndexingOptions--) | OCR処理と認識テキストのインデックス作成オプションを取得します。 |
|
|  | [getImageIndexingOptions()](#getImageIndexingOptions--) | 逆画像検索のための画像インデックス作成オプションを取得します。 |
|
| [getCore()](#getCore--) |  |
### ExtractionOptions() {#ExtractionOptions--}
```
public ExtractionOptions()
```


ExtractionOptions クラスの新しいインスタンスを初期化します。


### ExtractionOptions(Object data) {#ExtractionOptions-java.lang.Object-}
```
public ExtractionOptions(Object data)
```


ExtractionOptions クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | データ | java.lang.Object | シリアライズされたデータ。 |
|

### ExtractionOptions(IndexingOptions options, IFieldExtractor customExtractor, IOcrConnector ocrConnector) {#ExtractionOptions-com.groupdocs.search.options.IndexingOptions-com.groupdocs.search.common.IFieldExtractor-com.groupdocs.search.options.IOcrConnector-}
```
public ExtractionOptions(IndexingOptions options, IFieldExtractor customExtractor, IOcrConnector ocrConnector)
```


ExtractionOptions クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | オプション。 |
|
|  | customExtractor | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | カスタム抽出器。 |
|
|  | ocrConnector | [IOcrConnector](../../com.groupdocs.search.options/iocrconnector) | OCRコネクタ。 |
|

### getCustomExtractor() {#getCustomExtractor--}
```
public IFieldExtractor getCustomExtractor()
```


カスタムテキスト抽出器を取得します。デフォルト値は null です。


**Returns:**
[IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) - The custom text extractor.

### setCustomExtractor(IFieldExtractor value) {#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-}
```
public void setCustomExtractor(IFieldExtractor value)
```


カスタムテキスト抽出器を設定します。デフォルト値は null です。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | value | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | カスタムテキスト抽出器。 |
|

### getAutoDetectEncoding() {#getAutoDetectEncoding--}
```
public boolean getAutoDetectEncoding()
```


エンコーディングを自動検出するかどうかを示す値を取得します。デフォルト値は false です。


**Returns:**
boolean - エンコーディングを自動検出するかどうかを示す値。

### setAutoDetectEncoding(boolean value) {#setAutoDetectEncoding-boolean-}
```
public void setAutoDetectEncoding(boolean value)
```


エンコーディングを自動検出するかどうかを示す値を設定します。デフォルト値は false です。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 値 | boolean | エンコーディングを自動検出するかどうかを示す値。 |
|

### getEncoding() {#getEncoding--}
```
public String getEncoding()
```


テキストドキュメントからテキストを抽出する際に使用されるエンコーディングを取得します。デフォルト値は null で、これはデフォルトエンコーディングの UTF-8 が使用されることを意味します。AutoDetectEncoding が true の場合、この値がデフォルトエンコーディングとして使用されます。


**Returns:**
java.lang.String - テキストドキュメントからテキストを抽出する際に使用されるエンコーディング。

### setEncoding(String value) {#setEncoding-java.lang.String-}
```
public void setEncoding(String value)
```


テキストドキュメントからテキストを抽出する際に使用されるエンコーディングを設定します。デフォルト値は null で、これはデフォルトエンコーディングの UTF-8 が使用されることを意味します。AutoDetectEncoding が true の場合、この値がデフォルトエンコーディングとして使用されます。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 値 | java.lang.String | テキストドキュメントからテキストを抽出する際に使用されるエンコーディング。 |
|

### getUseRawTextExtraction() {#getUseRawTextExtraction--}
```
public boolean getUseRawTextExtraction()
```


可能な場合にテキスト抽出で生モードが使用されるかどうかを示す値を取得します。デフォルト値は true です。生モードはインデックス作成速度を大幅に向上させますが、通常モードは抽出されたテキストの書式設定を改善します。


**Returns:**
boolean - 可能な場合にテキスト抽出で生モードが使用されるかどうかを示す値。

### setUseRawTextExtraction(boolean value) {#setUseRawTextExtraction-boolean-}
```
public void setUseRawTextExtraction(boolean value)
```


可能な場合にテキスト抽出で生モードが使用されるかどうかを示す値を設定します。デフォルト値は true です。生モードはインデックス作成速度を大幅に向上させますが、通常モードは抽出されたテキストの書式設定を改善します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 値 | boolean | 可能な場合にテキスト抽出で生モードが使用されるかどうかを示す値。 |
|

### getMetadataIndexingOptions() {#getMetadataIndexingOptions--}
```
public MetadataIndexingOptions getMetadataIndexingOptions()
```


メタデータフィールドのインデックス作成オプションを取得します。


**Returns:**
[MetadataIndexingOptions](../../com.groupdocs.search.options/metadataindexingoptions) - The options for indexing metadata fields.

### getOcrIndexingOptions() {#getOcrIndexingOptions--}
```
public OcrIndexingOptions getOcrIndexingOptions()
```


OCR処理と認識テキストのインデックス作成オプションを取得します。


**Returns:**
[OcrIndexingOptions](../../com.groupdocs.search.options/ocrindexingoptions) - The options for OCR processing and indexing recognized text.

### getImageIndexingOptions() {#getImageIndexingOptions--}
```
public ImageIndexingOptions getImageIndexingOptions()
```


逆画像検索のための画像インデックス作成オプションを取得します。


**Returns:**
[ImageIndexingOptions](../../com.groupdocs.search.options/imageindexingoptions) - The image indexing options for reverse image search.

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
