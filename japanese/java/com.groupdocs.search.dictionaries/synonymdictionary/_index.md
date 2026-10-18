---
title: "SynonymDictionary"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "同義語辞書のインターフェイスを定義します。"
type: docs
weight: 23
url: /ja/java/com.groupdocs.search.dictionaries/synonymdictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface SynonymDictionary extends DictionaryBase, Iterable<String>
```

同義語辞書のインターフェイスを定義します。


**Learn more**

* [Synonym search](../https://docs.groupdocs.com/display/searchjava/Synonym+search)
* [Managing synonym dictionary](../https://docs.groupdocs.com/display/searchjava/Synonym+dictionary)

## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getCount()](#getCount--) | この SynonymDictionary に含まれる単語数を取得します。 |
|
|  | [addRange(Iterable<String[]> synonyms)](#addRange-java.lang.Iterable-java.lang.String----) | 指定された同義語グループのコレクションをこの SynonymDictionary のインスタンスに追加します。 |
|
|  | [addRange(String[][] synonyms)](#addRange-java.lang.String-----) | 指定された同義語グループのコレクションをこの SynonymDictionary のインスタンスに追加します。 |
|
|  | [clear()](#clear--) | この SynonymDictionary オブジェクトからすべての単語を削除します。 |
|
|  | [getSynonyms(String word)](#getSynonyms-java.lang.String-) | 指定された単語の同義語を取得します。 |
|
|  | [getSynonymGroups(String word)](#getSynonymGroups-java.lang.String-) | 指定された単語が属するすべての同義語グループを取得します。 |
|
|  | [getAllSynonymGroups()](#getAllSynonymGroups--) | この辞書に含まれるすべての同義語グループを取得します。 |
|
|  | [iterator()](#iterator--) | コレクションを反復するイテレータを返します。 |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


この SynonymDictionary に含まれる単語数を取得します。


**Returns:**
int - この SynonymDictionary に含まれる単語数。

### addRange(Iterable<String[]> synonyms) {#addRange-java.lang.Iterable-java.lang.String----}
```
public abstract void addRange(Iterable<String[]> synonyms)
```


指定された同義語グループのコレクションをこの SynonymDictionary のインスタンスに追加します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 同義語 | java.lang.Iterable<java.lang.String[]> | 辞書に追加する同義語グループのコレクション。 |
|

### addRange(String[][] synonyms) {#addRange-java.lang.String-----}
```
public abstract void addRange(String[][] synonyms)
```


指定された同義語グループのコレクションをこの SynonymDictionary のインスタンスに追加します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 同義語 | java.lang.String[][] | 辞書に追加する同義語グループのコレクション。 |
|

### clear() {#clear--}
```
public abstract void clear()
```


この SynonymDictionary オブジェクトからすべての単語を削除します。


### getSynonyms(String word) {#getSynonyms-java.lang.String-}
```
public abstract String[] getSynonyms(String word)
```


指定された単語の同義語を取得します。結果の配列には元の単語は含まれません。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 単語 | java.lang.String | 同義語を提案する単語。 |
|

**Returns:**
java.lang.String[] - 指定された単語の同義語、または SynonymDictionary オブジェクトに指定された単語が含まれていない場合は空の配列。

### getSynonymGroups(String word) {#getSynonymGroups-java.lang.String-}
```
public abstract String[][] getSynonymGroups(String word)
```


指定された単語が属するすべての同義語グループを取得します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 単語 | java.lang.String | 同義語グループを取得する単語。 |
|

**Returns:**
java.lang.String[][] - 指定された単語が属するすべての同義語グループ。

### getAllSynonymGroups() {#getAllSynonymGroups--}
```
public abstract String[][] getAllSynonymGroups()
```


この辞書に含まれるすべての同義語グループを取得します。


**Returns:**
java.lang.String[][] - すべての同義語グループ。

### iterator() {#iterator--}
```
public abstract Iterator<String> iterator()
```


コレクションを反復するイテレータを返します。


**Returns:**
java.util.Iterator<java.lang.String> - コレクションを反復するために使用できるイテレータ。

