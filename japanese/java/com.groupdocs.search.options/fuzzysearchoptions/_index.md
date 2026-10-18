---
title: "FuzzySearchOptions"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "ファジー検索のオプションを提供します。"
type: docs
weight: 21
url: /ja/java/com.groupdocs.search.options/fuzzysearchoptions/
---
**Inheritance:**
java.lang.Object
```
public abstract class FuzzySearchOptions
```

ファジー検索のオプションを提供します。


**Learn more**

* [Fuzzy search](../https://docs.groupdocs.com/display/searchjava/Fuzzy+search)
* [Search options](../https://docs.groupdocs.com/display/searchjava/Search+options)

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [FuzzySearchOptions()](#FuzzySearchOptions--) |  |
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getEnabled()](#getEnabled--) | ファジー検索機能が有効かどうかを示す値を取得します。 |
|
|  | [setEnabled(boolean value)](#setEnabled-boolean-) | ファジー検索機能が有効かどうかを示す値を設定します。 |
|
|  | [getFuzzyAlgorithm()](#getFuzzyAlgorithm--) | ファジー検索アルゴリズムを取得します。 |
|
|  | [setFuzzyAlgorithm(FuzzyAlgorithm value)](#setFuzzyAlgorithm-com.groupdocs.search.options.FuzzyAlgorithm-) | ファジー検索アルゴリズムを設定します。 |
|
|  | [getOnlyBestResults()](#getOnlyBestResults--) | 最良の結果のみが返されるかどうかを示す値を取得します。 |
|
|  | [setOnlyBestResults(boolean value)](#setOnlyBestResults-boolean-) | 最良の結果のみが返されるかどうかを示す値を設定します。 |
|
|  | [getOnlyBestResultsRange()](#getOnlyBestResultsRange--) | 見つかった最小ミス数を超える最大数を取得します。 |
|
|  | [setOnlyBestResultsRange(byte value)](#setOnlyBestResultsRange-byte-) | 見つかった最小ミス数を超える最大数を設定します。 |
|
|  | [getConsiderTranspositions()](#getConsiderTranspositions--) | ファジー検索アルゴリズムが隣接する2文字の転置を単一のミスとして考慮すべきかどうかを示す値を取得します。 |
|
|  | [setConsiderTranspositions(boolean value)](#setConsiderTranspositions-boolean-) | ファジー検索アルゴリズムが隣接する2文字の転置を単一のミスとして考慮すべきかどうかを示す値を設定します。 |
|
### FuzzySearchOptions() {#FuzzySearchOptions--}
```
public FuzzySearchOptions()
```


### getEnabled() {#getEnabled--}
```
public abstract boolean getEnabled()
```


ファジー検索機能が有効かどうかを示す値を取得します。デフォルト値は false です。


**Returns:**
boolean - ファジー検索機能が有効かどうかを示す値。

### setEnabled(boolean value) {#setEnabled-boolean-}
```
public abstract void setEnabled(boolean value)
```


あいまい検索機能が有効かどうかを示す値を設定します。デフォルト値は false です。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 値 | boolean | あいまい検索機能が有効かどうかを示す値です。 |
|

### getFuzzyAlgorithm() {#getFuzzyAlgorithm--}
```
public abstract FuzzyAlgorithm getFuzzyAlgorithm()
```


あいまい検索アルゴリズムを取得します。現在利用可能なあいまい検索アルゴリズムは  SimilarityLevel  と  TableDiscreteFunction  です。デフォルト値は類似度レベルが  0.5 の  SimilarityLevel  のインスタンスです。


**Returns:**
[FuzzyAlgorithm](../../com.groupdocs.search.options/fuzzyalgorithm) - The fuzzy search algorithm.


この例はあいまい検索アルゴリズムの設定方法を示しています。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // 指定されたフォルダーにインデックスを作成しています
index.add(documentsFolder); // 指定されたフォルダーからドキュメントをインデックス化しています
SearchOptions options = new SearchOptions();
options.getFuzzySearch().setEnabled(true); // ファジー検索を有効にしています
options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(1, new Step(5, 2), new Step(8, 3))); // ファジー検索アルゴリズムを作成しています
// この関数は、1 文字から 4 文字の単語に対する最大ミス数を 1 と指定します。
// この関数は、5 文字から 7 文字の単語に対する最大ミス数を 2 と指定します。
// この関数は、8 文字以上の単語に対する最大ミス数を 3 と指定します。
SearchResult result = index.search(query, options); // インデックス内を検索
 
```
 
````


### setFuzzyAlgorithm(FuzzyAlgorithm value) {#setFuzzyAlgorithm-com.groupdocs.search.options.FuzzyAlgorithm-}
```
public abstract void setFuzzyAlgorithm(FuzzyAlgorithm value)
```


あいまい検索アルゴリズムを設定します。現在利用可能なあいまい検索アルゴリズムは  SimilarityLevel  と  TableDiscreteFunction  です。デフォルト値は類似度レベルが  0.5 の  SimilarityLevel  のインスタンスです。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | value | [FuzzyAlgorithm](../../com.groupdocs.search.options/fuzzyalgorithm) | あいまい検索アルゴリズムです。 |


この例はあいまい検索アルゴリズムの設定方法を示しています。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // 指定されたフォルダーにインデックスを作成しています
index.add(documentsFolder); // 指定されたフォルダーからドキュメントをインデックス化しています
SearchOptions options = new SearchOptions();
options.getFuzzySearch().setEnabled(true); // ファジー検索を有効にしています
options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(1, new Step(5, 2), new Step(8, 3))); // ファジー検索アルゴリズムを作成しています
// この関数は、1 文字から 4 文字の単語に対する最大ミス数を 1 と指定します。
// この関数は、5 文字から 7 文字の単語に対する最大ミス数を 2 と指定します。
// この関数は、8 文字以上の単語に対する最大ミス数を 3 と指定します。
SearchResult result = index.search(query, options); // インデックス内を検索
 
```
 
````

|

### getOnlyBestResults() {#getOnlyBestResults--}
```
public abstract boolean getOnlyBestResults()
```


最良の結果のみが返されるかどうかを示す値を取得します。デフォルト値は false です。


**Returns:**
boolean - 最良の結果のみが返される場合は true、そうでない場合は false。

### setOnlyBestResults(boolean value) {#setOnlyBestResults-boolean-}
```
public abstract void setOnlyBestResults(boolean value)
```


最良の結果のみが返されるかどうかを示す値を設定します。デフォルト値は false です。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 値 | boolean | 最良の結果のみが返される場合は true、そうでない場合は false。 |
|

### getOnlyBestResultsRange() {#getOnlyBestResultsRange--}
```
public abstract byte getOnlyBestResultsRange()
```


見つかった最小ミス数の最大超過を取得します。デフォルト値は 0 です。


**Returns:**
byte - 見つかった最小ミス数の最大超過。

### setOnlyBestResultsRange(byte value) {#setOnlyBestResultsRange-byte-}
```
public abstract void setOnlyBestResultsRange(byte value)
```


見つかった最小ミス数の最大超過を設定します。デフォルト値は 0 です。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 値 | byte | 見つかった最小ミス数の最大超過。 |
|

### getConsiderTranspositions() {#getConsiderTranspositions--}
```
public abstract boolean getConsiderTranspositions()
```


あいまい検索アルゴリズムが隣接する2文字の転置を単一のミスとして考慮すべきかどうかを示す値を取得します。デフォルト値は true です。


**Returns:**
boolean -  true  ならばあいまい検索アルゴリズムが転置を考慮します。そうでなければ  false です。

### setConsiderTranspositions(boolean value) {#setConsiderTranspositions-boolean-}
```
public abstract void setConsiderTranspositions(boolean value)
```


あいまい検索アルゴリズムが隣接する2文字の転置を単一のミスとして考慮すべきかどうかを示す値を設定します。デフォルト値は true です。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 値 | boolean | :  true  ならばあいまい検索アルゴリズムが転置を考慮します。そうでなければ  false です。 |
|

