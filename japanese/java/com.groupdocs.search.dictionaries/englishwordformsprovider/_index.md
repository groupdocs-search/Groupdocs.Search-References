---
title: "EnglishWordFormsProvider"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "英語の語形提供者を表します。"
type: docs
weight: 13
url: /ja/java/com.groupdocs.search.dictionaries/englishwordformsprovider/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.IWordFormsProvider](../../com.groupdocs.search.dictionaries/iwordformsprovider)
```
public class EnglishWordFormsProvider implements IWordFormsProvider
```

英語の語形提供者を表します。


**Learn more**

* [Search for different word forms](../https://docs.groupdocs.com/display/searchjava/Search+for+different+word+forms)
* [Word forms provider](../https://docs.groupdocs.com/display/searchjava/Word+forms+provider)

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [EnglishWordFormsProvider()](#EnglishWordFormsProvider--) | 新しいインスタンスを初期化します |
EnglishWordFormsProvider
クラス。
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getWordForms(String word)](#getWordForms-java.lang.String-) | 指定された単語の語形を取得します。 |
|
### EnglishWordFormsProvider() {#EnglishWordFormsProvider--}
```
public EnglishWordFormsProvider()
```


新しいインスタンスを初期化します
EnglishWordFormsProvider
クラス。


### getWordForms(String word) {#getWordForms-java.lang.String-}
```
public final String[] getWordForms(String word)
```


指定された単語の語形を取得します。
結果の配列には元の単語は含まれません。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 単語 | java.lang.String | 語形を提案する単語。 |
|

**Returns:**
java.lang.String[] - 指定された単語の語形変化形、または IWordFormsProvider が指定された単語の語形変化形を提供しない場合は空配列です。

