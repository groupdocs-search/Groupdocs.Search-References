---
title: "SpellingCorrectorOptions"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "スペル補正機能のオプションを提供します。"
type: docs
weight: 36
url: /ja/java/com.groupdocs.search.options/spellingcorrectoroptions/
---
**Inheritance:**
java.lang.Object
```
public abstract class SpellingCorrectorOptions
```

スペル補正機能のオプションを提供します。


**Learn more**

* [Spell checking](../https://docs.groupdocs.com/display/searchjava/Spell+checking)
* [Search options](../https://docs.groupdocs.com/display/searchjava/Search+options)

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [SpellingCorrectorOptions()](#SpellingCorrectorOptions--) |  |
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getEnabled()](#getEnabled--) | スペリング補正機能が有効かどうかを示す値を取得します。 |
|
|  | [setEnabled(boolean value)](#setEnabled-boolean-) | スペリング補正機能が有効かどうかを示す値を設定します。 |
|
|  | [getMaxMistakeCount()](#getMaxMistakeCount--) | 最大ミス数を取得します。 |
|
|  | [setMaxMistakeCount(int value)](#setMaxMistakeCount-int-) | 最大ミス数を設定します。 |
|
|  | [getOnlyBestResults()](#getOnlyBestResults--) | 最良の結果のみが返されるかどうかを示す値を取得します。 |
|
|  | [setOnlyBestResults(boolean value)](#setOnlyBestResults-boolean-) | 最良の結果のみが返されるかどうかを示す値を設定します。 |
|
|  | [getOnlyBestResultsRange()](#getOnlyBestResultsRange--) | 見つかった最小ミス数を超える最大数を取得します。 |
|
|  | [setOnlyBestResultsRange(byte value)](#setOnlyBestResultsRange-byte-) | 見つかった最小ミス数を超える最大数を設定します。 |
|
|  | [getConsiderTranspositions()](#getConsiderTranspositions--) | アルゴリズムが隣接する2文字の転置を単一のミスとして考慮すべきかどうかを示す値を取得します。 |
|
|  | [setConsiderTranspositions(boolean value)](#setConsiderTranspositions-boolean-) | アルゴリズムが隣接する2文字の転置を単一のミスとして考慮すべきかどうかを示す値を設定します。 |
|
### SpellingCorrectorOptions() {#SpellingCorrectorOptions--}
```
public SpellingCorrectorOptions()
```


### getEnabled() {#getEnabled--}
```
public abstract boolean getEnabled()
```


スペリング補正機能が有効かどうかを示す値を取得します。デフォルト値は false です。


**Returns:**
boolean - スペリング補正機能が有効かどうかを示す値。

### setEnabled(boolean value) {#setEnabled-boolean-}
```
public abstract void setEnabled(boolean value)
```


スペリング補正機能が有効かどうかを示す値を設定します。デフォルト値は false です。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 値 | boolean | スペリング補正機能が有効かどうかを示す値。 |
|

### getMaxMistakeCount() {#getMaxMistakeCount--}
```
public abstract int getMaxMistakeCount()
```


最大ミス数を取得します。デフォルト値は 2 です。


**Returns:**
int - 最大ミス数。

### setMaxMistakeCount(int value) {#setMaxMistakeCount-int-}
```
public abstract void setMaxMistakeCount(int value)
```


最大ミス数を設定します。デフォルト値は 2 です。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 値 | int | 最大ミス数。 |
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


アルゴリズムが隣接する2文字の転置を単一のミスとして考慮すべきかを示す値を取得します。デフォルト値は true です。


**Returns:**
boolean - 転置を考慮する場合は true、そうでない場合は false。

### setConsiderTranspositions(boolean value) {#setConsiderTranspositions-boolean-}
```
public abstract void setConsiderTranspositions(boolean value)
```


アルゴリズムが隣接する2文字の転置を単一のミスとして考慮すべきかを示す値を設定します。デフォルト値は true です。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 値 | boolean | 転置を考慮する場合は true、そうでない場合は false。 |
|

