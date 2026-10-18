---
title: "アルファベット"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "インデックス作成時に文字種を検出するために使用される文字辞書のインターフェイスを定義します。"
type: docs
weight: 15
url: /ja/java/com.groupdocs.search.dictionaries/alphabet/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface Alphabet extends DictionaryBase, Iterable<Character>
```

インデックス作成時に文字種を検出するために使用される文字の辞書のインターフェイスを定義します。各文字は区切り文字、文字、またはその両方として扱うことができます。


**Learn more**

* [Character types](../https://docs.groupdocs.com/display/searchjava/Character+types)
* [Managing alphabet](../https://docs.groupdocs.com/display/searchjava/Alphabet)

## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getCharacterType(char character)](#getCharacterType-char-) | 文字のタイプを取得します。 |
|
|  | [getCount()](#getCount--) | Alphabet に含まれる文字数を取得します。 |
|
|  | [setRange(char[] characters, CharacterType type)](#setRange-char---com.groupdocs.search.dictionaries.CharacterType-) | この Alphabet インスタンス内の指定されたコレクションの各文字のタイプを設定します。 |
|
|  | [clear()](#clear--) | この Alphabet のすべての文字に CharacterType.Separator タイプを設定します。 |
|
|  | [iterator()](#iterator--) | コレクションを反復するイテレータを返します。 |
|
### getCharacterType(char character) {#getCharacterType-char-}
```
public abstract CharacterType getCharacterType(char character)
```


文字のタイプを取得します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 文字 | char | タイプを取得する文字。 |
|

**Returns:**
[CharacterType](../../com.groupdocs.search.dictionaries/charactertype) - A type of the character.

### getCount() {#getCount--}
```
public abstract int getCount()
```


Alphabet に含まれる文字数を取得します。


**Returns:**
int - 辞書内の文字数。

### setRange(char[] characters, CharacterType type) {#setRange-char---com.groupdocs.search.dictionaries.CharacterType-}
```
public abstract void setRange(char[] characters, CharacterType type)
```


この Alphabet インスタンス内の指定されたコレクションの各文字のタイプを設定します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 文字 | char[] | タイプを設定する文字のコレクション。 |
|
|  | type | [CharacterType](../../com.groupdocs.search.dictionaries/charactertype) | 文字タイプ。 |
|

### clear() {#clear--}
```
public abstract void clear()
```


この Alphabet のすべての文字に CharacterType.Separator タイプを設定します。


### iterator() {#iterator--}
```
public abstract Iterator<Character> iterator()
```


コレクションを反復するイテレータを返します。


**Returns:**
java.util.Iterator<java.lang.Character> - コレクションを反復処理できるイテレータ。

