---
title: "Avbrytning"
second_title: "GroupDocs.Search för Java API-referens"
description: "Representerar ett objekt för att begära avbrytning av en operation."
type: docs
weight: 11
url: /sv/java/com.groupdocs.search.common/cancellation/
---
**Inheritance:**
java.lang.Object
```
public class Cancellation
```

Representerar ett objekt för att begära avbrytning av en operation.


**Learn more**

* [Indexing options](../https://docs.groupdocs.com/display/searchjava/Indexing+options)
* [Search options](../https://docs.groupdocs.com/display/searchjava/Search+options)

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [Cancellation()](#Cancellation--) | Initierar en ny instans av |
Avbrytning
klassen.
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [isCancelled()](#isCancelled--) | Hämtar ett värde som indikerar att avbrytning har begärts. |
|
|  | [cancel()](#cancel--) | Gör en begäran om avbrytning. |
|
|  | [cancelAfter(int milliseconds)](#cancelAfter-int-) | Gör en begäran om avbrytning efter att det angivna antalet millisekunder har löpt ut. |
|
### Cancellation() {#Cancellation--}
```
public Cancellation()
```


Initierar en ny instans av
Avbrytning
klassen.


### isCancelled() {#isCancelled--}
```
public final boolean isCancelled()
```


Hämtar ett värde som indikerar att avbrytning har begärts.


**Returns:**
boolean - Ett värde som indikerar att avbrytning har begärts.

### cancel() {#cancel--}
```
public final void cancel()
```


Gör en begäran om avbrytning.


### cancelAfter(int milliseconds) {#cancelAfter-int-}
```
public final void cancelAfter(int milliseconds)
```


Gör en begäran om avbrytning efter att det angivna antalet millisekunder har löpt ut.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | millisekunder | int | Antalet millisekunder efter vilka en operation kommer att avbrytas. |
|

