---
title: "SearchPhase"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "検索フェーズを表します。"
type: docs
weight: 24
url: /ja/java/com.groupdocs.search.events/searchphase/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum SearchPhase extends Enum<SearchPhase>
```

検索フェーズを表します。

## Fields

| Field | 説明 |
| --- | --- |
|  | [AliasSubstitution](#AliasSubstitution) | エイリアス置換。 |
|
|  | [KeyboardLayoutCorrection](#KeyboardLayoutCorrection) | キーボードレイアウトの補正。 |
|
|  | [SpellingCorrection](#SpellingCorrection) | スペル補正。 |
|
|  | [HomophoneSearch](#HomophoneSearch) | 同音異義語検索。 |
|
|  | [SynonymSearch](#SynonymSearch) | 同義語検索。 |
|
|  | [WordFormsSearch](#WordFormsSearch) | 単語形検索。 |
|
|  | [FuzzySearch](#FuzzySearch) | あいまい検索。 |
|
|  | [WildcardMatching](#WildcardMatching) | ワイルドカードマッチング。 |
|
|  | [RegexMatching](#RegexMatching) | 正規表現マッチング。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### AliasSubstitution {#AliasSubstitution}
```
public static final SearchPhase AliasSubstitution
```


エイリアス置換。


### KeyboardLayoutCorrection {#KeyboardLayoutCorrection}
```
public static final SearchPhase KeyboardLayoutCorrection
```


キーボードレイアウトの補正。


### SpellingCorrection {#SpellingCorrection}
```
public static final SearchPhase SpellingCorrection
```


スペル補正。


### HomophoneSearch {#HomophoneSearch}
```
public static final SearchPhase HomophoneSearch
```


同音異義語検索。


### SynonymSearch {#SynonymSearch}
```
public static final SearchPhase SynonymSearch
```


同義語検索。


### WordFormsSearch {#WordFormsSearch}
```
public static final SearchPhase WordFormsSearch
```


単語形検索。


### FuzzySearch {#FuzzySearch}
```
public static final SearchPhase FuzzySearch
```


あいまい検索。


### WildcardMatching {#WildcardMatching}
```
public static final SearchPhase WildcardMatching
```


ワイルドカードマッチング。


### RegexMatching {#RegexMatching}
```
public static final SearchPhase RegexMatching
```


正規表現マッチング。


### values() {#values--}
```
public static SearchPhase[] values()
```




**Returns:**
com.groupdocs.search.events.SearchPhase[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static SearchPhase valueOf(String name)
```




**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[SearchPhase](../../com.groupdocs.search.events/searchphase)
