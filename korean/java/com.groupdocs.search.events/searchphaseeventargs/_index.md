---
title: "SearchPhaseEventArgs"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "검색 단계 변경 이벤트에 대한 인수를 나타냅니다."
type: docs
weight: 21
url: /ko/java/com.groupdocs.search.events/searchphaseeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class SearchPhaseEventArgs extends BaseIndexEventArgs
```

검색 단계 변경 이벤트에 대한 인수를 나타냅니다.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getSearchPhase()](#getSearchPhase--) | 검색 단계를 가져옵니다. |
|
|  | [getQuery()](#getQuery--) | 현재 검색의 초기 쿼리를 가져옵니다. |
|
|  | [getWords()](#getWords--) | 현재 단계에서 얻은 단어들을 가져옵니다. |
|
### getSearchPhase() {#getSearchPhase--}
```
public final SearchPhase getSearchPhase()
```


검색 단계를 가져옵니다.


**Returns:**
[SearchPhase](../../com.groupdocs.search.events/searchphase) - The search phase.

### getQuery() {#getQuery--}
```
public final String getQuery()
```


현재 검색의 초기 쿼리를 가져옵니다.


**Returns:**
java.lang.String - 현재 검색의 초기 쿼리.

### getWords() {#getWords--}
```
public final String[] getWords()
```


현재 단계에서 얻은 단어들을 가져옵니다.


**Returns:**
java.lang.String[] - 현재 단계에서 얻은 단어들.

