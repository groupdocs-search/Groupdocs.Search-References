---
title: "Extractor"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "後続の高速インデックス作成段階を分離するために、ドキュメントからの事前データ抽出ツールを表します。"
type: docs
weight: 16
url: /ja/java/com.groupdocs.search/extractor/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventHubBase](../../com.groupdocs.search.events/eventhubbase)
```
public class Extractor extends EventHubBase
```

後続の高速インデックス作成段階を分離するために、ドキュメントからの事前データ抽出ツールを表します。

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [Extractor()](#Extractor--) | Extractor クラスの新しいインスタンスを初期化します。 |
|
## Fields

| Field | 説明 |
| --- | --- |
|  | [ErrorOccurred](#ErrorOccurred) | extractor 操作中にエラーが発生したときに発生します。 |
|
|  | [ImagePreparing](#ImagePreparing) | image がインデックス作成のために準備されるときに発生します。 |
|
|  | [PasswordRequired](#PasswordRequired) | document が開く際にパスワードが必要なときに発生します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getSettings()](#getSettings--) | extractor の設定を取得します。 |
|
|  | [extract(Document document, ExtractionOptions extractionOptions)](#extract-com.groupdocs.search.Document-com.groupdocs.search.options.ExtractionOptions-) | document からデータを抽出します。 |
|
| [raiseErrorOccurredPublic(String message, boolean isCritical)](#raiseErrorOccurredPublic-java.lang.String-boolean-) |  |
| [raiseImagePreparingPublic(String documentKey, String[] innerPath, int imageIndex, ImageFrame[] frames, InputStream stream)](#raiseImagePreparingPublic-java.lang.String-java.lang.String---int-com.groupdocs.search.common.ImageFrame---java.io.InputStream-) |  |
| [raisePasswordRequiredPublic(String filePath)](#raisePasswordRequiredPublic-java.lang.String-) |  |
### Extractor() {#Extractor--}
```
public Extractor()
```


Extractor クラスの新しいインスタンスを初期化します。


### ErrorOccurred {#ErrorOccurred}
```
public final Event<EventHandler<IndexErrorEventArgs>> ErrorOccurred
```


extractor 操作中にエラーが発生したときに発生します。


### ImagePreparing {#ImagePreparing}
```
public final Event<EventHandler<ImagePreparingEventArgs>> ImagePreparing
```


image がインデックス作成のために準備されるときに発生します。


### PasswordRequired {#PasswordRequired}
```
public final Event<EventHandler<PasswordRequiredEventArgs>> PasswordRequired
```


document が開く際にパスワードが必要なときに発生します。


### getSettings() {#getSettings--}
```
public final ExtractorSettings getSettings()
```


extractor の設定を取得します。


**Returns:**
[ExtractorSettings](../../com.groupdocs.search.common/extractorsettings) - The extractor settings.

### extract(Document document, ExtractionOptions extractionOptions) {#extract-com.groupdocs.search.Document-com.groupdocs.search.options.ExtractionOptions-}
```
public final ExtractedData extract(Document document, ExtractionOptions extractionOptions)
```


document からデータを抽出します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | document | [Document](../../com.groupdocs.search/document) | ファイルシステム、ストリーム、または構造からの document。 |
|
|  | extractionOptions | [ExtractionOptions](../../com.groupdocs.search.options/extractionoptions) | 抽出オプション。 |
|

**Returns:**
[ExtractedData](../../com.groupdocs.search/extracteddata) - The extracted data of the document.

### raiseErrorOccurredPublic(String message, boolean isCritical) {#raiseErrorOccurredPublic-java.lang.String-boolean-}
```
public final void raiseErrorOccurredPublic(String message, boolean isCritical)
```




**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
| メッセージ | java.lang.String |  |
| isCritical | boolean |  |

### raiseImagePreparingPublic(String documentKey, String[] innerPath, int imageIndex, ImageFrame[] frames, InputStream stream) {#raiseImagePreparingPublic-java.lang.String-java.lang.String---int-com.groupdocs.search.common.ImageFrame---java.io.InputStream-}
```
public final void raiseImagePreparingPublic(String documentKey, String[] innerPath, int imageIndex, ImageFrame[] frames, InputStream stream)
```




**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
| documentKey | java.lang.String |  |
| innerPath | java.lang.String[] |  |
| imageIndex | int |  |
| frames | [ImageFrame\[\]](../../com.groupdocs.search.common/imageframe) |  |
| stream | java.io.InputStream |  |

### raisePasswordRequiredPublic(String filePath) {#raisePasswordRequiredPublic-java.lang.String-}
```
public final String raisePasswordRequiredPublic(String filePath)
```




**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
| filePath | java.lang.String |  |

**Returns:**
java.lang.String
