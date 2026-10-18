---
title: "Annulering"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Stelt een object voor om annulering van een bewerking aan te vragen."
type: docs
weight: 11
url: /nl/java/com.groupdocs.search.common/cancellation/
---
**Inheritance:**
java.lang.Object
```
public class Cancellation
```

Stelt een object voor om annulering van een bewerking aan te vragen.


**Learn more**

* [Indexing options](../https://docs.groupdocs.com/display/searchjava/Indexing+options)
* [Search options](../https://docs.groupdocs.com/display/searchjava/Search+options)

## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [Cancellation()](#Cancellation--) | Initialiseert een nieuw exemplaar van de |
Annulering
klasse.
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [isCancelled()](#isCancelled--) | Haalt een waarde op die aangeeft dat annulering is aangevraagd. |
|
|  | [cancel()](#cancel--) | Doet een verzoek tot annulering. |
|
|  | [cancelAfter(int milliseconds)](#cancelAfter-int-) | Doet een verzoek tot annulering na het verstrijken van het opgegeven aantal milliseconden. |
|
### Cancellation() {#Cancellation--}
```
public Cancellation()
```


Initialiseert een nieuw exemplaar van de
Annulering
klasse.


### isCancelled() {#isCancelled--}
```
public final boolean isCancelled()
```


Haalt een waarde op die aangeeft dat annulering is aangevraagd.


**Returns:**
boolean - Een waarde die aangeeft dat annulering is aangevraagd.

### cancel() {#cancel--}
```
public final void cancel()
```


Doet een verzoek tot annulering.


### cancelAfter(int milliseconds) {#cancelAfter-int-}
```
public final void cancelAfter(int milliseconds)
```


Doet een verzoek tot annulering na het verstrijken van het opgegeven aantal milliseconden.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | milliseconden | int | Het aantal milliseconden waarna een bewerking wordt geannuleerd. |
|

