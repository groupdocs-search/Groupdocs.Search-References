---
title: "CharacterReplacementDictionary"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "インデックス作成プロセスで使用される文字置換辞書のインターフェイスを定義します。"
type: docs
weight: 16
url: /ja/java/com.groupdocs.search.dictionaries/characterreplacementdictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface CharacterReplacementDictionary extends DictionaryBase, Iterable<Character>
```

インデックス作成プロセスで使用される文字置換辞書のインターフェイスを定義します。文字置換は、例えばアクセント付き文字からアクセントを除去したり、大文字小文字を区別しないインデックスを作成したりするために使用できます。


**Learn more**

* [Character replacement during Indexing](../https://docs.groupdocs.com/display/searchjava/Character+replacement+during+Indexing)
* [Managing character replacements](../https://docs.groupdocs.com/display/searchjava/Character+replacements)

## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getCount()](#getCount--) | この CharacterReplacementDictionary に含まれる文字数を取得します。 |
|
|  | [addRange(Iterable<CharacterReplacementPair> characterReplacements)](#addRange-java.lang.Iterable-com.groupdocs.search.dictionaries.CharacterReplacementPair--) | 指定された文字置換のコレクションをこの CharacterReplacementDictionary インスタンスに追加します。 |
|
|  | [addRange(CharacterReplacementPair[] characterReplacements)](#addRange-com.groupdocs.search.dictionaries.CharacterReplacementPair---) | 指定された文字置換のコレクションをこの CharacterReplacementDictionary インスタンスに追加します。 |
|
|  | [removeRange(char[] characters)](#removeRange-char---) | 指定された文字置換のコレクションをこの CharacterReplacementDictionary インスタンスから削除します。 |
|
|  | [contains(char character)](#contains-char-) | CharacterReplacementDictionary オブジェクトが指定された文字の置換を含むかどうかを判断します。 |
|
|  | [getReplacement(char character)](#getReplacement-char-) | 指定された文字の置換を取得します。 |
|
|  | [clear()](#clear--) | CharacterReplacementDictionary オブジェクトからすべての文字置換を削除します。 |
|
|  | [iterator()](#iterator--) | コレクションを反復するイテレータを返します。 |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


この CharacterReplacementDictionary に含まれる文字数を取得します。


**Returns:**
int - 辞書内の文字数。

### addRange(Iterable<CharacterReplacementPair> characterReplacements) {#addRange-java.lang.Iterable-com.groupdocs.search.dictionaries.CharacterReplacementPair--}
```
public abstract void addRange(Iterable<CharacterReplacementPair> characterReplacements)
```


指定された文字置換のコレクションをこの CharacterReplacementDictionary インスタンスに追加します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | characterReplacements | java.lang.Iterable<com.groupdocs.search.dictionaries.CharacterReplacementPair> | 辞書に追加する文字置換のコレクション。 |
|

### addRange(CharacterReplacementPair[] characterReplacements) {#addRange-com.groupdocs.search.dictionaries.CharacterReplacementPair---}
```
public abstract void addRange(CharacterReplacementPair[] characterReplacements)
```


指定された文字置換のコレクションをこの CharacterReplacementDictionary インスタンスに追加します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | characterReplacements | [CharacterReplacementPair\[\]](../../com.groupdocs.search.dictionaries/characterreplacementpair) | 辞書に追加する文字置換のコレクション。 |
|

### removeRange(char[] characters) {#removeRange-char---}
```
public abstract void removeRange(char[] characters)
```


指定された文字置換のコレクションをこの CharacterReplacementDictionary インスタンスから削除します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 文字 | char[] | 削除する文字のコレクション。 |
|

### contains(char character) {#contains-char-}
```
public abstract boolean contains(char character)
```


CharacterReplacementDictionary オブジェクトが指定された文字の置換を含むかどうかを判断します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 文字 | char | CharacterReplacementDictionary オブジェクトで検索する文字。 |
|

**Returns:**
boolean - CharacterReplacementDictionary オブジェクトが指定された文字を含む場合は true、そうでない場合は false。

### getReplacement(char character) {#getReplacement-char-}
```
public abstract char getReplacement(char character)
```


指定された文字の置換を取得します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 文字 | char | 置換対象の文字。 |
|

**Returns:**
char - 指定された文字の置換。

### clear() {#clear--}
```
public abstract void clear()
```


CharacterReplacementDictionary オブジェクトからすべての文字置換を削除します。


### iterator() {#iterator--}
```
public abstract Iterator<Character> iterator()
```


コレクションを反復するイテレータを返します。


**Returns:**
java.util.Iterator<java.lang.Character> - コレクションを反復処理できるイテレータ。

