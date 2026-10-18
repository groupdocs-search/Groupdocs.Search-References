---
title: "HighlightOptions"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "見つかった用語のハイライトオプションを提供します。"
type: docs
weight: 22
url: /ja/java/com.groupdocs.search.options/highlightoptions/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.options.TextOptions](../../com.groupdocs.search.options/textoptions)

**All Implemented Interfaces:**
[com.groupdocs.search.options.IHighlightOptions](../../com.groupdocs.search.options/ihighlightoptions)
```
public class HighlightOptions extends TextOptions implements IHighlightOptions
```

見つかった用語のハイライトオプションを提供します。


**Learn more**

* [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [HighlightOptions()](#HighlightOptions--) | HighlightOptions クラスの新しいインスタンスを初期化します。 |
|
|  | [HighlightOptions(Object data)](#HighlightOptions-java.lang.Object-) | TextOptions クラスの新しいインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getTermsBefore()](#getTermsBefore--) | ハイライトされた単語の前にあるテキストスニペットの最大単語数を取得します。 |
|
|  | [setTermsBefore(int value)](#setTermsBefore-int-) | ハイライトされた単語の前にあるテキストスニペットの最大単語数を設定します。 |
|
|  | [getTermsAfter()](#getTermsAfter--) | ハイライトされた単語の後にあるテキストスニペットの最大単語数を取得します。 |
|
|  | [setTermsAfter(int value)](#setTermsAfter-int-) | ハイライトされた単語の後にあるテキストスニペットの最大単語数を設定します。 |
|
|  | [getTermsTotal()](#getTermsTotal--) | テキストスニペットの最大単語数を取得します。 |
|
|  | [setTermsTotal(int value)](#setTermsTotal-int-) | テキストスニペットの最大単語数を設定します。 |
|
|  | [getUseInlineStyles()](#getUseInlineStyles--) | インラインスタイルが出現箇所のハイライトに使用されているかどうかを示す値を取得します。 |
|
|  | [setUseInlineStyles(boolean value)](#setUseInlineStyles-boolean-) | インラインスタイルが出現箇所のハイライトに使用されているかどうかを示す値を設定します。 |
|
|  | [getHighlightColor()](#getHighlightColor--) | 出現箇所のハイライトに使用される色を取得します。 |
|
|  | [setHighlightColor(Color value)](#setHighlightColor-com.groupdocs.search.options.Color-) | 出現箇所のハイライトに使用される色を設定します。 |
|
|  | [getTermHighlightStartTag()](#getTermHighlightStartTag--) | 見つかった単語のハイライト開始タグを取得します。 |
|
|  | [setTermHighlightStartTag(String value)](#setTermHighlightStartTag-java.lang.String-) | 見つかった単語のハイライト開始タグを設定します。 |
|
|  | [getTermHighlightEndTag()](#getTermHighlightEndTag--) | 見つかった単語のハイライト終了タグを取得します。 |
|
|  | [setTermHighlightEndTag(String value)](#setTermHighlightEndTag-java.lang.String-) | 見つかった単語のハイライト終了タグを設定します。 |
|
### HighlightOptions() {#HighlightOptions--}
```
public HighlightOptions()
```


HighlightOptions クラスの新しいインスタンスを初期化します。


### HighlightOptions(Object data) {#HighlightOptions-java.lang.Object-}
```
public HighlightOptions(Object data)
```


TextOptions クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | データ | java.lang.Object | シリアライズされたデータ。 |
|

### getTermsBefore() {#getTermsBefore--}
```
public int getTermsBefore()
```


ハイライトされた単語の前にあるテキストスニペットの最大単語数を取得します。値は 0 から 10000 の範囲である必要があります。デフォルト値は 7 です。


**Returns:**
int - ハイライトされた単語の前にあるテキストスニペットの最大単語数。

### setTermsBefore(int value) {#setTermsBefore-int-}
```
public void setTermsBefore(int value)
```


ハイライトされた単語の前にあるテキストスニペットの最大単語数を設定します。値は 0 から 10000 の範囲である必要があります。デフォルト値は 7 です。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 値 | int | ハイライトされた単語の前にあるテキストスニペットの最大単語数。 |
|

### getTermsAfter() {#getTermsAfter--}
```
public int getTermsAfter()
```


ハイライトされた単語の後にあるテキストスニペットの最大単語数を取得します。値は 0 から 10000 の範囲である必要があります。デフォルト値は 7 です。


**Returns:**
int - ハイライトされた単語の後にあるテキストスニペットの最大単語数。

### setTermsAfter(int value) {#setTermsAfter-int-}
```
public void setTermsAfter(int value)
```


ハイライトされた単語の後にあるテキストスニペットの最大単語数を設定します。値は 0 から 10000 の範囲である必要があります。デフォルト値は 7 です。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 値 | int | ハイライトされた単語の後にあるテキストスニペットの最大単語数。 |
|

### getTermsTotal() {#getTermsTotal--}
```
public int getTermsTotal()
```


テキストスニペットの最大単語数を取得します。値は 0 から 10000 の範囲である必要があります。デフォルト値は 21 です。


**Returns:**
int - テキストスニペットの最大単語数。

### setTermsTotal(int value) {#setTermsTotal-int-}
```
public void setTermsTotal(int value)
```


テキストスニペットの最大単語数を設定します。値は 0 から 10000 の範囲である必要があります。デフォルト値は 21 です。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 値 | int | テキストスニペットの最大単語数。 |
|

### getUseInlineStyles() {#getUseInlineStyles--}
```
public boolean getUseInlineStyles()
```


インラインスタイルが出現箇所のハイライトに使用されるかどうかを示す値を取得します。デフォルト値は true です。


**Returns:**
boolean - インラインスタイルが出現箇所のハイライトに使用されるかどうかを示す値。

### setUseInlineStyles(boolean value) {#setUseInlineStyles-boolean-}
```
public void setUseInlineStyles(boolean value)
```


インラインスタイルが出現箇所のハイライトに使用されるかどうかを示す値を設定します。デフォルト値は true です。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 値 | boolean | インラインスタイルが出現箇所のハイライトに使用されるかどうかを示す値。 |
|

### getHighlightColor() {#getHighlightColor--}
```
public Color getHighlightColor()
```


出現箇所のハイライトに使用される色を取得します。デフォルト値は #FFD800 です。


**Returns:**
[Color](../../com.groupdocs.search.options/color) - A color that is used to highlight occurrences.

### setHighlightColor(Color value) {#setHighlightColor-com.groupdocs.search.options.Color-}
```
public void setHighlightColor(Color value)
```


出現箇所のハイライトに使用される色を設定します。デフォルト値は #FFD800 です。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | value | [Color](../../com.groupdocs.search.options/color) | 出現箇所のハイライトに使用される色。 |
|

### getTermHighlightStartTag() {#getTermHighlightStartTag--}
```
public String getTermHighlightStartTag()
```


見つかった単語のハイライト開始タグを取得します。このタグはプレーンテキストでハイライトする場合にのみ使用されます。デフォルト値は空文字列です。


**Returns:**
java.lang.String - 見つかった単語のハイライト開始タグ。

### setTermHighlightStartTag(String value) {#setTermHighlightStartTag-java.lang.String-}
```
public void setTermHighlightStartTag(String value)
```


見つかった単語のハイライト開始タグを設定します。このタグはプレーンテキストでハイライトする場合にのみ使用されます。デフォルト値は空文字列です。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 値 | java.lang.String | 見つかった単語のハイライト開始タグ。 |
|

### getTermHighlightEndTag() {#getTermHighlightEndTag--}
```
public String getTermHighlightEndTag()
```


見つかった単語のハイライト終了タグを取得します。このタグはプレーンテキストでハイライトする場合にのみ使用されます。デフォルト値は空文字列です。


**Returns:**
java.lang.String - 見つかった単語のハイライト終了タグ。

### setTermHighlightEndTag(String value) {#setTermHighlightEndTag-java.lang.String-}
```
public void setTermHighlightEndTag(String value)
```


見つかった単語のハイライトの終了タグを設定します。このタグはプレーンテキストでハイライトする場合にのみ使用されます。デフォルト値は空文字列です。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 値 | java.lang.String | 見つかった単語のハイライトの終了タグ。 |
|

