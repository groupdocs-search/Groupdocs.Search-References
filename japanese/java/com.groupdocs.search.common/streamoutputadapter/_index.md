---
title: "StreamOutputAdapter"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "java.io.OutputStream に出力を収集する出力アダプタを表します。"
type: docs
weight: 31
url: /ja/java/com.groupdocs.search.common/streamoutputadapter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.common.OutputAdapter](../../com.groupdocs.search.common/outputadapter)

**All Implemented Interfaces:**
[com.groupdocs.search.common.IStreamOutputAdapter](../../com.groupdocs.search.common/istreamoutputadapter)
```
public class StreamOutputAdapter extends OutputAdapter implements IStreamOutputAdapter
```

出力を java.io.OutputStream に収集する出力アダプタを表します。


**Learn more**

* [Output adapters](../https://docs.groupdocs.com/display/searchjava/Output+adapters)


この例はクラスの典型的な使用方法を示しています。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // 指定されたフォルダーにインデックスを作成しています
index.add(documentsFolder); // 指定されたフォルダーからドキュメントをインデックス化しています
DocumentInfo[] documents = index.getIndexedDocuments(); // インデックスされたドキュメントの情報を取得
final ByteArrayOutputStream stream = new ByteArrayOutputStream(); // 出力ストリームを作成
StreamOutputAdapter adapter = new StreamOutputAdapter(stream); // ストリーム出力アダプタを作成
index.getDocumentText(documents[0], adapter); // ドキュメントテキストをストリームに生成
 
```
 
````


## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [StreamOutputAdapter(OutputFormat outputFormat, OutputStream stream)](#StreamOutputAdapter-com.groupdocs.search.options.OutputFormat-java.io.OutputStream-) | StreamOutputAdapter クラスの新しいインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getStream()](#getStream--) | 出力ストリームを取得します。 |
|
### StreamOutputAdapter(OutputFormat outputFormat, OutputStream stream) {#StreamOutputAdapter-com.groupdocs.search.options.OutputFormat-java.io.OutputStream-}
```
public StreamOutputAdapter(OutputFormat outputFormat, OutputStream stream)
```


StreamOutputAdapter クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | outputFormat | [OutputFormat](../../com.groupdocs.search.options/outputformat) | 出力フォーマットです。 |
|
|  | stream | java.io.OutputStream | 出力ストリームです。 |
|

### getStream() {#getStream--}
```
public final OutputStream getStream()
```


出力ストリームを取得します。


**Returns:**
java.io.OutputStream - 出力ストリームです。

