---
title: "SpellingCorrectorOptions"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "提供拼写校正器的选项。"
type: docs
weight: 36
url: /zh/java/com.groupdocs.search.options/spellingcorrectoroptions/
---
**Inheritance:**
java.lang.Object
```
public abstract class SpellingCorrectorOptions
```

提供拼写校正器的选项。


**Learn more**

* [Spell checking](../https://docs.groupdocs.com/display/searchjava/Spell+checking)
* [Search options](../https://docs.groupdocs.com/display/searchjava/Search+options)

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [SpellingCorrectorOptions()](#SpellingCorrectorOptions--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getEnabled()](#getEnabled--) | 获取指示拼写校正器是否已启用的值。 |
|
|  | [setEnabled(boolean value)](#setEnabled-boolean-) | 设置指示拼写校正器是否已启用的值。 |
|
|  | [getMaxMistakeCount()](#getMaxMistakeCount--) | 获取最大错误数。 |
|
|  | [setMaxMistakeCount(int value)](#setMaxMistakeCount-int-) | 设置最大错误数。 |
|
|  | [getOnlyBestResults()](#getOnlyBestResults--) | 获取指示是否仅返回最佳结果的值。 |
|
|  | [setOnlyBestResults(boolean value)](#setOnlyBestResults-boolean-) | 设置指示是否仅返回最佳结果的值。 |
|
|  | [getOnlyBestResultsRange()](#getOnlyBestResultsRange--) | 获取发现的最小错误数的最大超出值。 |
|
|  | [setOnlyBestResultsRange(byte value)](#setOnlyBestResultsRange-byte-) | 设置发现的最小错误数的最大超出值。 |
|
|  | [getConsiderTranspositions()](#getConsiderTranspositions--) | 获取指示算法是否必须将相邻两个字符的换位视为单个错误的值。 |
|
|  | [setConsiderTranspositions(boolean value)](#setConsiderTranspositions-boolean-) | 设置指示算法是否必须将相邻两个字符的换位视为单个错误的值。 |
|
### SpellingCorrectorOptions() {#SpellingCorrectorOptions--}
```
public SpellingCorrectorOptions()
```


### getEnabled() {#getEnabled--}
```
public abstract boolean getEnabled()
```


获取指示拼写校正器是否已启用的值。默认值为 false。


**Returns:**
boolean - 指示拼写校正器是否已启用的值。

### setEnabled(boolean value) {#setEnabled-boolean-}
```
public abstract void setEnabled(boolean value)
```


设置指示拼写校正器是否已启用的值。默认值为 false。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | boolean | 指示拼写校正器是否已启用的值。 |
|

### getMaxMistakeCount() {#getMaxMistakeCount--}
```
public abstract int getMaxMistakeCount()
```


获取最大错误数。默认值为 2。


**Returns:**
int - 最大错误数。

### setMaxMistakeCount(int value) {#setMaxMistakeCount-int-}
```
public abstract void setMaxMistakeCount(int value)
```


设置最大错误数。默认值为 2。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | int | 最大错误数。 |
|

### getOnlyBestResults() {#getOnlyBestResults--}
```
public abstract boolean getOnlyBestResults()
```


获取一个值，指示是否仅返回最佳结果。默认值为 false。


**Returns:**
boolean - true 如果仅返回最佳结果；否则 false。

### setOnlyBestResults(boolean value) {#setOnlyBestResults-boolean-}
```
public abstract void setOnlyBestResults(boolean value)
```


设置一个值，指示是否仅返回最佳结果。默认值为 false。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | boolean | true 如果仅返回最佳结果；否则 false。 |
|

### getOnlyBestResultsRange() {#getOnlyBestResultsRange--}
```
public abstract byte getOnlyBestResultsRange()
```


获取找到的最小错误数的最大超出值。默认值为 0。


**Returns:**
byte - 找到的最小错误数的最大超出值。

### setOnlyBestResultsRange(byte value) {#setOnlyBestResultsRange-byte-}
```
public abstract void setOnlyBestResultsRange(byte value)
```


设置找到的最小错误数的最大超出值。默认值为 0。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | byte | 找到的最小错误数的最大超出值。 |
|

### getConsiderTranspositions() {#getConsiderTranspositions--}
```
public abstract boolean getConsiderTranspositions()
```


获取一个值，指示算法是否必须将相邻两个字符的换位视为单个错误。默认值为 true。


**Returns:**
boolean - true 如果拼写纠正算法考虑换位；否则 false。

### setConsiderTranspositions(boolean value) {#setConsiderTranspositions-boolean-}
```
public abstract void setConsiderTranspositions(boolean value)
```


设置一个值，指示算法是否必须将相邻两个字符的换位视为单个错误。默认值为 true。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | boolean | true 如果拼写纠正算法考虑换位；否则 false。 |
|

