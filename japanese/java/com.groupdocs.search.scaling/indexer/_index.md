---
title: "Indexer"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "検索ネットワークのシャード間でインデックスされたドキュメントの配布を管理するサービスを表します。"
type: docs
weight: 10
url: /ja/java/com.groupdocs.search.scaling/indexer/
---
**Inheritance:**
java.lang.Object
```
public abstract class Indexer
```

検索ネットワークのシャード間でインデックスされたドキュメントの配布を管理するサービスを表します。

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [Indexer()](#Indexer--) |  |
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [add(Document[] documents, String[] passwords, IndexingOptions options)](#add-com.groupdocs.search.Document---java.lang.String---com.groupdocs.search.options.IndexingOptions-) | インデックス作成操作を実行します。 |
|
|  | [add(ExtractedData[] data, IndexingOptions options)](#add-com.groupdocs.search.ExtractedData---com.groupdocs.search.options.IndexingOptions-) | インデックス作成操作を実行します。 |
|
|  | [delete(String[] documentKeys, DeleteOptions options)](#delete-java.lang.String---com.groupdocs.search.options.DeleteOptions-) | インデックスされたドキュメントを削除します。 |
|
|  | [optimize(OptimizeOptions options)](#optimize-com.groupdocs.search.options.OptimizeOptions-) | インデックスセグメントの数を、セグメント同士をマージすることで最小化します。 |
|
|  | [synchronize(SynchronizeOptions options)](#synchronize-com.groupdocs.search.options.SynchronizeOptions-) | インデックスされたドキュメントのリストをシャード上のものと同期します。 |
|
|  | [changeAttributes(AttributeChangeBatch batch, ChangeAttributesOptions options)](#changeAttributes-com.groupdocs.search.common.AttributeChangeBatch-com.groupdocs.search.options.ChangeAttributesOptions-) | 再インデックス化せずに、指定された属性変更のバッチをインデックスされたドキュメントに適用します。 |
|
|  | [getAttributes(String documentKey)](#getAttributes-java.lang.String-) | 指定されたインデックス化ドキュメントに関連付けられたすべての属性を取得します。 |
|
|  | [getDictionary(DictionaryType dictionaryType, int shardIndex)](#getDictionary-com.groupdocs.search.dictionaries.DictionaryType-int-) | 指定されたシャードから辞書を取得します。 |
|
|  | [getAlphabet(int shardIndex)](#getAlphabet-int-) | アルファベット辞書を取得します。 |
|
|  | [getAliasDictionary(int shardIndex)](#getAliasDictionary-int-) | エイリアス辞書を取得します。 |
|
|  | [getCharacterReplacementDictionary(int shardIndex)](#getCharacterReplacementDictionary-int-) | 文字置換辞書を取得します。 |
|
|  | [getSynonymDictionary(int shardIndex)](#getSynonymDictionary-int-) | 同義語辞書を取得します。 |
|
|  | [getHomophoneDictionary(int shardIndex)](#getHomophoneDictionary-int-) | 同音異義語辞書を取得します。 |
|
|  | [getSpellingCorrector(int shardIndex)](#getSpellingCorrector-int-) | スペル補正辞書を取得します。 |
|
|  | [getStopWordDictionary(int shardIndex)](#getStopWordDictionary-int-) | ストップワード辞書を取得します。 |
|
|  | [getPasswordDictionary(int shardIndex)](#getPasswordDictionary-int-) | パスワード辞書を取得します。 |
|
|  | [setDictionary(DictionaryBase dictionary, int shardIndex)](#setDictionary-com.groupdocs.search.dictionaries.DictionaryBase-int-) | 指定されたシャードに辞書を設定します。 |
|
|  | [setDictionary(DictionaryBase dictionary)](#setDictionary-com.groupdocs.search.dictionaries.DictionaryBase-) | すべてのシャードに辞書を設定します。 |
|
|  | [deleteAllData()](#deleteAllData--) | 検索ネットワークのすべてのシャードからすべてのインデックスデータを削除します。 |
|
### Indexer() {#Indexer--}
```
public Indexer()
```


### add(Document[] documents, String[] passwords, IndexingOptions options) {#add-com.groupdocs.search.Document---java.lang.String---com.groupdocs.search.options.IndexingOptions-}
```
public abstract void add(Document[] documents, String[] passwords, IndexingOptions options)
```


インデックス作成操作を実行します。ストリームと構造からのインデックス作成のみがサポートされています。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | documents | [Document\[\]](../../com.groupdocs.search/document) | ファイルシステム、ストリーム、または構造からのドキュメント。 |
|
|  | パスワード | java.lang.String[] | ドキュメントのパスワード。 |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | 追加オプション。 |
|

### add(ExtractedData[] data, IndexingOptions options) {#add-com.groupdocs.search.ExtractedData---com.groupdocs.search.options.IndexingOptions-}
```
public abstract void add(ExtractedData[] data, IndexingOptions options)
```


インデックス作成操作を実行します。抽出されたデータを検索ネットワークに追加します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | data | [ExtractedData\[\]](../../com.groupdocs.search/extracteddata) | 抽出されたデータです。 |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | インデックスオプションです。 |
|

### delete(String[] documentKeys, DeleteOptions options) {#delete-java.lang.String---com.groupdocs.search.options.DeleteOptions-}
```
public abstract void delete(String[] documentKeys, DeleteOptions options)
```


インデックスされたドキュメントを削除します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | documentKeys | java.lang.String[] | ストリームまたは構造体から追加されたドキュメントのキー。 |
|
|  | options | [DeleteOptions](../../com.groupdocs.search.options/deleteoptions) | 削除オプション。 |
|

### optimize(OptimizeOptions options) {#optimize-com.groupdocs.search.options.OptimizeOptions-}
```
public abstract void optimize(OptimizeOptions options)
```


インデックスセグメントの数を相互にマージすることで最小化します。この操作は検索パフォーマンスを向上させます。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | options | [OptimizeOptions](../../com.groupdocs.search.options/optimizeoptions) | 最適化オプション。 |
|

### synchronize(SynchronizeOptions options) {#synchronize-com.groupdocs.search.options.SynchronizeOptions-}
```
public abstract void synchronize(SynchronizeOptions options)
```


インデックスされたドキュメントのリストをシャード上のものと同期します。この操作は、検索ネットワークノードとの通信問題に起因したインデックス作成やドキュメント削除の問題を修正します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | options | [SynchronizeOptions](../../com.groupdocs.search.options/synchronizeoptions) | 同期オプション。 |
|

### changeAttributes(AttributeChangeBatch batch, ChangeAttributesOptions options) {#changeAttributes-com.groupdocs.search.common.AttributeChangeBatch-com.groupdocs.search.options.ChangeAttributesOptions-}
```
public abstract void changeAttributes(AttributeChangeBatch batch, ChangeAttributesOptions options)
```


再インデックス化せずに、指定された属性変更のバッチをインデックスされたドキュメントに適用します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | batch | [AttributeChangeBatch](../../com.groupdocs.search.common/attributechangebatch) | 属性変更バッチ。 |
|
|  | options | [ChangeAttributesOptions](../../com.groupdocs.search.options/changeattributesoptions) | 属性変更オプション。 |
|

### getAttributes(String documentKey) {#getAttributes-java.lang.String-}
```
public abstract String[] getAttributes(String documentKey)
```


指定されたインデックス化ドキュメントに関連付けられたすべての属性を取得します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | documentKey | java.lang.String | ドキュメントキーです。 |
|

**Returns:**
java.lang.String[] - 指定されたインデックスドキュメントに関連付けられた属性。

### getDictionary(DictionaryType dictionaryType, int shardIndex) {#getDictionary-com.groupdocs.search.dictionaries.DictionaryType-int-}
```
public abstract DictionaryBase getDictionary(DictionaryType dictionaryType, int shardIndex)
```


指定されたシャードから辞書を取得します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | dictionaryType | [DictionaryType](../../com.groupdocs.search.dictionaries/dictionarytype) | 辞書の種類。 |
|
|  | shardIndex | int | シャードインデックス。 |
|

**Returns:**
[DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase) - The dictionary.

### getAlphabet(int shardIndex) {#getAlphabet-int-}
```
public abstract Alphabet getAlphabet(int shardIndex)
```


アルファベット辞書を取得します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | shardIndex | int | シャードインデックス。 |
|

**Returns:**
[Alphabet](../../com.groupdocs.search.dictionaries/alphabet) - The dictionary.

### getAliasDictionary(int shardIndex) {#getAliasDictionary-int-}
```
public abstract AliasDictionary getAliasDictionary(int shardIndex)
```


エイリアス辞書を取得します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | shardIndex | int | シャードインデックス。 |
|

**Returns:**
[AliasDictionary](../../com.groupdocs.search.dictionaries/aliasdictionary) - The dictionary.

### getCharacterReplacementDictionary(int shardIndex) {#getCharacterReplacementDictionary-int-}
```
public abstract CharacterReplacementDictionary getCharacterReplacementDictionary(int shardIndex)
```


文字置換辞書を取得します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | shardIndex | int | シャードインデックス。 |
|

**Returns:**
[CharacterReplacementDictionary](../../com.groupdocs.search.dictionaries/characterreplacementdictionary) - The dictionary.

### getSynonymDictionary(int shardIndex) {#getSynonymDictionary-int-}
```
public abstract SynonymDictionary getSynonymDictionary(int shardIndex)
```


同義語辞書を取得します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | shardIndex | int | シャードインデックス。 |
|

**Returns:**
[SynonymDictionary](../../com.groupdocs.search.dictionaries/synonymdictionary) - The dictionary.

### getHomophoneDictionary(int shardIndex) {#getHomophoneDictionary-int-}
```
public abstract HomophoneDictionary getHomophoneDictionary(int shardIndex)
```


同音異義語辞書を取得します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | shardIndex | int | シャードインデックス。 |
|

**Returns:**
[HomophoneDictionary](../../com.groupdocs.search.dictionaries/homophonedictionary) - The dictionary.

### getSpellingCorrector(int shardIndex) {#getSpellingCorrector-int-}
```
public abstract SpellingCorrector getSpellingCorrector(int shardIndex)
```


スペル補正辞書を取得します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | shardIndex | int | シャードインデックス。 |
|

**Returns:**
[SpellingCorrector](../../com.groupdocs.search.dictionaries/spellingcorrector) - The dictionary.

### getStopWordDictionary(int shardIndex) {#getStopWordDictionary-int-}
```
public abstract StopWordDictionary getStopWordDictionary(int shardIndex)
```


ストップワード辞書を取得します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | shardIndex | int | シャードインデックス。 |
|

**Returns:**
[StopWordDictionary](../../com.groupdocs.search.dictionaries/stopworddictionary) - The dictionary.

### getPasswordDictionary(int shardIndex) {#getPasswordDictionary-int-}
```
public abstract PasswordDictionary getPasswordDictionary(int shardIndex)
```


パスワード辞書を取得します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | shardIndex | int | シャードインデックス。 |
|

**Returns:**
[PasswordDictionary](../../com.groupdocs.search.dictionaries/passworddictionary) - The dictionary.

### setDictionary(DictionaryBase dictionary, int shardIndex) {#setDictionary-com.groupdocs.search.dictionaries.DictionaryBase-int-}
```
public abstract void setDictionary(DictionaryBase dictionary, int shardIndex)
```


指定されたシャードに辞書を設定します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | dictionary | [DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase) | 辞書。 |
|
|  | shardIndex | int | シャードインデックス。 |
|

### setDictionary(DictionaryBase dictionary) {#setDictionary-com.groupdocs.search.dictionaries.DictionaryBase-}
```
public abstract void setDictionary(DictionaryBase dictionary)
```


すべてのシャードに辞書を設定します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | dictionary | [DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase) | 辞書。 |
|

### deleteAllData() {#deleteAllData--}
```
public abstract void deleteAllData()
```


検索ネットワークのすべてのシャードからすべてのインデックスデータを削除します。


