---
title: "SearchPhaseEventArgs"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Stellt Argumente für die Ereignisse zur Änderung der Suchphase dar."
type: docs
weight: 21
url: /de/java/com.groupdocs.search.events/searchphaseeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class SearchPhaseEventArgs extends BaseIndexEventArgs
```

Stellt Argumente für die Ereignisse zur Änderung der Suchphase dar.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getSearchPhase()](#getSearchPhase--) | Liefert die Suchphase. |
|
|  | [getQuery()](#getQuery--) | Liefert die Anfangsanfrage der aktuellen Suche. |
|
|  | [getWords()](#getWords--) | Liefert die in der aktuellen Phase erhaltenen Wörter. |
|
### getSearchPhase() {#getSearchPhase--}
```
public final SearchPhase getSearchPhase()
```


Liefert die Suchphase.


**Returns:**
[SearchPhase](../../com.groupdocs.search.events/searchphase) - The search phase.

### getQuery() {#getQuery--}
```
public final String getQuery()
```


Liefert die Anfangsanfrage der aktuellen Suche.


**Returns:**
java.lang.String - Die Anfangsanfrage der aktuellen Suche.

### getWords() {#getWords--}
```
public final String[] getWords()
```


Liefert die in der aktuellen Phase erhaltenen Wörter.


**Returns:**
java.lang.String[] - Die in der aktuellen Phase erhaltenen Wörter.

