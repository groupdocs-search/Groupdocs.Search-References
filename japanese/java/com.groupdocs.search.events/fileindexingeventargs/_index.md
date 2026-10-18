---
title: "FileIndexingEventArgs"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "ドキュメントのインデックス作成開始イベントの引数を表します。"
type: docs
weight: 14
url: /ja/java/com.groupdocs.search.events/fileindexingeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class FileIndexingEventArgs extends BaseIndexEventArgs
```

ドキュメントのインデックス作成開始イベントの引数を表します。


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getDocument()](#getDocument--) | ドキュメントを取得します。 |
|
|  | [getDocumentFullPath()](#getDocumentFullPath--) | ドキュメントのフルパスを取得します。 |
|
|  | [getDocumentKey()](#getDocumentKey--) | ドキュメントキーを取得します。 |
|
|  | [getSkipIndexing()](#getSkipIndexing--) | ドキュメントのインデックス作成をスキップすべきかを示す値を取得します。 |
|
|  | [setSkipIndexing(boolean value)](#setSkipIndexing-boolean-) | ドキュメントのインデックス作成をスキップすべきかを示す値を設定します。 |
|
|  | [getEncoding()](#getEncoding--) | ドキュメントのエンコーディングを取得します。 |
|
|  | [setEncoding(String value)](#setEncoding-java.lang.String-) | ドキュメントのエンコーディングを設定します。 |
|
|  | [getCustomExtractor()](#getCustomExtractor--) | カスタムテキスト抽出機能を取得します。 |
|
|  | [setCustomExtractor(IFieldExtractor value)](#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-) | カスタムテキスト抽出器を設定します。 |
|
|  | [getAdditionalFields()](#getAdditionalFields--) | ドキュメントの追加フィールドを取得します。 |
|
|  | [setAdditionalFields(DocumentField[] value)](#setAdditionalFields-com.groupdocs.search.common.DocumentField---) | ドキュメントの追加フィールドを設定します。 |
|
|  | [getAttributes()](#getAttributes--) | ドキュメントの属性を取得します。 |
|
|  | [setAttributes(String[] value)](#setAttributes-java.lang.String---) | ドキュメントの属性を設定します。 |
|
### getDocument() {#getDocument--}
```
public final Document getDocument()
```


ドキュメントを取得します。


**Returns:**
[Document](../../com.groupdocs.search/document) - The document.

### getDocumentFullPath() {#getDocumentFullPath--}
```
public final String getDocumentFullPath()
```


ドキュメントのフルパスを取得します。


**Returns:**
java.lang.String - ドキュメントのフルパス。

### getDocumentKey() {#getDocumentKey--}
```
public final String getDocumentKey()
```


ドキュメントキーを取得します。


**Returns:**
java.lang.String - ドキュメントキー。

### getSkipIndexing() {#getSkipIndexing--}
```
public final boolean getSkipIndexing()
```


ドキュメントのインデックス作成をスキップすべきかを示す値を取得します。


**Returns:**
boolean - ドキュメントのインデックス作成をスキップすべきかを示す値。

### setSkipIndexing(boolean value) {#setSkipIndexing-boolean-}
```
public final void setSkipIndexing(boolean value)
```


ドキュメントのインデックス作成をスキップすべきかを示す値を設定します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 値 | boolean | ドキュメントのインデックス作成をスキップすべきかを示す値。 |
|

### getEncoding() {#getEncoding--}
```
public final String getEncoding()
```


ドキュメントのエンコーディングを取得します。


**Returns:**
java.lang.String - ドキュメントのエンコーディング。

### setEncoding(String value) {#setEncoding-java.lang.String-}
```
public final void setEncoding(String value)
```


ドキュメントのエンコーディングを設定します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 値 | java.lang.String | ドキュメントのエンコーディング。 |
|

### getCustomExtractor() {#getCustomExtractor--}
```
public final IFieldExtractor getCustomExtractor()
```


カスタムテキスト抽出機能を取得します。


**Returns:**
[IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) - The custom text extractor.

### setCustomExtractor(IFieldExtractor value) {#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-}
```
public final void setCustomExtractor(IFieldExtractor value)
```


カスタムテキスト抽出器を設定します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | value | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | カスタムテキスト抽出器。 |
|

### getAdditionalFields() {#getAdditionalFields--}
```
public final DocumentField[] getAdditionalFields()
```


ドキュメントの追加フィールドを取得します。


**Returns:**
com.groupdocs.search.common.DocumentField[] - ドキュメントの追加フィールド。

### setAdditionalFields(DocumentField[] value) {#setAdditionalFields-com.groupdocs.search.common.DocumentField---}
```
public final void setAdditionalFields(DocumentField[] value)
```


ドキュメントの追加フィールドを設定します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | value | [DocumentField\[\]](../../com.groupdocs.search.common/documentfield) | ドキュメントの追加フィールド。 |
|

### getAttributes() {#getAttributes--}
```
public final String[] getAttributes()
```


ドキュメントの属性を取得します。


**Returns:**
java.lang.String[] - ドキュメントの属性。

### setAttributes(String[] value) {#setAttributes-java.lang.String---}
```
public final void setAttributes(String[] value)
```


ドキュメントの属性を設定します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 値 | java.lang.String[] | ドキュメントの属性。 |
|

