---
title: "SearchPhaseEventArgs"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Representa los argumentos de los eventos de cambio de fase de búsqueda."
type: docs
weight: 21
url: /es/java/com.groupdocs.search.events/searchphaseeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class SearchPhaseEventArgs extends BaseIndexEventArgs
```

Representa los argumentos de los eventos de cambio de fase de búsqueda.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Métodos

| Método | Descripción |
| --- | --- |
|  | [getSearchPhase()](#getSearchPhase--) | Obtiene la fase de búsqueda. |
|
|  | [getQuery()](#getQuery--) | Obtiene la consulta inicial de la búsqueda actual. |
|
|  | [getWords()](#getWords--) | Obtiene las palabras obtenidas en la fase actual. |
|
### getSearchPhase() {#getSearchPhase--}
```
public final SearchPhase getSearchPhase()
```


Obtiene la fase de búsqueda.


**Returns:**
[SearchPhase](../../com.groupdocs.search.events/searchphase) - The search phase.

### getQuery() {#getQuery--}
```
public final String getQuery()
```


Obtiene la consulta inicial de la búsqueda actual.


**Returns:**
java.lang.String - La consulta inicial de la búsqueda actual.

### getWords() {#getWords--}
```
public final String[] getWords()
```


Obtiene las palabras obtenidas en la fase actual.


**Returns:**
java.lang.String[] - Las palabras obtenidas en la fase actual.

