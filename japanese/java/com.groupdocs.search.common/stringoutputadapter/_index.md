---
title: "StringOutputAdapter"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "System.String として出力を収集する出力アダプタを表します。"
type: docs
weight: 32
url: /ja/java/com.groupdocs.search.common/stringoutputadapter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.common.OutputAdapter](../../com.groupdocs.search.common/outputadapter)

**All Implemented Interfaces:**
[com.groupdocs.search.common.IStringOutputAdapter](../../com.groupdocs.search.common/istringoutputadapter)
```
public class StringOutputAdapter extends OutputAdapter implements IStringOutputAdapter
```

出力を System.String として収集する出力アダプタを表します。


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
StringOutputAdapter adapter = new StringOutputAdapter(); // 文字列出力アダプタを作成
index.getDocumentText(documents[0], adapter); // アダプタにドキュメントテキストを生成
String result = adapter.getResult(); // 結果を取得
 
```
 
````


## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [StringOutputAdapter(OutputFormat outputFormat)](#StringOutputAdapter-com.groupdocs.search.options.OutputFormat-) | StringOutputAdapter クラスの新しいインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getResult()](#getResult--) | 結果の文字列を取得します。 |
|
### StringOutputAdapter(OutputFormat outputFormat) {#StringOutputAdapter-com.groupdocs.search.options.OutputFormat-}
```
public StringOutputAdapter(OutputFormat outputFormat)
```


StringOutputAdapter クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | outputFormat | [OutputFormat](../../com.groupdocs.search.options/outputformat) | 出力フォーマットです。 |
|

### getResult() {#getResult--}
```
public final String getResult()
```


結果の文字列を取得します。


**Returns:**
java.lang.String - 結果の文字列。

