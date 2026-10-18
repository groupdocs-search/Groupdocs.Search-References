---
title: "SearchReport"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "検索操作に関する詳細情報を表します。"
type: docs
weight: 30
url: /ja/java/com.groupdocs.search.common/searchreport/
---
**Inheritance:**
java.lang.Object
```
public abstract class SearchReport
```

検索操作に関する詳細情報を表します。


**Learn more**

* [Search reports](../https://docs.groupdocs.com/display/searchjava/Search+reports)


この例はクラスの典型的な使用方法を示しています。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// 指定されたフォルダーにインデックスを作成しています
Index index = new Index(indexFolder);
// 指定されたフォルダーからドキュメントをインデックス化
index.add(documentsFolder);
// インデックスを検索しています
SearchResult result1 = index.search("Einstein");
SearchResult result2 = index.search("\"Theory of Relativity\"");
// 検索レポートを取得しています
SearchReport[] reports = index.getSearchReports();
// コンソールにレポートを出力
for (SearchReport report : reports) {
System.out.println("Query: " + report.getTextQuery());
DateFormat df = new SimpleDateFormat("MM/dd/yyyy HH:mm:ss");
System.out.println("Time: " + df.format(report.getStartTime()));
System.out.println("Duration: " + report.getSearchDuration());
System.out.println("Documents: " + report.getDocumentCount());
System.out.println("Occurrences: " + report.getOccurrenceCount());
System.out.println();
}
 
```
 
````


## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [SearchReport()](#SearchReport--) |  |
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getStartTime()](#getStartTime--) | 検索の開始時刻を取得します。 |
|
|  | [getEndTime()](#getEndTime--) | 検索の終了時刻を取得します。 |
|
|  | [getSearchDuration()](#getSearchDuration--) | 検索の所要時間（秒）を取得します。 |
|
|  | [getDocumentCount()](#getDocumentCount--) | 見つかったドキュメント数を取得します。 |
|
|  | [getOccurrenceCount()](#getOccurrenceCount--) | 見つかった総出現回数を取得します。 |
|
|  | [getTextQuery()](#getTextQuery--) | テキスト形式の検索クエリを取得します。 |
|
|  | [getObjectQuery()](#getObjectQuery--) | オブジェクト形式の検索クエリを取得します。 |
|
|  | [getSearchOptions()](#getSearchOptions--) | 検索オプションを取得します。 |
|
|  | [toString()](#toString--) | 現在の SearchReport を表す文字列を返します。 |
|
### SearchReport() {#SearchReport--}
```
public SearchReport()
```


### getStartTime() {#getStartTime--}
```
public abstract Date getStartTime()
```


検索の開始時刻を取得します。


**Returns:**
java.util.Date - 検索の開始時刻。

### getEndTime() {#getEndTime--}
```
public abstract Date getEndTime()
```


検索の終了時刻を取得します。


**Returns:**
java.util.Date - 検索の終了時刻。

### getSearchDuration() {#getSearchDuration--}
```
public abstract double getSearchDuration()
```


検索の所要時間（秒）を取得します。


**Returns:**
double - 検索の所要時間（秒）。

### getDocumentCount() {#getDocumentCount--}
```
public abstract int getDocumentCount()
```


見つかったドキュメント数を取得します。


**Returns:**
int - 見つかったドキュメント数。

### getOccurrenceCount() {#getOccurrenceCount--}
```
public abstract int getOccurrenceCount()
```


見つかった総出現回数を取得します。


**Returns:**
int - 見つかった総出現回数。

### getTextQuery() {#getTextQuery--}
```
public abstract String getTextQuery()
```


テキスト形式の検索クエリを取得します。


**Returns:**
java.lang.String - テキスト形式の検索クエリ。

### getObjectQuery() {#getObjectQuery--}
```
public abstract SearchQuery getObjectQuery()
```


オブジェクト形式の検索クエリを取得します。


**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - The search query in object form.

### getSearchOptions() {#getSearchOptions--}
```
public abstract SearchOptions getSearchOptions()
```


検索オプションを取得します。


**Returns:**
[SearchOptions](../../com.groupdocs.search.options/searchoptions) - The search options.

### toString() {#toString--}
```
public abstract String toString()
```


現在の SearchReport を表す文字列を返します。


**Returns:**
java.lang.String - 現在の SearchReport を表す文字列。

