---
title: "TextOptions"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "インデックスから文書テキストを取得するオプションを提供します。"
type: docs
weight: 41
url: /ja/java/com.groupdocs.search.options/textoptions/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.search.options.ITextOptions](../../com.groupdocs.search.options/itextoptions)
```
public class TextOptions implements ITextOptions
```

インデックスから文書テキストを取得するオプションを提供します。


**Learn more**

* [Getting indexed documents](../https://docs.groupdocs.com/display/searchjava/Getting+indexed+documents)
* [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [TextOptions()](#TextOptions--) | TextOptions クラスの新しいインスタンスを初期化します。 |
|
|  | [TextOptions(Object data)](#TextOptions-java.lang.Object-) | TextOptions クラスの新しいインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getCustomExtractor()](#getCustomExtractor--) | インデックス作成に使用されたカスタムテキスト抽出器を取得します。 |
|
|  | [setCustomExtractor(IFieldExtractor value)](#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-) | インデックス作成に使用されたカスタムテキスト抽出器を設定します。 |
|
|  | [getAdditionalFields()](#getAdditionalFields--) | インデックス作成に使用された追加のドキュメントフィールドを取得します。 |
|
|  | [setAdditionalFields(DocumentField[] value)](#setAdditionalFields-com.groupdocs.search.common.DocumentField---) | インデックス作成に使用された追加のドキュメントフィールドを設定します。 |
|
|  | [getCancellation()](#getCancellation--) | キャンセルオブジェクトを取得します。 |
|
|  | [setCancellation(Cancellation value)](#setCancellation-com.groupdocs.search.common.Cancellation-) | キャンセルオブジェクトを設定します。 |
|
|  | [getGenerateHead()](#getGenerateHead--) | 出力HTMLに Head タグが生成されるかどうかを示す値を取得します。 |
|
|  | [setGenerateHead(boolean value)](#setGenerateHead-boolean-) | 出力HTMLに Head タグが生成されるかどうかを示す値を設定します。 |
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
### TextOptions() {#TextOptions--}
```
public TextOptions()
```


TextOptions クラスの新しいインスタンスを初期化します。


### TextOptions(Object data) {#TextOptions-java.lang.Object-}
```
public TextOptions(Object data)
```


TextOptions クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | データ | java.lang.Object | シリアライズされたデータ。 |
|

### getCustomExtractor() {#getCustomExtractor--}
```
public IFieldExtractor getCustomExtractor()
```


インデックス作成に使用されたカスタムテキスト抽出器を取得します。デフォルト値は null です。なお、この値はドキュメントテキストがインデックスに保存されていない場合にのみ使用されます。


**Returns:**
[IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) - The custom text extractor that was used for indexing.

### setCustomExtractor(IFieldExtractor value) {#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-}
```
public void setCustomExtractor(IFieldExtractor value)
```


インデックス作成に使用されたカスタムテキスト抽出器を設定します。デフォルト値は null です。なお、この値はドキュメントテキストがインデックスに保存されていない場合にのみ使用されます。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | value | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | インデックス作成に使用されたカスタムテキスト抽出器です。 |
|

### getAdditionalFields() {#getAdditionalFields--}
```
public DocumentField[] getAdditionalFields()
```


インデックス作成に使用された追加のドキュメントフィールドを取得します。デフォルト値は null です。なお、この値はドキュメントテキストがインデックスに保存されていない場合にのみ使用されます。


**Returns:**
com.groupdocs.search.common.DocumentField[] - インデックス作成に使用された追加のドキュメントフィールドです。

### setAdditionalFields(DocumentField[] value) {#setAdditionalFields-com.groupdocs.search.common.DocumentField---}
```
public void setAdditionalFields(DocumentField[] value)
```


インデックス作成に使用された追加のドキュメントフィールドを設定します。デフォルト値は null です。なお、この値はドキュメントテキストがインデックスに保存されていない場合にのみ使用されます。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | value | [DocumentField\[\]](../../com.groupdocs.search.common/documentfield) | インデックス作成に使用された追加のドキュメントフィールドです。 |
|

### getCancellation() {#getCancellation--}
```
public Cancellation getCancellation()
```


キャンセルオブジェクトを取得します。デフォルト値は null です。


**Returns:**
[Cancellation](../../com.groupdocs.search.common/cancellation) - The cancellation object.

### setCancellation(Cancellation value) {#setCancellation-com.groupdocs.search.common.Cancellation-}
```
public void setCancellation(Cancellation value)
```


キャンセルオブジェクトを設定します。デフォルト値は null です。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | value | [Cancellation](../../com.groupdocs.search.common/cancellation) | キャンセルオブジェクト。 |
|

### getGenerateHead() {#getGenerateHead--}
```
public boolean getGenerateHead()
```


出力HTMLで Head タグが生成されるかどうかを示す値を取得します。デフォルト値は true です。


**Returns:**
boolean - 出力HTMLで Head タグが生成されるかどうかを示す値です。

### setGenerateHead(boolean value) {#setGenerateHead-boolean-}
```
public void setGenerateHead(boolean value)
```


出力HTMLで Head タグが生成されるかどうかを示す値を設定します。デフォルト値は true です。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 値 | boolean | 出力HTMLで Head タグが生成されるかどうかを示す値です。 |
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
