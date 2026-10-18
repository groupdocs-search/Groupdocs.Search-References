---
title: "DocumentStatus"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "ドキュメント処理のステータスを表します。"
type: docs
weight: 40
url: /ja/java/com.groupdocs.search.common/documentstatus/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum DocumentStatus extends Enum<DocumentStatus>
```

ドキュメント処理のステータスを表します。

## Fields

| Field | 説明 |
| --- | --- |
|  | [SuccessfullyProcessed](#SuccessfullyProcessed) | ドキュメントが正常にインデックス付けされました。 |
|
|  | [Skipped](#Skipped) | ドキュメントはスキップされました。 |
|
|  | [ProcessedWithError](#ProcessedWithError) | ドキュメントのインデックス付け中にエラーが発生しました。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### SuccessfullyProcessed {#SuccessfullyProcessed}
```
public static final DocumentStatus SuccessfullyProcessed
```


ドキュメントが正常にインデックス付けされました。


### Skipped {#Skipped}
```
public static final DocumentStatus Skipped
```


ドキュメントはスキップされました。


### ProcessedWithError {#ProcessedWithError}
```
public static final DocumentStatus ProcessedWithError
```


ドキュメントのインデックス付け中にエラーが発生しました。


### values() {#values--}
```
public static DocumentStatus[] values()
```




**Returns:**
com.groupdocs.search.common.DocumentStatus[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static DocumentStatus valueOf(String name)
```




**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[DocumentStatus](../../com.groupdocs.search.common/documentstatus)
