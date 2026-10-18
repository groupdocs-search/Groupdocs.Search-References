---
title: "WordPattern"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "単語ワイルドカード検索で使用する単語パターンを表します。"
type: docs
weight: 34
url: /ja/java/com.groupdocs.search.common/wordpattern/
---
**Inheritance:**
java.lang.Object
```
public class WordPattern
```

単語ワイルドカード検索で使用する単語パターンを表します。


**Learn more**

* [Wildcard search](../https://docs.groupdocs.com/display/searchjava/Wildcard+search)
* [Phrase search](../https://docs.groupdocs.com/display/searchjava/Phrase+search)

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [WordPattern()](#WordPattern--) | WordPattern クラスの新しいインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [appendString(String text)](#appendString-java.lang.String-) | 文字列を word pattern に追加します。 |
|
|  | [appendCharacter(char character)](#appendCharacter-char-) | 文字を word pattern に追加します。 |
|
|  | [appendOneCharacterWildcard()](#appendOneCharacterWildcard--) | 1 文字のワイルドカードを word pattern に追加します。 |
|
|  | [appendZeroOrOneCharacterWildcard()](#appendZeroOrOneCharacterWildcard--) | 0 または 1 文字のワイルドカードを word pattern に追加します。 |
|
|  | [appendZeroOrMoreCharactersWildcard()](#appendZeroOrMoreCharactersWildcard--) | 0 個以上の文字のワイルドカードを word pattern に追加します。 |
|
|  | [appendOneOrMoreCharactersWildcard()](#appendOneOrMoreCharactersWildcard--) | 1 個以上の文字のワイルドカードを word pattern に追加します。 |
|
|  | [appendWildcard(int min, int max)](#appendWildcard-int-int-) | ワイルドカードを word pattern に追加します。 |
|
|  | [toString()](#toString--) | 現在の WordPattern を表す System.String を返します。 |
|
| [getCore()](#getCore--) |  |
### WordPattern() {#WordPattern--}
```
public WordPattern()
```


WordPattern クラスの新しいインスタンスを初期化します。


### appendString(String text) {#appendString-java.lang.String-}
```
public void appendString(String text)
```


文字列を word pattern に追加します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | テキスト | java.lang.String | 追加する文字列。 |
|

### appendCharacter(char character) {#appendCharacter-char-}
```
public void appendCharacter(char character)
```


文字を word pattern に追加します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 文字 | char | 追加する文字。 |
|

### appendOneCharacterWildcard() {#appendOneCharacterWildcard--}
```
public void appendOneCharacterWildcard()
```


1 文字のワイルドカードを word pattern に追加します。


### appendZeroOrOneCharacterWildcard() {#appendZeroOrOneCharacterWildcard--}
```
public void appendZeroOrOneCharacterWildcard()
```


0 または 1 文字のワイルドカードを word pattern に追加します。


### appendZeroOrMoreCharactersWildcard() {#appendZeroOrMoreCharactersWildcard--}
```
public void appendZeroOrMoreCharactersWildcard()
```


0 個以上の文字のワイルドカードを word pattern に追加します。


### appendOneOrMoreCharactersWildcard() {#appendOneOrMoreCharactersWildcard--}
```
public void appendOneOrMoreCharactersWildcard()
```


1 個以上の文字のワイルドカードを word pattern に追加します。


### appendWildcard(int min, int max) {#appendWildcard-int-int-}
```
public void appendWildcard(int min, int max)
```


ワイルドカードを word pattern に追加します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | min | int | 文字数の最小値。 |
|
|  | max | int | 文字数の最大値。 |
|

### toString() {#toString--}
```
public String toString()
```


現在の WordPattern を表す System.String を返します。


**Returns:**
java.lang.String - 現在の WordPattern を表す System.String

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
