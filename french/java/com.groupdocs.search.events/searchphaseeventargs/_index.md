---
title: "SearchPhaseEventArgs"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Représente les arguments des événements de changement de phase de recherche."
type: docs
weight: 21
url: /fr/java/com.groupdocs.search.events/searchphaseeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class SearchPhaseEventArgs extends BaseIndexEventArgs
```

Représente les arguments des événements de changement de phase de recherche.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getSearchPhase()](#getSearchPhase--) | Obtient la phase de recherche. |
|
|  | [getQuery()](#getQuery--) | Obtient la requête initiale de la recherche en cours. |
|
|  | [getWords()](#getWords--) | Obtient les mots obtenus dans la phase actuelle. |
|
### getSearchPhase() {#getSearchPhase--}
```
public final SearchPhase getSearchPhase()
```


Obtient la phase de recherche.


**Returns:**
[SearchPhase](../../com.groupdocs.search.events/searchphase) - The search phase.

### getQuery() {#getQuery--}
```
public final String getQuery()
```


Obtient la requête initiale de la recherche en cours.


**Returns:**
java.lang.String - La requête initiale de la recherche en cours.

### getWords() {#getWords--}
```
public final String[] getWords()
```


Obtient les mots obtenus dans la phase actuelle.


**Returns:**
java.lang.String[] - Les mots obtenus dans la phase actuelle.

