---
title: "FileLogger"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "イベントとエラーをローカルファイルに記録するロガーを表します。"
type: docs
weight: 20
url: /ja/java/com.groupdocs.search.common/filelogger/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.search.common.ILogger](../../com.groupdocs.search.common/ilogger)
```
public class FileLogger implements ILogger
```

イベントとエラーをローカルファイルに記録するロガーを表します。


**Learn more**

* [Logging](../https://docs.groupdocs.com/display/searchjava/Logging)


この例はクラスの典型的な使用方法を示しています。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
String logPath = "c:\\Log.txt";
IndexSettings settings = new IndexSettings();
settings.setLogger(new FileLogger(logPath, 4.0)); // ログファイルのパスと最大長さ4 MB を指定
Index index = new Index(indexFolder, settings); // 指定されたフォルダーにインデックスを作成
index.add(documentsFolder); // 指定されたフォルダーからドキュメントをインデックス化しています
SearchResult result = index.search(query); // インデックス内を検索
 
```
 
````


## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [FileLogger(String filePath, double maxSize)](#FileLogger-java.lang.String-double-) | FileLogger クラスの新しいインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [error(String message)](#error-java.lang.String-) | インデックスで発生したエラーを記録します。 |
|
|  | [trace(String message)](#trace-java.lang.String-) | インデックスで発生したイベントを記録します。 |
|
|  | [getFilePath()](#getFilePath--) | ログファイルのパスを取得します。 |
|
|  | [getMaxSize()](#getMaxSize--) | ログファイルの最大サイズ（メガバイト）を取得します。 |
|
### FileLogger(String filePath, double maxSize) {#FileLogger-java.lang.String-double-}
```
public FileLogger(String filePath, double maxSize)
```


FileLogger クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | filePath | java.lang.String | ログファイルのパスです。 |
|
|  | maxSize | double | ログファイルの最大サイズ（メガバイト単位）。値は 0.1 から 1000 の範囲でなければなりません。 |
|

### error(String message) {#error-java.lang.String-}
```
public final void error(String message)
```


インデックスで発生したエラーを記録します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | メッセージ | java.lang.String | エラーメッセージ。 |
|

### trace(String message) {#trace-java.lang.String-}
```
public final void trace(String message)
```


インデックスで発生したイベントを記録します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | メッセージ | java.lang.String | イベントメッセージ。 |
|

### getFilePath() {#getFilePath--}
```
public final String getFilePath()
```


ログファイルのパスを取得します。


**Returns:**
java.lang.String - ログファイルのパス。

### getMaxSize() {#getMaxSize--}
```
public final double getMaxSize()
```


ログファイルの最大サイズ（メガバイト）を取得します。


**Returns:**
double - ログファイルの最大サイズ（メガバイト単位）。

