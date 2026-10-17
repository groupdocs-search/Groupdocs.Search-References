---
title: "SearchPhaseEventArgs"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "表示搜索阶段更改事件的参数。"
type: docs
weight: 21
url: /zh/java/com.groupdocs.search.events/searchphaseeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class SearchPhaseEventArgs extends BaseIndexEventArgs
```

表示搜索阶段更改事件的参数。


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getSearchPhase()](#getSearchPhase--) | 获取搜索阶段。 |
|
|  | [getQuery()](#getQuery--) | 获取当前搜索的初始查询。 |
|
|  | [getWords()](#getWords--) | 获取当前阶段获得的词。 |
|
### getSearchPhase() {#getSearchPhase--}
```
public final SearchPhase getSearchPhase()
```


获取搜索阶段。


**Returns:**
[SearchPhase](../../com.groupdocs.search.events/searchphase) - The search phase.

### getQuery() {#getQuery--}
```
public final String getQuery()
```


获取当前搜索的初始查询。


**Returns:**
java.lang.String - 当前搜索的初始查询。

### getWords() {#getWords--}
```
public final String[] getWords()
```


获取当前阶段获得的词。


**Returns:**
java.lang.String[] - 当前阶段获得的词。

