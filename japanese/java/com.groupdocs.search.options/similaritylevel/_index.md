---
title: "SimilarityLevel"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "類似検索のアルゴリズムで、類似度レベルを指定します。"
type: docs
weight: 35
url: /ja/java/com.groupdocs.search.options/similaritylevel/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.options.FuzzyAlgorithm](../../com.groupdocs.search.options/fuzzyalgorithm)
```
public class SimilarityLevel extends FuzzyAlgorithm
```

あいまい検索のアルゴリズムで、類似度レベルを指定します。類似度レベルのアルゴリズムは、単語の長さに反比例して単語の最大誤り数を計算します。


**Learn more**

* [Fuzzy search](../https://docs.groupdocs.com/display/searchjava/Fuzzy+search)


この例はクラスの典型的な使用方法を示しています。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // 指定されたフォルダーにインデックスを作成しています
index.add(documentsFolder); // 指定されたフォルダーからドキュメントをインデックス化しています
SearchOptions options = new SearchOptions();
options.getFuzzySearch().setEnabled(true); // ファジー検索を有効にしています
options.getFuzzySearch().setFuzzyAlgorithm(new SimilarityLevel(0.8)); // あいまい検索アルゴリズムを作成
// この関数は、1〜4文字の単語に対する最大誤り数を 0 に指定します。
// 5〜9文字の単語に対する最大誤り数を 1 に指定します。
// 10〜14文字の単語に対する最大誤り数を 2 に指定します。以降同様です。
SearchResult result = index.search(query, options); // インデックス内を検索
 
```
 
````


## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [SimilarityLevel(double value)](#SimilarityLevel-double-) | SimilarityLevel クラスの新しいインスタンスを初期化します。 |
|
|  | [SimilarityLevel(Object data)](#SimilarityLevel-java.lang.Object-) | SimilarityLevel クラスの新しいインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getSimilarityLevel(int termLength)](#getSimilarityLevel-int-) | 指定された語長に対する類似度レベルの値を取得します。 |
|
|  | [getMaxMistakeCount(int termLength)](#getMaxMistakeCount-int-) | 指定された語長に対する許容最大誤り数を取得します。 |
|
### SimilarityLevel(double value) {#SimilarityLevel-double-}
```
public SimilarityLevel(double value)
```


SimilarityLevel クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 値 | double | 類似度レベルの値。 |
|

### SimilarityLevel(Object data) {#SimilarityLevel-java.lang.Object-}
```
public SimilarityLevel(Object data)
```


SimilarityLevel クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | データ | java.lang.Object | シリアライズされたデータ。 |
|

### getSimilarityLevel(int termLength) {#getSimilarityLevel-int-}
```
public double getSimilarityLevel(int termLength)
```


指定された語長に対する類似度レベルの値を取得します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | termLength | int | 期間の長さ。 |
|

**Returns:**
double - 類似度レベルの値。

### getMaxMistakeCount(int termLength) {#getMaxMistakeCount-int-}
```
public int getMaxMistakeCount(int termLength)
```


指定された語長に対する許容最大誤り数を取得します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | termLength | int | 期間の長さ。 |
|

**Returns:**
int - 許容される最大誤り数。

