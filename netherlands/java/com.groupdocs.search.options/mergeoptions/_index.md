---
title: "MergeOptions"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Biedt opties voor de samenvoegbewerking."
type: docs
weight: 28
url: /nl/java/com.groupdocs.search.options/mergeoptions/
---
**Inheritance:**
java.lang.Object
```
public class MergeOptions
```

Biedt opties voor de samenvoegbewerking.


**Learn more**

* [Merge indexes](../https://docs.groupdocs.com/display/searchjava/Merge+indexes)
* [Optimize index](../https://docs.groupdocs.com/display/searchjava/Optimize+index)

## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [MergeOptions()](#MergeOptions--) | Initialiseert een nieuw exemplaar van de MergeOptions-klasse. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [isAsync()](#isAsync--) | Haalt de vlag op van asynchrone uitvoering van de bewerking. |
|
|  | [setAsync(boolean value)](#setAsync-boolean-) | Stelt de vlag in van asynchrone uitvoering van de bewerking. |
|
|  | [getCancellation()](#getCancellation--) | Haalt het annuleringsobject van de bewerking op. |
|
|  | [setCancellation(Cancellation value)](#setCancellation-com.groupdocs.search.common.Cancellation-) | Stelt het annuleringsobject van de bewerking in. |
|
### MergeOptions() {#MergeOptions--}
```
public MergeOptions()
```


Initialiseert een nieuw exemplaar van de MergeOptions-klasse.


### isAsync() {#isAsync--}
```
public final boolean isAsync()
```


Haalt de vlag op voor asynchrone uitvoering van de bewerking. De standaardwaarde is false.


**Returns:**
boolean - De vlag voor asynchrone uitvoering van de bewerking.

### setAsync(boolean value) {#setAsync-boolean-}
```
public final void setAsync(boolean value)
```


Stelt de vlag in voor asynchrone uitvoering van de bewerking. De standaardwaarde is false.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | waarde | boolean | De vlag voor asynchrone uitvoering van de bewerking. |
|

### getCancellation() {#getCancellation--}
```
public final Cancellation getCancellation()
```


Haalt het annuleringsobject van de bewerking op. De standaardwaarde is null.


**Returns:**
[Cancellation](../../com.groupdocs.search.common/cancellation) - The operation cancellation object.

### setCancellation(Cancellation value) {#setCancellation-com.groupdocs.search.common.Cancellation-}
```
public final void setCancellation(Cancellation value)
```


Stelt het annuleringsobject van de bewerking in. De standaardwaarde is null.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | value | [Cancellation](../../com.groupdocs.search.common/cancellation) | Het annuleringsobject van de bewerking. |
|

