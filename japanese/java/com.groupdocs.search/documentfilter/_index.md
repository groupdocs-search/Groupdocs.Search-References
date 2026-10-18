---
title: "DocumentFilter"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "ドキュメントフィルタの基底クラスを表します。"
type: docs
weight: 14
url: /ja/java/com.groupdocs.search/documentfilter/
---
**Inheritance:**
java.lang.Object
```
public abstract class DocumentFilter
```

ドキュメントフィルターの基底クラスを表します。ドキュメントフィルターインスタンスの作成用メソッドを含みます。


**Learn more**

* [Document filtering during indexing](../https://docs.groupdocs.com/display/searchjava/Document+filtering+during+indexing)

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [DocumentFilter()](#DocumentFilter--) |  |
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [toString()](#toString--) | ドキュメントフィルターの文字列表現を返します。 |
|
|  | [createCreationTimeLowerBound(Date lowerBound)](#createCreationTimeLowerBound-java.util.Date-) | 下限よりも作成日が早いドキュメントをスキップするフィルターを作成します。 |
|
|  | [createCreationTimeUpperBound(Date upperBound)](#createCreationTimeUpperBound-java.util.Date-) | 上限よりも作成日が遅いドキュメントをスキップするフィルターを作成します。 |
|
|  | [createCreationTimeRange(Date lowerBound, Date upperBound)](#createCreationTimeRange-java.util.Date-java.util.Date-) | 指定された範囲外の作成日のドキュメントをスキップするフィルターを作成します。 |
|
|  | [createModificationTimeLowerBound(Date lowerBound)](#createModificationTimeLowerBound-java.util.Date-) | 下限よりも更新日が早いドキュメントをスキップするフィルターを作成します。 |
|
|  | [createModificationTimeUpperBound(Date upperBound)](#createModificationTimeUpperBound-java.util.Date-) | 上限よりも更新日が遅いドキュメントをスキップするフィルターを作成します。 |
|
|  | [createModificationTimeRange(Date lowerBound, Date upperBound)](#createModificationTimeRange-java.util.Date-java.util.Date-) | 指定された範囲外の更新日のドキュメントをスキップするフィルターを作成します。 |
|
|  | [createFilePathRegularExpression(String pattern)](#createFilePathRegularExpression-java.lang.String-) | 正規表現に一致しないドキュメントをスキップするフィルターを作成します。 |
|
|  | [createFilePathRegularExpression(String pattern, int options)](#createFilePathRegularExpression-java.lang.String-int-) | 正規表現に一致しないドキュメントをスキップするフィルターを作成します。 |
|
|  | [createFileLengthLowerBound(long lowerBound)](#createFileLengthLowerBound-long-) | 下限よりも長さが短いドキュメントをスキップするフィルターを作成します。 |
|
|  | [createFileLengthUpperBound(long upperBound)](#createFileLengthUpperBound-long-) | 上限よりも長さが長いドキュメントをスキップするフィルターを作成します。 |
|
|  | [createFileLengthRange(long lowerBound, long upperBound)](#createFileLengthRange-long-long-) | 指定されたドキュメント長さの範囲外のドキュメントをスキップするフィルターを作成します。 |
|
|  | [createFileExtension(String[] extensions)](#createFileExtension-java.lang.String...-) | 許可された拡張子を持たないドキュメントをスキップするフィルターを作成します。 |
|
|  | [createNot(DocumentFilter innerFilter)](#createNot-com.groupdocs.search.DocumentFilter-) | 指定された内部フィルターに対して逆のロジックを持つフィルターを作成します。 |
|
|  | [createAnd(DocumentFilter[] filters)](#createAnd-com.groupdocs.search.DocumentFilter...-) | 指定されたフィルターの論理積を作成します。 |
|
|  | [createOr(DocumentFilter[] filters)](#createOr-com.groupdocs.search.DocumentFilter...-) | 指定されたフィルターの論理和を作成します。 |
|
### DocumentFilter() {#DocumentFilter--}
```
public DocumentFilter()
```


### toString() {#toString--}
```
public abstract String toString()
```


ドキュメントフィルターの文字列表現を返します。


**Returns:**
java.lang.String - ドキュメントフィルターの文字列表現です。

### createCreationTimeLowerBound(Date lowerBound) {#createCreationTimeLowerBound-java.util.Date-}
```
public static DocumentFilter createCreationTimeLowerBound(Date lowerBound)
```


下限よりも作成日が早いドキュメントをスキップするフィルターを作成します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | lowerBound | java.util.Date | ドキュメント作成時間の下限です。 |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document creation time.

### createCreationTimeUpperBound(Date upperBound) {#createCreationTimeUpperBound-java.util.Date-}
```
public static DocumentFilter createCreationTimeUpperBound(Date upperBound)
```


上限よりも作成日が遅いドキュメントをスキップするフィルターを作成します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | upperBound | java.util.Date | ドキュメント作成時間の上限です。 |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document creation time.

### createCreationTimeRange(Date lowerBound, Date upperBound) {#createCreationTimeRange-java.util.Date-java.util.Date-}
```
public static DocumentFilter createCreationTimeRange(Date lowerBound, Date upperBound)
```


指定された範囲外の作成日のドキュメントをスキップするフィルターを作成します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | lowerBound | java.util.Date | ドキュメント作成時間の下限です。 |
|
|  | upperBound | java.util.Date | ドキュメント作成時間の上限です。 |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document creation time.

### createModificationTimeLowerBound(Date lowerBound) {#createModificationTimeLowerBound-java.util.Date-}
```
public static DocumentFilter createModificationTimeLowerBound(Date lowerBound)
```


下限よりも更新日が早いドキュメントをスキップするフィルターを作成します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | lowerBound | java.util.Date | ドキュメント更新時間の下限です。 |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document modification time.

### createModificationTimeUpperBound(Date upperBound) {#createModificationTimeUpperBound-java.util.Date-}
```
public static DocumentFilter createModificationTimeUpperBound(Date upperBound)
```


上限よりも更新日が遅いドキュメントをスキップするフィルターを作成します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | upperBound | java.util.Date | ドキュメント更新時間の上限です。 |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document modification time.

### createModificationTimeRange(Date lowerBound, Date upperBound) {#createModificationTimeRange-java.util.Date-java.util.Date-}
```
public static DocumentFilter createModificationTimeRange(Date lowerBound, Date upperBound)
```


指定された範囲外の更新日のドキュメントをスキップするフィルターを作成します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | lowerBound | java.util.Date | ドキュメント更新時間の下限です。 |
|
|  | upperBound | java.util.Date | ドキュメント更新時間の上限です。 |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document modification time.

### createFilePathRegularExpression(String pattern) {#createFilePathRegularExpression-java.lang.String-}
```
public static DocumentFilter createFilePathRegularExpression(String pattern)
```


正規表現に一致しないドキュメントをスキップするフィルターを作成します。正規表現はドキュメントのフルパスに適用されます。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | パターン | java.lang.String | 正規表現パターンです。 |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by file name.

### createFilePathRegularExpression(String pattern, int options) {#createFilePathRegularExpression-java.lang.String-int-}
```
public static DocumentFilter createFilePathRegularExpression(String pattern, int options)
```


正規表現に一致しないドキュメントをスキップするフィルターを作成します。正規表現はドキュメントのフルパスに適用されます。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | パターン | java.lang.String | 正規表現パターンです。 |
|
|  | オプション | int | 正規表現のオプションです。 |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by file name.

### createFileLengthLowerBound(long lowerBound) {#createFileLengthLowerBound-long-}
```
public static DocumentFilter createFileLengthLowerBound(long lowerBound)
```


下限よりも長さが短いドキュメントをスキップするフィルターを作成します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | lowerBound | long | ドキュメント長さの下限です。 |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document length.

### createFileLengthUpperBound(long upperBound) {#createFileLengthUpperBound-long-}
```
public static DocumentFilter createFileLengthUpperBound(long upperBound)
```


上限よりも長さが長いドキュメントをスキップするフィルターを作成します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | upperBound | long | ドキュメント長さの上限です。 |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document length.

### createFileLengthRange(long lowerBound, long upperBound) {#createFileLengthRange-long-long-}
```
public static DocumentFilter createFileLengthRange(long lowerBound, long upperBound)
```


指定されたドキュメント長さの範囲外のドキュメントをスキップするフィルターを作成します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | lowerBound | long | ドキュメント長さの下限です。 |
|
|  | upperBound | long | ドキュメント長さの上限です。 |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document length.

### createFileExtension(String[] extensions) {#createFileExtension-java.lang.String...-}
```
public static DocumentFilter createFileExtension(String[] extensions)
```


許可された拡張子を持たないドキュメントをスキップするフィルターを作成します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 拡張子 | java.lang.String[] | 許可可能な拡張子の一覧です。 |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document extension.

### createNot(DocumentFilter innerFilter) {#createNot-com.groupdocs.search.DocumentFilter-}
```
public static DocumentFilter createNot(DocumentFilter innerFilter)
```


指定された内部フィルターに対して逆のロジックを持つフィルターを作成します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | innerFilter | [DocumentFilter](../../com.groupdocs.search/documentfilter) | 内部ドキュメントフィルタ。 |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - An inverted document filter.

### createAnd(DocumentFilter[] filters) {#createAnd-com.groupdocs.search.DocumentFilter...-}
```
public static DocumentFilter createAnd(DocumentFilter[] filters)
```


指定されたフィルターの論理積を作成します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | filters | [DocumentFilter\[\]](../../com.groupdocs.search/documentfilter) | ドキュメントフィルタ。 |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter that represents result of conjunction of the specified filters.

### createOr(DocumentFilter[] filters) {#createOr-com.groupdocs.search.DocumentFilter...-}
```
public static DocumentFilter createOr(DocumentFilter[] filters)
```


指定されたフィルターの論理和を作成します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | filters | [DocumentFilter\[\]](../../com.groupdocs.search/documentfilter) | ドキュメントフィルタ。 |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter that represents result of disjunction of the specified filters.

