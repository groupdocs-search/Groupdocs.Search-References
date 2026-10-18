---
title: "IndexingReport"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "インデックス作成操作に関する詳細情報を表します。"
type: docs
weight: 25
url: /ja/java/com.groupdocs.search.common/indexingreport/
---
**Inheritance:**
java.lang.Object
```
public abstract class IndexingReport
```

インデックス作成操作に関する詳細情報を表します。


**Learn more**

* [Indexing reports](../https://docs.groupdocs.com/display/searchjava/Indexing+reports)


この例はクラスの典型的な使用方法を示しています。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder1 = "c:\\MyDocuments1\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
// 指定されたフォルダーにインデックスを作成しています
Index index = new Index(indexFolder);
// ドキュメントをインデックスしています
index.add(documentsFolder1);
index.add(documentsFolder2);
// インデックスレポートを取得
IndexingReport[] reports = index.getIndexingReports();
// コンソールにレポートを出力
for (IndexingReport report : reports) {
DateFormat df = new SimpleDateFormat("MM/dd/yyyy HH:mm:ss");
System.out.println("Time: " + df.format(report.getStartTime()));
System.out.println("Duration: " + report.getIndexingTime());
System.out.println("Documents total: " + report.getTotalDocumentsInIndex());
System.out.println("Terms total: " + report.getTotalTermCount());
System.out.println("Indexed documents size (MB): " + report.getIndexedDocumentsSize());
System.out.println("Index size (MB): " + (report.getTotalIndexSize() / 1024.0 / 1024.0));
System.out.println();
}
 
```
 
````


## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [IndexingReport()](#IndexingReport--) |  |
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getTotalDocumentsInIndex()](#getTotalDocumentsInIndex--) | インデックス内のドキュメント総数を取得します。 |
|
|  | [getTotalTermCount()](#getTotalTermCount--) | インデックス内の用語総数を取得します。 |
|
|  | [getIndexedDocumentsSize()](#getIndexedDocumentsSize--) | インデックスされたドキュメントの総長さ（MB）を取得します。 |
|
|  | [getSegmentCount()](#getSegmentCount--) | インデックスセグメントの数を取得します。 |
|
|  | [getTotalIndexSize()](#getTotalIndexSize--) | インデックスの総サイズ（バイト）を取得します。 |
|
|  | [getStartTime()](#getStartTime--) | インデックス作成開始時刻を取得します。 |
|
|  | [getEndTime()](#getEndTime--) | インデックス作成終了時刻を取得します。 |
|
|  | [getIndexingTime()](#getIndexingTime--) | インデックス作成の所要時間（秒）を取得します。 |
|
|  | [getErrors()](#getErrors--) | エラーの一覧を取得します。 |
|
|  | [getIndexedDocuments()](#getIndexedDocuments--) | インデックスされたドキュメントの一覧を取得します。 |
|
|  | [getUpdatedDocuments()](#getUpdatedDocuments--) | 更新されたドキュメントの一覧を取得します。 |
|
|  | [getRemovedDocuments()](#getRemovedDocuments--) | インデックスから削除されたドキュメントの一覧を取得します。 |
|
### IndexingReport() {#IndexingReport--}
```
public IndexingReport()
```


### getTotalDocumentsInIndex() {#getTotalDocumentsInIndex--}
```
public abstract int getTotalDocumentsInIndex()
```


インデックス内のドキュメント総数を取得します。


**Returns:**
int - インデックス内のドキュメント総数。

### getTotalTermCount() {#getTotalTermCount--}
```
public abstract int getTotalTermCount()
```


インデックス内の用語総数を取得します。


**Returns:**
int - インデックス内の用語総数。

### getIndexedDocumentsSize() {#getIndexedDocumentsSize--}
```
public abstract double getIndexedDocumentsSize()
```


インデックスされたドキュメントの総長さ（MB）を取得します。


**Returns:**
double - インデックスされたドキュメントの総長さ（MB）。

### getSegmentCount() {#getSegmentCount--}
```
public abstract int getSegmentCount()
```


インデックスセグメントの数を取得します。


**Returns:**
int - インデックスセグメントの数です。

### getTotalIndexSize() {#getTotalIndexSize--}
```
public abstract long getTotalIndexSize()
```


インデックスの総サイズ（バイト）を取得します。


**Returns:**
long - インデックスの総サイズ（バイト）。

### getStartTime() {#getStartTime--}
```
public abstract Date getStartTime()
```


インデックス作成開始時刻を取得します。


**Returns:**
java.util.Date - インデックス作成開始時刻。

### getEndTime() {#getEndTime--}
```
public abstract Date getEndTime()
```


インデックス作成終了時刻を取得します。


**Returns:**
java.util.Date - インデックス作成の終了時刻。

### getIndexingTime() {#getIndexingTime--}
```
public abstract double getIndexingTime()
```


インデックス作成の所要時間（秒）を取得します。


**Returns:**
double - インデックス作成の所要時間（秒）。

### getErrors() {#getErrors--}
```
public abstract String[] getErrors()
```


エラーの一覧を取得します。


**Returns:**
java.lang.String[] - エラーの一覧。

### getIndexedDocuments() {#getIndexedDocuments--}
```
public abstract String[] getIndexedDocuments()
```


インデックスされたドキュメントの一覧を取得します。


**Returns:**
java.lang.String[] - インデックス作成されたドキュメントの一覧。

### getUpdatedDocuments() {#getUpdatedDocuments--}
```
public abstract String[] getUpdatedDocuments()
```


更新されたドキュメントの一覧を取得します。


**Returns:**
java.lang.String[] - 更新されたドキュメントの一覧。

### getRemovedDocuments() {#getRemovedDocuments--}
```
public abstract String[] getRemovedDocuments()
```


インデックスから削除されたドキュメントの一覧を取得します。


**Returns:**
java.lang.String[] - インデックスから削除されたドキュメントの一覧。

