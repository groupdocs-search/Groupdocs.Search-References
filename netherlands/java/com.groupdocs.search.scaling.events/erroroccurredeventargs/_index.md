---
title: "ErrorOccurredEventArgs"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Stelt de argumenten voor het evenement voor wanneer een fout optreedt in een van de knooppunten van het zoeknetwerk."
type: docs
weight: 13
url: /nl/java/com.groupdocs.search.scaling.events/erroroccurredeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class ErrorOccurredEventArgs extends EventArgs
```

Stelt de argumenten voor het evenement voor wanneer een fout optreedt in een van de knooppunten van het zoeknetwerk.

## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getNodeIndex()](#getNodeIndex--) | Haalt de index van het zoeknetwerk‑knooppunt op. |
|
|  | [getServiceIndex()](#getServiceIndex--) | Haalt de index van de zoeknetwerk‑knooppuntservice op. |
|
|  | [getMessage()](#getMessage--) | Haalt het foutbericht op. |
|
### getNodeIndex() {#getNodeIndex--}
```
public final int getNodeIndex()
```


Haalt de index van het zoeknetwerk‑knooppunt op.


**Returns:**
int - De index van het zoeknetwerk‑knooppunt.

### getServiceIndex() {#getServiceIndex--}
```
public final int getServiceIndex()
```


Haalt de index van de zoeknetwerk‑knooppuntservice op.


**Returns:**
int - De index van de zoeknetwerk‑knooppuntservice.

### getMessage() {#getMessage--}
```
public final String getMessage()
```


Haalt het foutbericht op.


**Returns:**
java.lang.String - Het foutbericht.

