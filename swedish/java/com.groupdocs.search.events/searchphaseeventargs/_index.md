---
title: "SearchPhaseEventArgs"
second_title: "GroupDocs.Search för Java API-referens"
description: "Representerar argument för händelser när sökfasen ändras."
type: docs
weight: 21
url: /sv/java/com.groupdocs.search.events/searchphaseeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class SearchPhaseEventArgs extends BaseIndexEventArgs
```

Representerar argument för händelser när sökfasen ändras.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getSearchPhase()](#getSearchPhase--) | Hämtar sökfasen. |
|
|  | [getQuery()](#getQuery--) | Hämtar den initiala frågan för den aktuella sökningen. |
|
|  | [getWords()](#getWords--) | Hämtar orden som erhålls i den aktuella fasen. |
|
### getSearchPhase() {#getSearchPhase--}
```
public final SearchPhase getSearchPhase()
```


Hämtar sökfasen.


**Returns:**
[SearchPhase](../../com.groupdocs.search.events/searchphase) - The search phase.

### getQuery() {#getQuery--}
```
public final String getQuery()
```


Hämtar den initiala frågan för den aktuella sökningen.


**Returns:**
java.lang.String - Den initiala frågan för den aktuella sökningen.

### getWords() {#getWords--}
```
public final String[] getWords()
```


Hämtar orden som erhålls i den aktuella fasen.


**Returns:**
java.lang.String[] - Orden som erhålls i den aktuella fasen.

