---
title: "SearchPhaseEventArgs"
second_title: "GroupDocs.Search для Java API Reference"
description: "Представляет аргументы событий изменения фаз поиска."
type: docs
weight: 21
url: /ru/java/com.groupdocs.search.events/searchphaseeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class SearchPhaseEventArgs extends BaseIndexEventArgs
```

Представляет аргументы событий изменения фаз поиска.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Методы

| Метод | Описание |
| --- | --- |
|  | [getSearchPhase()](#getSearchPhase--) | Получает фазу поиска. |
|
|  | [getQuery()](#getQuery--) | Получает исходный запрос текущего поиска. |
|
|  | [getWords()](#getWords--) | Получает слова, полученные в текущей фазе. |
|
### getSearchPhase() {#getSearchPhase--}
```
public final SearchPhase getSearchPhase()
```


Получает фазу поиска.


**Returns:**
[SearchPhase](../../com.groupdocs.search.events/searchphase) - The search phase.

### getQuery() {#getQuery--}
```
public final String getQuery()
```


Получает исходный запрос текущего поиска.


**Returns:**
java.lang.String - Исходный запрос текущего поиска.

### getWords() {#getWords--}
```
public final String[] getWords()
```


Получает слова, полученные в текущей фазе.


**Returns:**
java.lang.String[] - Слова, полученные в текущей фазе.

