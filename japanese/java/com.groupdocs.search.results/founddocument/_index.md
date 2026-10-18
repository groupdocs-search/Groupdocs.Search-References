---
title: "FoundDocument"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "見つかったドキュメントを表します。"
type: docs
weight: 14
url: /ja/java/com.groupdocs.search.results/founddocument/
---
**Inheritance:**
java.lang.Object
```
public abstract class FoundDocument
```

見つかったドキュメントを表します。


**Learn more**

* [Search results](../https://docs.groupdocs.com/display/searchjava/Search+results)

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [FoundDocument()](#FoundDocument--) |  |
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getDocumentInfo()](#getDocumentInfo--) | ドキュメント情報を取得します。 |
|
|  | [getRelevance()](#getRelevance--) | 検索結果の関連性を取得します。 |
|
|  | [getOccurrenceCount()](#getOccurrenceCount--) | 見つかった出現回数を取得します。 |
|
|  | [getFoundFields()](#getFoundFields--) | 見つかったドキュメントフィールドを取得します。 |
|
|  | [getTerms()](#getTerms--) | 見つかった用語を取得します。 |
|
|  | [getTermSequences()](#getTermSequences--) | 見つかった用語シーケンスを取得します。 |
|
|  | [getAttributes()](#getAttributes--) | 見つかったドキュメントに関連付けられた属性を取得します。 |
|
|  | [toString()](#toString--) | 見つかったドキュメントの文字列表現を返します。 |
|
|  | [serialize()](#serialize--) | 現在のインスタンスをバイト配列にシリアライズします。 |
|
|  | [deserialize(byte[] array)](#deserialize-byte---) | バイト配列からインスタンスをデシリアライズします。 |
|
### FoundDocument() {#FoundDocument--}
```
public FoundDocument()
```


### getDocumentInfo() {#getDocumentInfo--}
```
public abstract DocumentInfo getDocumentInfo()
```


ドキュメント情報を取得します。


**Returns:**
[DocumentInfo](../../com.groupdocs.search.results/documentinfo) - The document info.

### getRelevance() {#getRelevance--}
```
public abstract double getRelevance()
```


検索結果の関連性を取得します。


**Returns:**
double - 検索結果の関連性。

### getOccurrenceCount() {#getOccurrenceCount--}
```
public abstract int getOccurrenceCount()
```


見つかった出現回数を取得します。


**Returns:**
int - 見つかった出現回数。

### getFoundFields() {#getFoundFields--}
```
public abstract FoundDocumentField[] getFoundFields()
```


見つかったドキュメントフィールドを取得します。


**Returns:**
com.groupdocs.search.results.FoundDocumentField[] - 見つかったドキュメントフィールド。

### getTerms() {#getTerms--}
```
public abstract String[] getTerms()
```


見つかった用語を取得します。プロパティがアクセスされるたびに値が評価されます。


**Returns:**
java.lang.String[] - 見つかった用語。

### getTermSequences() {#getTermSequences--}
```
public abstract String[][] getTermSequences()
```


見つかった用語シーケンスを取得します。


**Returns:**
java.lang.String[][] - 見つかった用語シーケンス。

### getAttributes() {#getAttributes--}
```
public abstract String[] getAttributes()
```


検索されたドキュメントに関連付けられた属性を取得します。属性を取得するには、検索オプションで対応するオプションを有効にする必要があります。


**Returns:**
java.lang.String[] - 検索されたドキュメントに関連付けられた属性

### toString() {#toString--}
```
public abstract String toString()
```


見つかったドキュメントの文字列表現を返します。


**Returns:**
java.lang.String - 検索されたドキュメントを表す文字列

### serialize() {#serialize--}
```
public abstract byte[] serialize()
```


現在のインスタンスをバイト配列にシリアライズします。


**Returns:**
byte[] - 現在のインスタンスを表すバイト配列です。

### deserialize(byte[] array) {#deserialize-byte---}
```
public static FoundDocument deserialize(byte[] array)
```


バイト配列からインスタンスをデシリアライズします。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 配列 | byte[] | デシリアライズ元のバイト配列です。 |
|

**Returns:**
[FoundDocument](../../com.groupdocs.search.results/founddocument) - An instance deserialized from a byte array.

