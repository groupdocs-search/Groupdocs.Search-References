---
title: "DeleteResult"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "インデックスからインデックス化されたファイルまたはフォルダーを削除する操作の結果を表します。"
type: docs
weight: 10
url: /ja/java/com.groupdocs.search.results/deleteresult/
---
**Inheritance:**
java.lang.Object
```
public class DeleteResult
```

インデックスからインデックス化されたファイルまたはフォルダーを削除する操作の結果を表します。


**Learn more**

* [Delete indexed paths](../https://docs.groupdocs.com/display/searchjava/Delete+indexed+paths)

## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getItemResults()](#getItemResults--) | 各パスの削除結果を返します。 |
|
|  | [getTotalCount()](#getTotalCount--) | 削除するパスの総数を返します。 |
|
|  | [getSuccessCount()](#getSuccessCount--) | 正常に削除されたパスの数を返します。 |
|
|  | [getFailedCount()](#getFailedCount--) | エラーにより削除されなかったパスの数を返します。 |
|
|  | [getErrors()](#getErrors--) | 削除エラーの説明を返します。 |
|
### getItemResults() {#getItemResults--}
```
public final PathDeleteResult[] getItemResults()
```


各パスの削除結果を返します。


**Returns:**
com.groupdocs.search.results.PathDeleteResult[] - 各パスの削除結果。

### getTotalCount() {#getTotalCount--}
```
public final int getTotalCount()
```


削除するパスの総数を返します。


**Returns:**
int - 削除するパスの総数。

### getSuccessCount() {#getSuccessCount--}
```
public final int getSuccessCount()
```


正常に削除されたパスの数を返します。


**Returns:**
int - 正常に削除されたパスの数。

### getFailedCount() {#getFailedCount--}
```
public final int getFailedCount()
```


エラーにより削除されなかったパスの数を返します。


**Returns:**
int - エラーにより削除されなかったパスの数。

### getErrors() {#getErrors--}
```
public final String[] getErrors()
```


削除エラーの説明を返します。


**Returns:**
java.lang.String[] - 削除エラーの説明。

