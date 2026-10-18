---
title: "FileOutputAdapter"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "出力をファイルに収集する出力アダプターを表します。"
type: docs
weight: 21
url: /ja/java/com.groupdocs.search.common/fileoutputadapter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.common.OutputAdapter](../../com.groupdocs.search.common/outputadapter)

**All Implemented Interfaces:**
[com.groupdocs.search.common.IFileOutputAdapter](../../com.groupdocs.search.common/ifileoutputadapter)
```
public class FileOutputAdapter extends OutputAdapter implements IFileOutputAdapter
```

出力をファイルに収集する出力アダプターを表します。


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
FileOutputAdapter adapter = new FileOutputAdapter("c:\\DocumentText.htm"); // ファイル出力アダプタを作成しています
index.getDocumentText(documents[0], adapter); // 出力ファイルに文書テキストを生成しています
 
```
 
````


## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [FileOutputAdapter(OutputFormat outputFormat, String filePath)](#FileOutputAdapter-com.groupdocs.search.options.OutputFormat-java.lang.String-) | FileOutputAdapter クラスの新しいインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getFilePath()](#getFilePath--) | 出力ファイルパスを取得します。 |
|
### FileOutputAdapter(OutputFormat outputFormat, String filePath) {#FileOutputAdapter-com.groupdocs.search.options.OutputFormat-java.lang.String-}
```
public FileOutputAdapter(OutputFormat outputFormat, String filePath)
```


FileOutputAdapter クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | outputFormat | [OutputFormat](../../com.groupdocs.search.options/outputformat) | 出力フォーマットです。 |
|
|  | filePath | java.lang.String | 出力ファイルパスです。 |
|

### getFilePath() {#getFilePath--}
```
public final String getFilePath()
```


出力ファイルパスを取得します。


**Returns:**
java.lang.String - 出力ファイルパスです。

