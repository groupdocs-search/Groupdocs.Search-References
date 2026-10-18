---
title: "SearchResult"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "検索クエリに一致する検索結果を表します。"
type: docs
weight: 19
url: /ja/java/com.groupdocs.search.results/searchresult/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public abstract class SearchResult implements Iterable<FoundDocument>
```

検索クエリに一致する検索結果を表します。


**Learn more**

* [Searching](../https://docs.groupdocs.com/display/searchjava/Searching)
* [Search results](../https://docs.groupdocs.com/display/searchjava/Search+results)


この例はクラスの典型的な使用方法を示しています。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentFolder = "c:\\MyDocuments\\";
// インデックスを作成
Index index = new Index(indexFolder);
// 指定されたフォルダーからドキュメントをインデックス化
index.add(documentFolder);
// 検索オプションの設定
SearchOptions options = new SearchOptions();
options.getFuzzySearch().setEnabled(true); // ファジー検索を有効にしています
options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(3)); // 最大差分数を3に設定
// 'Einstein' という単語または 'Theory of Relativity' というフレーズを含むドキュメントを検索
SearchResult result = index.search("Einstein OR \"Theory of Relativity\"", options);
// 結果の出力
System.out.println("ドキュメント: " + result.getDocumentCount());
System.out.println("総出現数: " + result.getOccurrenceCount());
for (int i = 0; i < result.getDocumentCount(); i++) {
FoundDocument document = result.getFoundDocument(i);
System.out.println("\tドキュメント: " + document.getDocumentInfo().getFilePath());
System.out.println("\t出現回数: " + document.getOccurrenceCount());
for (int j = 0; j < document.getFoundFields().length; j++) {
FoundDocumentField field = document.getFoundFields()[j];
System.out.println("\t\tフィールド: " + field.getFieldName());
System.out.println("\t\t出現回数: " + document.getOccurrenceCount());
// 見つかった用語の出力
if (field.getTerms() != null) {
for (int k = 0; k < field.getTerms().length; k++) {
System.out.println("\t\t\t" + field.getTerms()[k] + " - " + field.getTermsOccurrences()[k]);
}
}
// 見つかったフレーズの出力
if (field.getTermSequences() != null) {
for (int k = 0; k < field.getTermSequences().length; k++) {
String[] terms = field.getTermSequences()[k];
String sequence = "";
for (int m = 0; m < terms.length; m++) {
sequence += terms[m] + " ";
}
System.out.println("\t\t\t" + sequence + " - " + field.getTermSequencesOccurrences()[k]);
}
}
}
}
 
```
 
````


## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [SearchResult()](#SearchResult--) |  |
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getDocumentCount()](#getDocumentCount--) | 見つかったドキュメント数を取得します。 |
|
|  | [getOccurrenceCount()](#getOccurrenceCount--) | 見つかった総出現回数を取得します。 |
|
|  | [getTruncated()](#getTruncated--) | 結果が切り詰められていることを示す値を取得します。 |
|
|  | [getWarnings()](#getWarnings--) | 結果を説明する警告を取得します。 |
|
|  | [getNextChunkSearchToken()](#getNextChunkSearchToken--) | 次のチャンクを検索するためのチャンク検索トークンを取得します。 |
|
|  | [getStartTime()](#getStartTime--) | 検索の開始時刻を取得します。 |
|
|  | [getEndTime()](#getEndTime--) | 検索の終了時刻を取得します。 |
|
|  | [getSearchDuration()](#getSearchDuration--) | 検索の所要時間（秒）を取得します。 |
|
|  | [getFoundDocument(int index)](#getFoundDocument-int-) | インデックスで見つかったドキュメントを取得します。 |
|
|  | [iterator()](#iterator--) | 見つかったドキュメントのコレクションを反復処理するイテレータを返します。 |
|
### SearchResult() {#SearchResult--}
```
public SearchResult()
```


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

### getTruncated() {#getTruncated--}
```
public abstract boolean getTruncated()
```


結果が切り詰められていることを示す値を取得します。


**Returns:**
boolean - 結果が切り詰められていることを示す値。

### getWarnings() {#getWarnings--}
```
public abstract String getWarnings()
```


結果を説明する警告を取得します。


**Returns:**
java.lang.String - 結果を説明する警告。

### getNextChunkSearchToken() {#getNextChunkSearchToken--}
```
public abstract ChunkSearchToken getNextChunkSearchToken()
```


次のチャンクを検索するためのチャンク検索トークンを取得します。


**Returns:**
[ChunkSearchToken](../../com.groupdocs.search.common/chunksearchtoken) - A chunk search token for searching the next chunk.

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

### getFoundDocument(int index) {#getFoundDocument-int-}
```
public abstract FoundDocument getFoundDocument(int index)
```


インデックスで見つかったドキュメントを取得します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | インデックス | int | 見つかったドキュメントのインデックス。 |
|

**Returns:**
[FoundDocument](../../com.groupdocs.search.results/founddocument) - The found document.

### iterator() {#iterator--}
```
public abstract Iterator<FoundDocument> iterator()
```


見つかったドキュメントのコレクションを反復処理するイテレータを返します。


**Returns:**
java.util.Iterator<com.groupdocs.search.results.FoundDocument> - 見つかったドキュメントのコレクションを反復処理するために使用できるイテレータです。

