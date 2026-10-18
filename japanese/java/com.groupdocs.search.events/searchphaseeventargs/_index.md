---
title: "SearchPhaseEventArgs"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "検索フェーズ変更イベントの引数を表します。"
type: docs
weight: 21
url: /ja/java/com.groupdocs.search.events/searchphaseeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class SearchPhaseEventArgs extends BaseIndexEventArgs
```

検索フェーズ変更イベントの引数を表します。


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getSearchPhase()](#getSearchPhase--) | 検索フェーズを取得します。 |
|
|  | [getQuery()](#getQuery--) | 現在の検索の初期クエリを取得します。 |
|
|  | [getWords()](#getWords--) | 現在のフェーズで取得された単語を取得します。 |
|
### getSearchPhase() {#getSearchPhase--}
```
public final SearchPhase getSearchPhase()
```


検索フェーズを取得します。


**Returns:**
[SearchPhase](../../com.groupdocs.search.events/searchphase) - The search phase.

### getQuery() {#getQuery--}
```
public final String getQuery()
```


現在の検索の初期クエリを取得します。


**Returns:**
java.lang.String - 現在の検索の初期クエリ。

### getWords() {#getWords--}
```
public final String[] getWords()
```


現在のフェーズで取得された単語を取得します。


**Returns:**
java.lang.String[] - 現在のフェーズで取得された単語。

