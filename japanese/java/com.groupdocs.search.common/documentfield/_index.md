---
title: "DocumentField"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "ドキュメントフィールドデータを表します。"
type: docs
weight: 15
url: /ja/java/com.groupdocs.search.common/documentfield/
---
**Inheritance:**
java.lang.Object
```
public class DocumentField
```

ドキュメントフィールドデータを表します。


**Learn more**

* [Custom text extractors](../https://docs.groupdocs.com/display/searchjava/Custom+text+extractors)
* [Indexing additional fields](../https://docs.groupdocs.com/display/searchjava/Indexing+additional+fields)

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [DocumentField(String name, String value)](#DocumentField-java.lang.String-java.lang.String-) | DocumentField クラスの新しいインスタンスを初期化します。 |
|
|  | [DocumentField(Object data)](#DocumentField-java.lang.Object-) | DocumentField クラスの新しいインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getName()](#getName--) | フィールド名を取得します。 |
|
|  | [getValue()](#getValue--) | フィールド値を取得します。 |
|
| [getCore()](#getCore--) |  |
### DocumentField(String name, String value) {#DocumentField-java.lang.String-java.lang.String-}
```
public DocumentField(String name, String value)
```


DocumentField クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | name | java.lang.String | フィールド名。 |
|
|  | 値 | java.lang.String | フィールド値。 |
|

### DocumentField(Object data) {#DocumentField-java.lang.Object-}
```
public DocumentField(Object data)
```


DocumentField クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | データ | java.lang.Object | シリアライズされたデータ。 |
|

### getName() {#getName--}
```
public String getName()
```


フィールド名を取得します。


**Returns:**
java.lang.String - フィールド名です。

### getValue() {#getValue--}
```
public String getValue()
```


フィールド値を取得します。


**Returns:**
java.lang.String - フィールド値。

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
