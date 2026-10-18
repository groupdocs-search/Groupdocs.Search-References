---
title: "TableDiscreteFunction"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "単語長と許容ミス数の対応関係を含む曖昧検索アルゴリズムを表します。"
type: docs
weight: 40
url: /ja/java/com.groupdocs.search.options/tablediscretefunction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.options.FuzzyAlgorithm](../../com.groupdocs.search.options/fuzzyalgorithm)
```
public class TableDiscreteFunction extends FuzzyAlgorithm
```

単語の長さと許容ミス数の対応関係を含むファジー検索アルゴリズムを表します。このアルゴリズムは出力値のテーブルまたはステップ関数で指定できます。


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
options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(1, new Step(5, 2), new Step(8, 3))); // ファジー検索アルゴリズムを作成しています
// この関数は、1 文字から 4 文字の単語に対する最大ミス数を 1 と指定します。
// この関数は、5 文字から 7 文字の単語に対する最大ミス数を 2 と指定します。
// この関数は、8 文字以上の単語に対する最大ミス数を 3 と指定します。
SearchResult result = index.search(query, options); // インデックス内を検索
 
```
 
````


## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [TableDiscreteFunction(int offsetOfInputs, int[] tableOfOutputs)](#TableDiscreteFunction-int-int---) | TableDiscreteFunction クラスの新しいインスタンスを初期化します。 |
|
|  | [TableDiscreteFunction(int firstStepLevel, Step[] steps)](#TableDiscreteFunction-int-com.groupdocs.search.options.Step...-) | TableDiscreteFunction クラスの新しいインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getSimilarityLevel(int termLength)](#getSimilarityLevel-int-) | 指定された語長に対する類似度レベルを取得します。 |
|
|  | [getMaxMistakeCount(int termLength)](#getMaxMistakeCount-int-) | 指定された語長に対する許容最大ミス数を取得します。 |
|
### TableDiscreteFunction(int offsetOfInputs, int[] tableOfOutputs) {#TableDiscreteFunction-int-int---}
```
public TableDiscreteFunction(int offsetOfInputs, int[] tableOfOutputs)
```


TableDiscreteFunction クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | offsetOfInputs | int | 入力値に対するテーブルインデックスのオフセットです。 |
|
|  | tableOfOutputs | int[] | 出力値のテーブル。 |
|

### TableDiscreteFunction(int firstStepLevel, Step[] steps) {#TableDiscreteFunction-int-com.groupdocs.search.options.Step...-}
```
public TableDiscreteFunction(int firstStepLevel, Step[] steps)
```


TableDiscreteFunction クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | firstStepLevel | int | ステップ関数の最初のステップのレベル。 |
|
|  | steps | [Step\[\]](../../com.groupdocs.search.options/step) | ステップ関数の次のステップ。 |
|

### getSimilarityLevel(int termLength) {#getSimilarityLevel-int-}
```
public double getSimilarityLevel(int termLength)
```


指定された語長に対する類似度レベルを取得します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | termLength | int | 期間の長さ。 |
|

**Returns:**
double - 類似度レベル。

### getMaxMistakeCount(int termLength) {#getMaxMistakeCount-int-}
```
public int getMaxMistakeCount(int termLength)
```


指定された語長に対する許容最大ミス数を取得します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | termLength | int | 期間の長さ。 |
|

**Returns:**
int - 許容される最大ミス数。

