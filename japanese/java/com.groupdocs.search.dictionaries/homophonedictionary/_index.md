---
title: "HomophoneDictionary"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "異形同音語辞書のインターフェイスを定義します。"
type: docs
weight: 18
url: /ja/java/com.groupdocs.search.dictionaries/homophonedictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface HomophoneDictionary extends DictionaryBase, Iterable<String>
```

異形同音語辞書のインターフェイスを定義します。


**Learn more**

* [Homophone search](../https://docs.groupdocs.com/display/searchjava/Homophone+search)
* [Managing homophone dictionary](../https://docs.groupdocs.com/display/searchjava/Homophone+dictionary)

## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getCount()](#getCount--) | この HomophoneDictionary に含まれる単語数を取得します。 |
|
|  | [addRange(Iterable<String[]> homophones)](#addRange-java.lang.Iterable-java.lang.String----) | 指定された同音語グループのコレクションをこの HomophoneDictionary のインスタンスに追加します。 |
|
|  | [addRange(String[][] homophones)](#addRange-java.lang.String-----) | 指定された同音語グループのコレクションをこの HomophoneDictionary のインスタンスに追加します。 |
|
|  | [clear()](#clear--) | HomophoneDictionary オブジェクトからすべての単語を削除します。 |
|
|  | [getHomophones(String word)](#getHomophones-java.lang.String-) | 指定された単語の同音語を取得します。 |
|
|  | [getHomophoneGroups(String word)](#getHomophoneGroups-java.lang.String-) | 指定された単語が属するすべての同音語グループを取得します。 |
|
|  | [getAllHomophoneGroups()](#getAllHomophoneGroups--) | この辞書に含まれるすべての同音語グループを取得します。 |
|
|  | [iterator()](#iterator--) | コレクションを反復するイテレータを返します。 |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


この HomophoneDictionary に含まれる単語数を取得します。


**Returns:**
int - 単語数。

### addRange(Iterable<String[]> homophones) {#addRange-java.lang.Iterable-java.lang.String----}
```
public abstract void addRange(Iterable<String[]> homophones)
```


指定された同音語グループのコレクションをこの HomophoneDictionary のインスタンスに追加します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 同音語 | java.lang.Iterable<java.lang.String[]> | 辞書に追加する同音語グループのコレクション。 |
|

### addRange(String[][] homophones) {#addRange-java.lang.String-----}
```
public abstract void addRange(String[][] homophones)
```


指定された同音語グループのコレクションをこの HomophoneDictionary のインスタンスに追加します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 同音語 | java.lang.String[][] | 辞書に追加する同音語グループのコレクション。 |
|

### clear() {#clear--}
```
public abstract void clear()
```


HomophoneDictionary オブジェクトからすべての単語を削除します。


### getHomophones(String word) {#getHomophones-java.lang.String-}
```
public abstract String[] getHomophones(String word)
```


指定された単語の同音語を取得します。結果の配列には元の単語は含まれません。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 単語 | java.lang.String | 同音語を提案する単語。 |
|

**Returns:**
java.lang.String[] - 指定された単語の同音語、または HomophoneDictionary オブジェクトが指定された単語を含まない場合は空の配列。

### getHomophoneGroups(String word) {#getHomophoneGroups-java.lang.String-}
```
public abstract String[][] getHomophoneGroups(String word)
```


指定された単語が属するすべての同音語グループを取得します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 単語 | java.lang.String | 同音語グループを取得するための単語。 |
|

**Returns:**
java.lang.String[][] - 指定された単語が属するすべての同音語グループ。

### getAllHomophoneGroups() {#getAllHomophoneGroups--}
```
public abstract String[][] getAllHomophoneGroups()
```


この辞書に含まれるすべての同音語グループを取得します。


**Returns:**
java.lang.String[][] - すべての同音語グループ。

### iterator() {#iterator--}
```
public abstract Iterator<String> iterator()
```


コレクションを反復するイテレータを返します。


**Returns:**
java.util.Iterator<java.lang.String> - コレクションを反復するために使用できるイテレータ。

