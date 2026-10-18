---
title: "SpellingCorrector"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "クエリ内の用語のスペル補正機能のインターフェイスを定義します。"
type: docs
weight: 21
url: /ja/java/com.groupdocs.search.dictionaries/spellingcorrector/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase)
```
public interface SpellingCorrector extends DictionaryBase
```

クエリ内の用語のスペル補正機能のインターフェイスを定義します。


**Learn more**

* [Spell checking](../https://docs.groupdocs.com/display/searchjava/Spell+checking)
* [Managing spelling corrector](../https://docs.groupdocs.com/display/searchjava/Spelling+corrector)

## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getCount()](#getCount--) | この SpellingCorrector に含まれる単語数を取得します。 |
|
|  | [getWords()](#getWords--) | この SpellingCorrector に現在含まれている単語のコレクションを取得します。 |
|
|  | [addRange(Iterable<String> words)](#addRange-java.lang.Iterable-java.lang.String--) | 指定された単語のコレクションをこの SpellingCorrector インスタンスに追加します。 |
|
|  | [addRange(String[] words)](#addRange-java.lang.String---) | 指定された単語のコレクションをこの SpellingCorrector インスタンスに追加します。 |
|
|  | [clear()](#clear--) | SpellingCorrector オブジェクトからすべての単語を削除します。 |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


この SpellingCorrector に含まれる単語数を取得します。


**Returns:**
int - この SpellingCorrector に含まれる単語数。

### getWords() {#getWords--}
```
public abstract String[] getWords()
```


この SpellingCorrector に現在含まれている単語のコレクションを取得します。


**Returns:**
java.lang.String[] - 単語のコレクション。

### addRange(Iterable<String> words) {#addRange-java.lang.Iterable-java.lang.String--}
```
public abstract void addRange(Iterable<String> words)
```


指定された単語のコレクションをこの SpellingCorrector インスタンスに追加します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 単語 | java.lang.Iterable<java.lang.String> | 辞書に追加する単語のコレクション。 |
|

### addRange(String[] words) {#addRange-java.lang.String---}
```
public abstract void addRange(String[] words)
```


指定された単語のコレクションをこの SpellingCorrector インスタンスに追加します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 単語 | java.lang.String[] | 辞書に追加する単語のコレクション。 |
|

### clear() {#clear--}
```
public abstract void clear()
```


SpellingCorrector オブジェクトからすべての単語を削除します。


