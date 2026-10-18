---
title: "DateFormatCollection"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "DateFormat オブジェクトのコレクションを表します。"
type: docs
weight: 14
url: /ja/java/com.groupdocs.search.options/dateformatcollection/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public abstract class DateFormatCollection implements Iterable<DateFormat>
```

DateFormat オブジェクトのコレクションを表します。


**Learn more**

* [Date range search](../https://docs.groupdocs.com/display/searchjava/Date+range+search)

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [DateFormatCollection()](#DateFormatCollection--) |  |
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [addItem(DateFormat item)](#addItem-com.groupdocs.search.options.DateFormat-) | コレクションに日付フォーマットオブジェクトを追加します。 |
|
|  | [clear()](#clear--) | コレクションからすべての要素を削除します。 |
|
|  | [containsItem(DateFormat item)](#containsItem-com.groupdocs.search.options.DateFormat-) | コレクションが特定の項目を含むかどうかを判断します。 |
|
|  | [copyToTArray(DateFormat[] array, int arrayIndex)](#copyToTArray-com.groupdocs.search.options.DateFormat---int-) | コレクションの要素を特定の Array インデックスから Array にコピーします。 |
|
|  | [size()](#size--) | コレクションに含まれる要素数を取得します。 |
|
|  | [isReadOnly()](#isReadOnly--) | コレクションが読み取り専用かどうかを示す値を取得します。 |
|
|  | [removeItem(DateFormat item)](#removeItem-com.groupdocs.search.options.DateFormat-) | コレクションから特定の要素の最初の出現を削除します。 |
|
|  | [iterator()](#iterator--) | コレクションを反復する列挙子を返します。 |
|
### DateFormatCollection() {#DateFormatCollection--}
```
public DateFormatCollection()
```


### addItem(DateFormat item) {#addItem-com.groupdocs.search.options.DateFormat-}
```
public abstract void addItem(DateFormat item)
```


コレクションに日付フォーマットオブジェクトを追加します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | item | [DateFormat](../../com.groupdocs.search.options/dateformat) | コレクションに追加する日付フォーマットオブジェクト。 |
|

### clear() {#clear--}
```
public abstract void clear()
```


コレクションからすべての要素を削除します。


### containsItem(DateFormat item) {#containsItem-com.groupdocs.search.options.DateFormat-}
```
public abstract boolean containsItem(DateFormat item)
```


コレクションが特定の項目を含むかどうかを判断します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | item | [DateFormat](../../com.groupdocs.search.options/dateformat) | コレクション内で検索する項目。 |
|

**Returns:**
boolean - コレクションで項目が見つかった場合は true、そうでない場合は false。

### copyToTArray(DateFormat[] array, int arrayIndex) {#copyToTArray-com.groupdocs.search.options.DateFormat---int-}
```
public abstract void copyToTArray(DateFormat[] array, int arrayIndex)
```


コレクションの要素を特定の Array インデックスから Array にコピーします。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | array | [DateFormat\[\]](../../com.groupdocs.search.options/dateformat) | コレクションからコピーされた要素の宛先となる一次元 Array。 |
|
|  | arrayIndex | int | コピーが開始される配列内のゼロベースインデックス。 |
|

### size() {#size--}
```
public abstract int size()
```


コレクションに含まれる要素数を取得します。


**Returns:**
int - コレクションに含まれる要素数。

### isReadOnly() {#isReadOnly--}
```
public abstract boolean isReadOnly()
```


コレクションが読み取り専用かどうかを示す値を取得します。


**Returns:**
boolean -  true  コレクションが読み取り専用の場合; それ以外の場合は  false 。

### removeItem(DateFormat item) {#removeItem-com.groupdocs.search.options.DateFormat-}
```
public abstract boolean removeItem(DateFormat item)
```


コレクションから特定の要素の最初の出現を削除します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | item | [DateFormat](../../com.groupdocs.search.options/dateformat) | コレクションから削除する項目。 |
|

**Returns:**
boolean -  true  アイテムがコレクションから正常に削除された場合; それ以外の場合は  false 。アイテムがコレクションに見つからない場合もこのメソッドは  false を返します。

### iterator() {#iterator--}
```
public abstract Iterator<DateFormat> iterator()
```


コレクションを反復する列挙子を返します。


**Returns:**
java.util.Iterator<com.groupdocs.search.options.DateFormat> - コレクションを反復処理できるイテレータ。

