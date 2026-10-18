---
title: "SearchPhaseEventArgs"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Rappresenta gli argomenti per gli eventi di cambiamento della fase di ricerca."
type: docs
weight: 21
url: /it/java/com.groupdocs.search.events/searchphaseeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class SearchPhaseEventArgs extends BaseIndexEventArgs
```

Rappresenta gli argomenti per gli eventi di cambiamento della fase di ricerca.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getSearchPhase()](#getSearchPhase--) | Ottiene la fase di ricerca. |
|
|  | [getQuery()](#getQuery--) | Ottiene la query iniziale della ricerca corrente. |
|
|  | [getWords()](#getWords--) | Ottiene le parole ottenute nella fase corrente. |
|
### getSearchPhase() {#getSearchPhase--}
```
public final SearchPhase getSearchPhase()
```


Ottiene la fase di ricerca.


**Returns:**
[SearchPhase](../../com.groupdocs.search.events/searchphase) - The search phase.

### getQuery() {#getQuery--}
```
public final String getQuery()
```


Ottiene la query iniziale della ricerca corrente.


**Returns:**
java.lang.String - La query iniziale della ricerca corrente.

### getWords() {#getWords--}
```
public final String[] getWords()
```


Ottiene le parole ottenute nella fase corrente.


**Returns:**
java.lang.String[] - Le parole ottenute nella fase corrente.

