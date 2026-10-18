---
title: "StopWordDictionary"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "ストップワード辞書のインターフェイスを定義します。"
type: docs
weight: 22
url: /ja/java/com.groupdocs.search.dictionaries/stopworddictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface StopWordDictionary extends DictionaryBase, Iterable<String>
```

ストップワード辞書のインターフェイスを定義します。


**Learn more**

* [Indexing with stop words](../https://docs.groupdocs.com/display/searchjava/Indexing+with+stop+words)
* [Managing stop word dictionary](../https://docs.groupdocs.com/display/searchjava/Stop+word+dictionary)

## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getCount()](#getCount--) | StopWordDictionary に含まれるストップワードの数を取得します。 |
|
|  | [addRange(Iterable<String> words)](#addRange-java.lang.Iterable-java.lang.String--) | 指定された単語のコレクションをこの StopWordDictionary インスタンスに追加します。 |
|
|  | [addRange(String[] words)](#addRange-java.lang.String---) | 指定された単語のコレクションをこの StopWordDictionary インスタンスに追加します。 |
|
|  | [removeRange(Iterable<String> words)](#removeRange-java.lang.Iterable-java.lang.String--) | 指定された単語のコレクションをこの StopWordDictionary インスタンスから削除します。 |
|
|  | [removeRange(String[] words)](#removeRange-java.lang.String---) | 指定された単語のコレクションをこの StopWordDictionary インスタンスから削除します。 |
|
|  | [contains(String word)](#contains-java.lang.String-) | StopWordDictionary オブジェクトが指定された単語を含むかどうかを判定します。 |
|
|  | [clear()](#clear--) | StopWordDictionary オブジェクトからすべての単語を削除します。 |
|
|  | [iterator()](#iterator--) | コレクションを反復するイテレータを返します。 |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


StopWordDictionary に含まれるストップワードの数を取得します。


**Returns:**
int - 辞書内のストップワードの数。

### addRange(Iterable<String> words) {#addRange-java.lang.Iterable-java.lang.String--}
```
public abstract void addRange(Iterable<String> words)
```


指定された単語のコレクションをこの StopWordDictionary インスタンスに追加します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 単語 | java.lang.Iterable<java.lang.String> | 辞書に追加する単語のコレクション。 |
|

### addRange(String[] words) {#addRange-java.lang.String---}
```
public abstract void addRange(String[] words)
```


指定された単語のコレクションをこの StopWordDictionary インスタンスに追加します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 単語 | java.lang.String[] | 辞書に追加する単語のコレクション。 |
|

### removeRange(Iterable<String> words) {#removeRange-java.lang.Iterable-java.lang.String--}
```
public abstract void removeRange(Iterable<String> words)
```


指定された単語のコレクションをこの StopWordDictionary インスタンスから削除します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 単語 | java.lang.Iterable<java.lang.String> | 削除する単語のコレクション。 |
|

### removeRange(String[] words) {#removeRange-java.lang.String---}
```
public abstract void removeRange(String[] words)
```


指定された単語のコレクションをこの StopWordDictionary インスタンスから削除します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 単語 | java.lang.String[] | 削除する単語のコレクション。 |
|

### contains(String word) {#contains-java.lang.String-}
```
public abstract boolean contains(String word)
```


StopWordDictionary オブジェクトが指定された単語を含むかどうかを判定します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 単語 | java.lang.String | StopWordDictionary オブジェクト内で検索する単語。 |
|

**Returns:**
boolean - StopWordDictionary オブジェクトが指定された単語を含む場合は true、そうでない場合は false。

### clear() {#clear--}
```
public abstract void clear()
```


StopWordDictionary オブジェクトからすべての単語を削除します。


### iterator() {#iterator--}
```
public abstract Iterator<String> iterator()
```


コレクションを反復するイテレータを返します。


**Returns:**
java.util.Iterator<java.lang.String> - コレクションを反復するために使用できるイテレータ。

