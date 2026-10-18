---
title: "DocumentSourceKind"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "ドキュメントソースの種類を定義します。"
type: docs
weight: 39
url: /ja/java/com.groupdocs.search.common/documentsourcekind/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum DocumentSourceKind extends Enum<DocumentSourceKind>
```

ドキュメントソースの種類を定義します。

## Fields

| Field | 説明 |
| --- | --- |
|  | [File](#File) | ファイルドキュメントソースです。 |
|
|  | [Stream](#Stream) | ストリームドキュメントソースです。 |
|
|  | [Structure](#Structure) | 構造ドキュメントソースです。 |
|
|  | [ExtractedData](#ExtractedData) | 以前に抽出されたデータのドキュメントソースです。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### File {#File}
```
public static final DocumentSourceKind File
```


ファイルドキュメントソースです。


### Stream {#Stream}
```
public static final DocumentSourceKind Stream
```


ストリームドキュメントソースです。


### Structure {#Structure}
```
public static final DocumentSourceKind Structure
```


構造ドキュメントソースです。


### ExtractedData {#ExtractedData}
```
public static final DocumentSourceKind ExtractedData
```


以前に抽出されたデータのドキュメントソースです。


### values() {#values--}
```
public static DocumentSourceKind[] values()
```




**Returns:**
com.groupdocs.search.common.DocumentSourceKind[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static DocumentSourceKind valueOf(String name)
```




**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[DocumentSourceKind](../../com.groupdocs.search.common/documentsourcekind)
