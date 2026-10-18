---
title: "FoundDocumentField"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "見つかったドキュメントフィールドを表します。"
type: docs
weight: 15
url: /ja/java/com.groupdocs.search.results/founddocumentfield/
---
**Inheritance:**
java.lang.Object
```
public abstract class FoundDocumentField
```

見つかったドキュメントフィールドを表します。


**Learn more**

* [Search results](../https://docs.groupdocs.com/display/searchjava/Search+results)

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [FoundDocumentField()](#FoundDocumentField--) |  |
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getFieldName()](#getFieldName--) | フィールド名を取得します。 |
|
|  | [getOccurrenceCount()](#getOccurrenceCount--) | 見つかった出現回数を取得します。 |
|
|  | [getTerms()](#getTerms--) | 見つかった用語を取得します。 |
|
|  | [getTermsOccurrences()](#getTermsOccurrences--) | 見つかった用語の出現回数を取得します。 |
|
|  | [getTermSequences()](#getTermSequences--) | 見つかった用語シーケンスを取得します。 |
|
|  | [getTermSequencesOccurrences()](#getTermSequencesOccurrences--) | 見つかった用語シーケンスの出現回数を取得します。 |
|
|  | [toString()](#toString--) | 見つかったドキュメントフィールドの文字列表現を返します。 |
|
|  | [serialize()](#serialize--) | 現在のインスタンスをバイト配列にシリアライズします。 |
|
|  | [deserialize(byte[] array)](#deserialize-byte---) | バイト配列からインスタンスをデシリアライズします。 |
|
### FoundDocumentField() {#FoundDocumentField--}
```
public FoundDocumentField()
```


### getFieldName() {#getFieldName--}
```
public abstract String getFieldName()
```


フィールド名を取得します。


**Returns:**
java.lang.String - フィールド名です。

### getOccurrenceCount() {#getOccurrenceCount--}
```
public abstract int getOccurrenceCount()
```


見つかった出現回数を取得します。


**Returns:**
int - 見つかった出現回数。

### getTerms() {#getTerms--}
```
public abstract String[] getTerms()
```


見つかった用語を取得します。


**Returns:**
java.lang.String[] - 見つかった用語。

### getTermsOccurrences() {#getTermsOccurrences--}
```
public abstract int[] getTermsOccurrences()
```


見つかった用語の出現回数を取得します。


**Returns:**
int[] - 見つかった用語の出現回数。

### getTermSequences() {#getTermSequences--}
```
public abstract String[][] getTermSequences()
```


見つかった用語シーケンスを取得します。


**Returns:**
java.lang.String[][] - 見つかった用語シーケンス。

### getTermSequencesOccurrences() {#getTermSequencesOccurrences--}
```
public abstract int[] getTermSequencesOccurrences()
```


見つかった用語シーケンスの出現回数を取得します。


**Returns:**
int[] - 見つかった用語シーケンスの出現回数。

### toString() {#toString--}
```
public abstract String toString()
```


見つかったドキュメントフィールドの文字列表現を返します。


**Returns:**
java.lang.String - 見つかったドキュメントフィールドを表す文字列。

### serialize() {#serialize--}
```
public abstract byte[] serialize()
```


現在のインスタンスをバイト配列にシリアライズします。


**Returns:**
byte[] - 現在のインスタンスを表すバイト配列です。

### deserialize(byte[] array) {#deserialize-byte---}
```
public static FoundDocumentField deserialize(byte[] array)
```


バイト配列からインスタンスをデシリアライズします。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 配列 | byte[] | デシリアライズ元のバイト配列です。 |
|

**Returns:**
[FoundDocumentField](../../com.groupdocs.search.results/founddocumentfield) - An instance deserialized from a byte array.

