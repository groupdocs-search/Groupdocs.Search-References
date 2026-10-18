---
title: "FuzzyAlgorithm"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "ファジー検索アルゴリズムの基底クラスを表します。"
type: docs
weight: 20
url: /ja/java/com.groupdocs.search.options/fuzzyalgorithm/
---
**Inheritance:**
java.lang.Object
```
public abstract class FuzzyAlgorithm
```

ファジー検索アルゴリズムの基底クラスを表します。


**Learn more**

* [Fuzzy search](../https://docs.groupdocs.com/display/searchjava/Fuzzy+search)

## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getSimilarityLevel(int termLength)](#getSimilarityLevel-int-) | 指定された語句長さに対する類似度レベルを取得します。 |
|
|  | [getMaxMistakeCount(int termLength)](#getMaxMistakeCount-int-) | 指定された語長に対する許容最大誤り数を取得します。 |
|
| [getCore()](#getCore--) |  |
### getSimilarityLevel(int termLength) {#getSimilarityLevel-int-}
```
public abstract double getSimilarityLevel(int termLength)
```


指定された語句長さに対する類似度レベルを取得します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | termLength | int | 期間の長さ。 |
|

**Returns:**
double - 類似度レベルです。

### getMaxMistakeCount(int termLength) {#getMaxMistakeCount-int-}
```
public abstract int getMaxMistakeCount(int termLength)
```


指定された語長に対する許容最大誤り数を取得します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | termLength | int | 期間の長さ。 |
|

**Returns:**
int - 許容される最大誤り数。

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
