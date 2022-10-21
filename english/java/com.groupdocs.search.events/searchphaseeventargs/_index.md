---
title: SearchPhaseEventArgs
second_title: GroupDocs.Search for Java API Reference
description: Represents arguments for the search phase changing events.
type: docs
weight: 21
url: /java/com.groupdocs.search.events/searchphaseeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class SearchPhaseEventArgs extends BaseIndexEventArgs
```

Represents arguments for the search phase changing events.

**Learn more**

 *  [Search index events][]


[Search index events]: https://docs.groupdocs.com/display/searchjava/Search+index+events
## Methods

| Method | Description |
| --- | --- |
| [getSearchPhase()](#getSearchPhase--) | Gets the search phase. |
| [getQuery()](#getQuery--) | Gets the initial query of the current search. |
| [getWords()](#getWords--) | Gets the words obtained in the current phase. |
### getSearchPhase() {#getSearchPhase--}
```
public final SearchPhase getSearchPhase()
```


Gets the search phase.

**Returns:**
[SearchPhase](../../com.groupdocs.search.events/searchphase) - The search phase.
### getQuery() {#getQuery--}
```
public final String getQuery()
```


Gets the initial query of the current search.

**Returns:**
java.lang.String - The initial query of the current search.
### getWords() {#getWords--}
```
public final String[] getWords()
```


Gets the words obtained in the current phase.

**Returns:**
java.lang.String[] - The words obtained in the current phase.
