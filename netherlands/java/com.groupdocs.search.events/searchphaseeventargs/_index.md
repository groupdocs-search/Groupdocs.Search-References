---
title: "SearchPhaseEventArgs"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Stelt de argumenten voor de zoekfase‑veranderings‑evenementen voor."
type: docs
weight: 21
url: /nl/java/com.groupdocs.search.events/searchphaseeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class SearchPhaseEventArgs extends BaseIndexEventArgs
```

Stelt de argumenten voor de zoekfase‑veranderings‑evenementen voor.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getSearchPhase()](#getSearchPhase--) | Haalt de zoekfase op. |
|
|  | [getQuery()](#getQuery--) | Haalt de initiële query van de huidige zoekopdracht op. |
|
|  | [getWords()](#getWords--) | Haalt de woorden op die in de huidige fase zijn verkregen. |
|
### getSearchPhase() {#getSearchPhase--}
```
public final SearchPhase getSearchPhase()
```


Haalt de zoekfase op.


**Returns:**
[SearchPhase](../../com.groupdocs.search.events/searchphase) - The search phase.

### getQuery() {#getQuery--}
```
public final String getQuery()
```


Haalt de initiële query van de huidige zoekopdracht op.


**Returns:**
java.lang.String - De initiële query van de huidige zoekopdracht.

### getWords() {#getWords--}
```
public final String[] getWords()
```


Haalt de woorden op die in de huidige fase zijn verkregen.


**Returns:**
java.lang.String[] - De woorden die in de huidige fase zijn verkregen.

