---
title: "PathDeleteResult"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "インデックスからインデックスされたファイルまたはフォルダーを削除する操作の結果を表します。"
type: docs
weight: 18
url: /ja/java/com.groupdocs.search.results/pathdeleteresult/
---
**Inheritance:**
java.lang.Object
```
public class PathDeleteResult
```

インデックスからインデックスされたファイルまたはフォルダーを削除する操作の結果を表します。


**Learn more**

* [Delete indexed paths](../https://docs.groupdocs.com/display/searchjava/Delete+indexed+paths)

## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [isSuccess()](#isSuccess--) | 削除操作の成功指標を返します。 |
|
|  | [getError()](#getError--) | 削除エラーの説明を返します。 |
|
|  | [getPath()](#getPath--) | 削除対象のファイルまたはフォルダーへのパスを返します。 |
|
### isSuccess() {#isSuccess--}
```
public final boolean isSuccess()
```


削除操作の成功指標を返します。


**Returns:**
boolean - 削除操作が成功した場合は  true 、それ以外の場合は  false  を返します。

### getError() {#getError--}
```
public final String getError()
```


削除エラーの説明を返します。


**Returns:**
java.lang.String - 削除エラーの説明です。

### getPath() {#getPath--}
```
public final String getPath()
```


削除対象のファイルまたはフォルダーへのパスを返します。


**Returns:**
java.lang.String - 削除対象のファイルまたはフォルダーへのパスです。

