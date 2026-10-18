---
title: "ドキュメント"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "ファイルシステムのストリームまたは構造からインデックスに追加されたドキュメントの基底クラスを表します。"
type: docs
weight: 13
url: /ja/java/com.groupdocs.search/document/
---
**Inheritance:**
java.lang.Object
```
public abstract class Document
```

ファイルシステム、ストリーム、または構造からインデックスに追加されたドキュメントの基底クラスを表します。さまざまなソースからドキュメントを作成するための静的メソッドを含みます。


**Learn more**

* [Indexing from different sources](../https://docs.groupdocs.com/search/java/indexing-from-different-sources/)

## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getDocumentSourceKind()](#getDocumentSourceKind--) | ドキュメントソースの種類を取得します。 |
|
|  | [getDocumentKey()](#getDocumentKey--) | インデックス内でドキュメントを識別するために使用されるドキュメントキーを取得します。 |
|
|  | [isLazy()](#isLazy--) | ドキュメントが必要に応じてロードされるかどうかを示す値を取得します。 |
|
|  | [getModificationDate()](#getModificationDate--) | ドキュメントの最終更新日を取得します。 |
|
|  | [getExtension()](#getExtension--) | このドキュメントタイプで使用される拡張子を取得します。 |
|
|  | [getAdditionalFields()](#getAdditionalFields--) | ドキュメントの追加フィールドを取得します。 |
|
|  | [setAdditionalFields(DocumentField[] value)](#setAdditionalFields-com.groupdocs.search.common.DocumentField---) | ドキュメントの追加フィールドを設定します。 |
|
|  | [getAttributes()](#getAttributes--) | ドキュメントの属性を取得します。 |
|
|  | [setAttributes(String[] value)](#setAttributes-java.lang.String---) | ドキュメントの属性を設定します。 |
|
|  | [createFromFile(String filePath)](#createFromFile-java.lang.String-) | ファイルからドキュメントを作成します。 |
|
|  | [createFromStream(String documentKey, Date modificationDate, String extension, InputStream stream)](#createFromStream-java.lang.String-java.util.Date-java.lang.String-java.io.InputStream-) | ストリームからドキュメントを作成します。 |
|
|  | [createFromStructure(String documentKey, Date modificationDate, DocumentField[] fields)](#createFromStructure-java.lang.String-java.util.Date-com.groupdocs.search.common.DocumentField---) | テキストフィールドの配列である構造体からドキュメントを作成します。 |
|
|  | [createLazy(DocumentSourceKind documentSourceKind, String documentKey, IDocumentLoader documentLoader)](#createLazy-com.groupdocs.search.common.DocumentSourceKind-java.lang.String-com.groupdocs.search.common.IDocumentLoader-) | 遅延ロードされるドキュメントを作成します。 |
|
|  | [toString()](#toString--) | 現在の Document を表す java.lang.String を返します。 |
|
### getDocumentSourceKind() {#getDocumentSourceKind--}
```
public abstract DocumentSourceKind getDocumentSourceKind()
```


ドキュメントソースの種類を取得します。


**Returns:**
[DocumentSourceKind](../../com.groupdocs.search.common/documentsourcekind) - The document source kind.

### getDocumentKey() {#getDocumentKey--}
```
public abstract String getDocumentKey()
```


インデックス内でドキュメントを識別するために使用されるドキュメントキーを取得します。


**Returns:**
java.lang.String - インデックス内でドキュメントを識別するために使用されるドキュメントキー。

### isLazy() {#isLazy--}
```
public abstract boolean isLazy()
```


ドキュメントが必要に応じてロードされるかどうかを示す値を取得します。


**Returns:**
boolean - ドキュメントが必要に応じてロードされるかどうかを示す値。

### getModificationDate() {#getModificationDate--}
```
public abstract Date getModificationDate()
```


ドキュメントの最終更新日を取得します。


**Returns:**
java.util.Date - ドキュメントの最終更新日。

### getExtension() {#getExtension--}
```
public abstract String getExtension()
```


このドキュメントタイプで使用される拡張子を取得します。


**Returns:**
java.lang.String - このドキュメントタイプで使用される拡張子。

### getAdditionalFields() {#getAdditionalFields--}
```
public DocumentField[] getAdditionalFields()
```


ドキュメントの追加フィールドを取得します。


**Returns:**
com.groupdocs.search.common.DocumentField[] - ドキュメントの追加フィールド。

### setAdditionalFields(DocumentField[] value) {#setAdditionalFields-com.groupdocs.search.common.DocumentField---}
```
public void setAdditionalFields(DocumentField[] value)
```


ドキュメントの追加フィールドを設定します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | value | [DocumentField\[\]](../../com.groupdocs.search.common/documentfield) | ドキュメントの追加フィールド。 |
|

### getAttributes() {#getAttributes--}
```
public String[] getAttributes()
```


ドキュメントの属性を取得します。


**Returns:**
java.lang.String[] - ドキュメントの属性。

### setAttributes(String[] value) {#setAttributes-java.lang.String---}
```
public void setAttributes(String[] value)
```


ドキュメントの属性を設定します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 値 | java.lang.String[] | ドキュメントの属性。 |
|

### createFromFile(String filePath) {#createFromFile-java.lang.String-}
```
public static Document createFromFile(String filePath)
```


ファイルからドキュメントを作成します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | filePath | java.lang.String | ドキュメントのファイルパスです。 |
|

**Returns:**
[Document](../../com.groupdocs.search/document) - The created document.

### createFromStream(String documentKey, Date modificationDate, String extension, InputStream stream) {#createFromStream-java.lang.String-java.util.Date-java.lang.String-java.io.InputStream-}
```
public static Document createFromStream(String documentKey, Date modificationDate, String extension, InputStream stream)
```


ストリームからドキュメントを作成します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | documentKey | java.lang.String | ドキュメントキーです。 |
|
|  | modificationDate | java.util.Date | ドキュメントの更新日です。 |
|
|  | extension | java.lang.String | ドキュメント拡張子です。 |
|
|  | stream | java.io.InputStream | ドキュメントストリームです。 |
|

**Returns:**
[Document](../../com.groupdocs.search/document) - The created document.

### createFromStructure(String documentKey, Date modificationDate, DocumentField[] fields) {#createFromStructure-java.lang.String-java.util.Date-com.groupdocs.search.common.DocumentField---}
```
public static Document createFromStructure(String documentKey, Date modificationDate, DocumentField[] fields)
```


テキストフィールドの配列である構造体からドキュメントを作成します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | documentKey | java.lang.String | ドキュメントキーです。 |
|
|  | modificationDate | java.util.Date | ドキュメントの更新日です。 |
|
|  | fields | [DocumentField\[\]](../../com.groupdocs.search.common/documentfield) | ドキュメントフィールドです。 |
|

**Returns:**
[Document](../../com.groupdocs.search/document) - The created document.

### createLazy(DocumentSourceKind documentSourceKind, String documentKey, IDocumentLoader documentLoader) {#createLazy-com.groupdocs.search.common.DocumentSourceKind-java.lang.String-com.groupdocs.search.common.IDocumentLoader-}
```
public static Document createLazy(DocumentSourceKind documentSourceKind, String documentKey, IDocumentLoader documentLoader)
```


遅延ロードされるドキュメントを作成します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | documentSourceKind | [DocumentSourceKind](../../com.groupdocs.search.common/documentsourcekind) | ドキュメントのソース種別です。この値はロードされたドキュメントの種別と一致する必要があります。 |
|
|  | documentKey | java.lang.String | ドキュメントキーです。この値はロードされたドキュメントのキーと一致する必要があります。 |
|
|  | documentLoader | [IDocumentLoader](../../com.groupdocs.search.common/idocumentloader) | ドキュメントローダーです。 |
|

**Returns:**
[Document](../../com.groupdocs.search/document) - The created document.

### toString() {#toString--}
```
public String toString()
```


現在の Document を表す java.lang.String を返します。


**Returns:**
java.lang.String - 現在の Document を表す java.lang.String

