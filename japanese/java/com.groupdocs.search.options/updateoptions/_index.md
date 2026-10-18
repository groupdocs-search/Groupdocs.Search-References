---
title: "UpdateOptions"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "更新操作のオプションを提供します。"
type: docs
weight: 43
url: /ja/java/com.groupdocs.search.options/updateoptions/
---
**Inheritance:**
java.lang.Object
```
public class UpdateOptions
```

更新操作のオプションを提供します。


**Learn more**

* [Update index](../https://docs.groupdocs.com/display/searchjava/Update+index)
* [Delete indexed paths](../https://docs.groupdocs.com/display/searchjava/Delete+indexed+paths)

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [UpdateOptions()](#UpdateOptions--) | UpdateOptions クラスの新しいインスタンスを初期化します。 |
|
|  | [UpdateOptions(Object data)](#UpdateOptions-java.lang.Object-) | UpdateOptions クラスの新しいインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getThreads()](#getThreads--) | インデックス作成に使用されるスレッド数を取得します。 |
|
|  | [setThreads(int value)](#setThreads-int-) | インデックス作成に使用されるスレッド数を設定します。 |
|
|  | [isAsync()](#isAsync--) | 操作を非同期で実行するフラグを取得します。 |
|
|  | [setAsync(boolean value)](#setAsync-boolean-) | 操作を非同期で実行するフラグを設定します。 |
|
|  | [getCancellation()](#getCancellation--) | 操作のキャンセルオブジェクトを取得します。 |
|
|  | [setCancellation(Cancellation value)](#setCancellation-com.groupdocs.search.common.Cancellation-) | 操作のキャンセルオブジェクトを設定します。 |
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
### UpdateOptions() {#UpdateOptions--}
```
public UpdateOptions()
```


UpdateOptions クラスの新しいインスタンスを初期化します。


### UpdateOptions(Object data) {#UpdateOptions-java.lang.Object-}
```
public UpdateOptions(Object data)
```


UpdateOptions クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | データ | java.lang.Object | シリアライズされたデータ。 |
|

### getThreads() {#getThreads--}
```
public int getThreads()
```


インデックス作成に使用されるスレッド数を取得します。デフォルト値は 1 です。


**Returns:**
int - インデックス作成に使用されるスレッド数。

### setThreads(int value) {#setThreads-int-}
```
public void setThreads(int value)
```


インデックス作成に使用されるスレッド数を設定します。デフォルト値は 1 です。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 値 | int | インデックス作成に使用されるスレッド数。 |
|

### isAsync() {#isAsync--}
```
public boolean isAsync()
```


操作を非同期で実行するフラグを取得します。デフォルト値は false です。


**Returns:**
boolean - 操作を非同期で実行するフラグ。

### setAsync(boolean value) {#setAsync-boolean-}
```
public void setAsync(boolean value)
```


操作を非同期で実行するフラグを設定します。デフォルト値は false です。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 値 | boolean | 操作を非同期で実行するフラグ。 |
|

### getCancellation() {#getCancellation--}
```
public Cancellation getCancellation()
```


操作のキャンセルオブジェクトを取得します。デフォルト値は null です。


**Returns:**
[Cancellation](../../com.groupdocs.search.common/cancellation) - The operation cancellation object.

### setCancellation(Cancellation value) {#setCancellation-com.groupdocs.search.common.Cancellation-}
```
public void setCancellation(Cancellation value)
```


操作のキャンセルオブジェクトを設定します。デフォルト値は null です。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | value | [Cancellation](../../com.groupdocs.search.common/cancellation) | 操作のキャンセルオブジェクト。 |
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
