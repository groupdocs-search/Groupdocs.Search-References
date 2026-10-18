---
title: "DocumentInfo"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "インデックスされたドキュメントの記述子を表します。"
type: docs
weight: 11
url: /ja/java/com.groupdocs.search.results/documentinfo/
---
**Inheritance:**
java.lang.Object
```
public abstract class DocumentInfo
```

インデックスされたドキュメントの記述子を表します。


**Learn more**

* [Search results](../https://docs.groupdocs.com/display/searchjava/Search+results)
* [Getting indexed documents](../https://docs.groupdocs.com/display/searchjava/Getting+indexed+documents)

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [DocumentInfo()](#DocumentInfo--) |  |
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [toString()](#toString--) | 現在の  DocumentInfo  を表す  System.String  を返します。 |
|
|  | [getFilePath()](#getFilePath--) | ファイルからインデックスされた場合のファイルパス、またはストリームまたは構造からインデックスされた場合のドキュメントキーを取得します。 |
|
|  | [getFileType()](#getFileType--) | ファイルタイプを取得します。 |
|
|  | [getFormatFamily()](#getFormatFamily--) | ドキュメント形式ファミリを取得します。 |
|
|  | [getInnerPath()](#getInnerPath--) | コンテナドキュメント項目の内部パスを取得します。 |
|
|  | [getInnerPathParts()](#getInnerPathParts--) | コンテナドキュメント項目の内部パス部分を取得します。 |
|
|  | [getDocumentSourceKind()](#getDocumentSourceKind--) | ドキュメントソースの種類を取得します。 |
|
|  | [getIndexedWithError()](#getIndexedWithError--) | インデックスエラーの指標を取得します。 |
|
|  | [serialize()](#serialize--) | 現在のインスタンスをバイト配列にシリアライズします。 |
|
|  | [deserialize(byte[] array)](#deserialize-byte---) | バイト配列からインスタンスをデシリアライズします。 |
|
### DocumentInfo() {#DocumentInfo--}
```
public DocumentInfo()
```


### toString() {#toString--}
```
public abstract String toString()
```


現在の  DocumentInfo  を表す  System.String  を返します。


**Returns:**
java.lang.String - 現在の  DocumentInfo  を表す  System.String  です。

### getFilePath() {#getFilePath--}
```
public abstract String getFilePath()
```


ファイルからインデックスされた場合のファイルパス、またはストリームまたは構造からインデックスされた場合のドキュメントキーを取得します。


**Returns:**
java.lang.String - ファイルパスまたはドキュメントキーです。

### getFileType() {#getFileType--}
```
public abstract FileType getFileType()
```


ファイルタイプを取得します。


**Returns:**
[FileType](../../com.groupdocs.search.results/filetype) - The file type.

### getFormatFamily() {#getFormatFamily--}
```
public abstract FormatFamily getFormatFamily()
```


ドキュメント形式ファミリを取得します。


**Returns:**
[FormatFamily](../../com.groupdocs.search.results/formatfamily) - The document format family.

### getInnerPath() {#getInnerPath--}
```
public abstract String getInnerPath()
```


コンテナドキュメント項目の内部パスを取得します。


**Returns:**
java.lang.String - 内部パス。

### getInnerPathParts() {#getInnerPathParts--}
```
public abstract String[] getInnerPathParts()
```


コンテナドキュメント項目の内部パス部分を取得します。


**Returns:**
java.lang.String[] - 内部パス部分です。

### getDocumentSourceKind() {#getDocumentSourceKind--}
```
public abstract DocumentSourceKind getDocumentSourceKind()
```


ドキュメントソースの種類を取得します。


**Returns:**
[DocumentSourceKind](../../com.groupdocs.search.common/documentsourcekind) - The document source kind.

### getIndexedWithError() {#getIndexedWithError--}
```
public abstract boolean getIndexedWithError()
```


インデックスエラーの指標を取得します。


**Returns:**
boolean - インデックスエラーの指標です。

### serialize() {#serialize--}
```
public abstract byte[] serialize()
```


現在のインスタンスをバイト配列にシリアライズします。


**Returns:**
byte[] - 現在のインスタンスを表すバイト配列です。

### deserialize(byte[] array) {#deserialize-byte---}
```
public static DocumentInfo deserialize(byte[] array)
```


バイト配列からインスタンスをデシリアライズします。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 配列 | byte[] | デシリアライズ元のバイト配列です。 |
|

**Returns:**
[DocumentInfo](../../com.groupdocs.search.results/documentinfo) - An instance deserialized from a byte array.

