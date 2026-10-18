---
title: "AliasDictionary"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "エイリアス辞書のインターフェイスを定義します。"
type: docs
weight: 14
url: /ja/java/com.groupdocs.search.dictionaries/aliasdictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface AliasDictionary extends DictionaryBase, Iterable<String>
```

エイリアス辞書のインターフェイスを定義します。


**Learn more**

* [Using aliases](../https://docs.groupdocs.com/display/searchjava/Using+aliases)
* [Managing alias dictionary](../https://docs.groupdocs.com/display/searchjava/Alias+dictionary)

## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getCount()](#getCount--) | AliasDictionary に含まれるエイリアスの数を取得します。 |
|
|  | [addRange(Iterable<AliasReplacementPair> pairs)](#addRange-java.lang.Iterable-com.groupdocs.search.dictionaries.AliasReplacementPair--) | 指定されたエイリアス/置換ペアのコレクションをこの AliasDictionary インスタンスに追加します。 |
|
|  | [addRange(AliasReplacementPair[] pairs)](#addRange-com.groupdocs.search.dictionaries.AliasReplacementPair---) | 指定されたエイリアス/置換ペアのコレクションをこの AliasDictionary インスタンスに追加します。 |
|
|  | [add(String alias, String text)](#add-java.lang.String-java.lang.String-) | 指定されたエイリアスと関連テキストのペアをこの AliasDictionary インスタンスに追加します。 |
|
|  | [remove(String alias)](#remove-java.lang.String-) | 指定されたエイリアスを AliasDictionary オブジェクトから削除します。 |
|
|  | [contains(String alias)](#contains-java.lang.String-) | AliasDictionary オブジェクトが指定されたエイリアスを含むかどうかを判定します。 |
|
|  | [getText(String alias)](#getText-java.lang.String-) | 指定されたエイリアスに関連付けられたテキストを取得します。 |
|
|  | [clear()](#clear--) | AliasDictionary オブジェクトからすべてのエイリアスを削除します。 |
|
|  | [iterator()](#iterator--) | コレクションを反復するイテレータを返します。 |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


AliasDictionary に含まれるエイリアスの数を取得します。


**Returns:**
int - AliasDictionary に含まれるエイリアスの数です。

### addRange(Iterable<AliasReplacementPair> pairs) {#addRange-java.lang.Iterable-com.groupdocs.search.dictionaries.AliasReplacementPair--}
```
public abstract void addRange(Iterable<AliasReplacementPair> pairs)
```


指定されたエイリアス/置換ペアのコレクションをこの AliasDictionary インスタンスに追加します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | ペア | java.lang.Iterable<com.groupdocs.search.dictionaries.AliasReplacementPair> | 辞書に追加するエイリアス/置換ペアのコレクションです。 |
|

### addRange(AliasReplacementPair[] pairs) {#addRange-com.groupdocs.search.dictionaries.AliasReplacementPair---}
```
public abstract void addRange(AliasReplacementPair[] pairs)
```


指定されたエイリアス/置換ペアのコレクションをこの AliasDictionary インスタンスに追加します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | pairs | [AliasReplacementPair\[\]](../../com.groupdocs.search.dictionaries/aliasreplacementpair) | 辞書に追加するエイリアス/置換ペアのコレクションです。 |
|

### add(String alias, String text) {#add-java.lang.String-java.lang.String-}
```
public abstract void add(String alias, String text)
```


指定されたエイリアスと関連テキストのペアをこの AliasDictionary インスタンスに追加します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | エイリアス | java.lang.String | 辞書に追加するエイリアスです。 |
|
|  | テキスト | java.lang.String | エイリアスに関連付けるテキストです。 |
|

### remove(String alias) {#remove-java.lang.String-}
```
public abstract boolean remove(String alias)
```


指定されたエイリアスを AliasDictionary オブジェクトから削除します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | エイリアス | java.lang.String | 削除するエイリアスです。 |
|

**Returns:**
boolean - エイリアスが正常に見つかり削除された場合は true を返します。エイリアスが AliasDictionary オブジェクトに見つからない場合は false を返します。

### contains(String alias) {#contains-java.lang.String-}
```
public abstract boolean contains(String alias)
```


AliasDictionary オブジェクトが指定されたエイリアスを含むかどうかを判定します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | エイリアス | java.lang.String | AliasDictionary オブジェクト内で検索するエイリアスです。 |
|

**Returns:**
boolean - AliasDictionary オブジェクトが指定されたエイリアスを含む場合は true、そうでなければ false を返します。

### getText(String alias) {#getText-java.lang.String-}
```
public abstract String getText(String alias)
```


指定されたエイリアスに関連付けられたテキストを取得します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | エイリアス | java.lang.String | AliasDictionary オブジェクト内で検索するエイリアスです。 |
|

**Returns:**
java.lang.String - 指定されたエイリアスに関連付けられたテキスト、または null です。

### clear() {#clear--}
```
public abstract void clear()
```


AliasDictionary オブジェクトからすべてのエイリアスを削除します。


### iterator() {#iterator--}
```
public abstract Iterator<String> iterator()
```


コレクションを反復するイテレータを返します。


**Returns:**
java.util.Iterator<java.lang.String> - コレクションを反復するために使用できるイテレータ。

