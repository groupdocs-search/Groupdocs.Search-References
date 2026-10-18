---
title: "DictionaryRepository"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "インデックス内のすべての辞書のリポジトリを表します。"
type: docs
weight: 12
url: /ja/java/com.groupdocs.search.dictionaries/dictionaryrepository/
---
**Inheritance:**
java.lang.Object
```
public abstract class DictionaryRepository
```

インデックス内のすべての辞書のリポジトリを表します。

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [DictionaryRepository()](#DictionaryRepository--) |  |
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getAliasDictionary()](#getAliasDictionary--) | エイリアスの辞書を取得します。 |
|
|  | [getStopWordDictionary()](#getStopWordDictionary--) | ストップワードの辞書を取得します。 |
|
|  | [getSynonymDictionary()](#getSynonymDictionary--) | 同義語の辞書を取得します。 |
|
|  | [getDocumentPasswords()](#getDocumentPasswords--) | 文書パスワードの辞書を取得します。 |
|
|  | [getSpellingCorrector()](#getSpellingCorrector--) | スペル補正機能を取得します。 |
|
|  | [getHomophoneDictionary()](#getHomophoneDictionary--) | 同音異義語の辞書を取得します。 |
|
|  | [getAlphabet()](#getAlphabet--) | 文字の辞書を取得します。 |
|
|  | [getCharacterReplacements()](#getCharacterReplacements--) | 文字置換の辞書を取得します。 |
|
|  | [getWordFormsProvider()](#getWordFormsProvider--) | 単語形態プロバイダーを取得します。 |
|
|  | [setWordFormsProvider(IWordFormsProvider value)](#setWordFormsProvider-com.groupdocs.search.dictionaries.IWordFormsProvider-) | 単語形態プロバイダーを設定します。 |
|
### DictionaryRepository() {#DictionaryRepository--}
```
public DictionaryRepository()
```


### getAliasDictionary() {#getAliasDictionary--}
```
public abstract AliasDictionary getAliasDictionary()
```


エイリアスの辞書を取得します。


**Returns:**
[AliasDictionary](../../com.groupdocs.search.dictionaries/aliasdictionary) - The dictionary of aliases.

### getStopWordDictionary() {#getStopWordDictionary--}
```
public abstract StopWordDictionary getStopWordDictionary()
```


ストップワードの辞書を取得します。


**Returns:**
[StopWordDictionary](../../com.groupdocs.search.dictionaries/stopworddictionary) - The dictionary of stop words.

### getSynonymDictionary() {#getSynonymDictionary--}
```
public abstract SynonymDictionary getSynonymDictionary()
```


同義語の辞書を取得します。


**Returns:**
[SynonymDictionary](../../com.groupdocs.search.dictionaries/synonymdictionary) - The dictionary of synonyms.

### getDocumentPasswords() {#getDocumentPasswords--}
```
public abstract PasswordDictionary getDocumentPasswords()
```


文書パスワードの辞書を取得します。


**Returns:**
[PasswordDictionary](../../com.groupdocs.search.dictionaries/passworddictionary) - The dictionary of document passwords.

### getSpellingCorrector() {#getSpellingCorrector--}
```
public abstract SpellingCorrector getSpellingCorrector()
```


スペル補正機能を取得します。


**Returns:**
[SpellingCorrector](../../com.groupdocs.search.dictionaries/spellingcorrector) - The spelling corrector.

### getHomophoneDictionary() {#getHomophoneDictionary--}
```
public abstract HomophoneDictionary getHomophoneDictionary()
```


同音異義語の辞書を取得します。


**Returns:**
[HomophoneDictionary](../../com.groupdocs.search.dictionaries/homophonedictionary) - The dictionary of homophones.

### getAlphabet() {#getAlphabet--}
```
public abstract Alphabet getAlphabet()
```


文字の辞書を取得します。


**Returns:**
[Alphabet](../../com.groupdocs.search.dictionaries/alphabet) - The dictionary of characters.

### getCharacterReplacements() {#getCharacterReplacements--}
```
public abstract CharacterReplacementDictionary getCharacterReplacements()
```


文字置換の辞書を取得します。


**Returns:**
[CharacterReplacementDictionary](../../com.groupdocs.search.dictionaries/characterreplacementdictionary) - The dictionary of character replacements.

### getWordFormsProvider() {#getWordFormsProvider--}
```
public abstract IWordFormsProvider getWordFormsProvider()
```


単語形態プロバイダーを取得します。


**Returns:**
[IWordFormsProvider](../../com.groupdocs.search.dictionaries/iwordformsprovider) - The word forms provider.

### setWordFormsProvider(IWordFormsProvider value) {#setWordFormsProvider-com.groupdocs.search.dictionaries.IWordFormsProvider-}
```
public abstract void setWordFormsProvider(IWordFormsProvider value)
```


単語形態プロバイダーを設定します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | value | [IWordFormsProvider](../../com.groupdocs.search.dictionaries/iwordformsprovider) | 単語形態プロバイダー。 |
|

