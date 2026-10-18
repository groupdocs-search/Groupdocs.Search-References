---
title: "MergeOptions"
second_title: "GroupDocs.Search för Java API-referens"
description: "Tillhandahåller alternativ för sammanslagningsoperationen."
type: docs
weight: 28
url: /sv/java/com.groupdocs.search.options/mergeoptions/
---
**Inheritance:**
java.lang.Object
```
public class MergeOptions
```

Tillhandahåller alternativ för sammanslagningsoperationen.


**Learn more**

* [Merge indexes](../https://docs.groupdocs.com/display/searchjava/Merge+indexes)
* [Optimize index](../https://docs.groupdocs.com/display/searchjava/Optimize+index)

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [MergeOptions()](#MergeOptions--) | Initierar en ny instans av  MergeOptions  -klassen. |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [isAsync()](#isAsync--) | Hämtar flaggan för asynkron utförande av operationen. |
|
|  | [setAsync(boolean value)](#setAsync-boolean-) | Ställer in flaggan för asynkron utförande av operationen. |
|
|  | [getCancellation()](#getCancellation--) | Hämtar objektet för avbrytning av operationen. |
|
|  | [setCancellation(Cancellation value)](#setCancellation-com.groupdocs.search.common.Cancellation-) | Ställer in objektet för avbrytning av operationen. |
|
### MergeOptions() {#MergeOptions--}
```
public MergeOptions()
```


Initierar en ny instans av  MergeOptions  -klassen.


### isAsync() {#isAsync--}
```
public final boolean isAsync()
```


Hämtar flaggan för asynkron utförande av operationen. Standardvärdet är  false .


**Returns:**
boolean - Flaggan för asynkron utförande av operationen.

### setAsync(boolean value) {#setAsync-boolean-}
```
public final void setAsync(boolean value)
```


Ställer in flaggan för asynkron utförande av operationen. Standardvärdet är  false .


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | värde | boolean | Flaggan för asynkron utförande av operationen. |
|

### getCancellation() {#getCancellation--}
```
public final Cancellation getCancellation()
```


Hämtar objektet för avbrytning av operationen. Standardvärdet är  null .


**Returns:**
[Cancellation](../../com.groupdocs.search.common/cancellation) - The operation cancellation object.

### setCancellation(Cancellation value) {#setCancellation-com.groupdocs.search.common.Cancellation-}
```
public final void setCancellation(Cancellation value)
```


Ställer in objektet för avbrytning av operationen. Standardvärdet är  null .


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | value | [Cancellation](../../com.groupdocs.search.common/cancellation) | Objektet för avbrytning av operationen. |
|

