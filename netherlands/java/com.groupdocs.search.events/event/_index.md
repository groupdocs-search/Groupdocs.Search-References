---
title: "Event"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Deze klasse is bedoeld om te worden geërfd bij het abonneren op gebeurtenissen."
type: docs
weight: 11
url: /nl/java/com.groupdocs.search.events/event/
---
**Inheritance:**
java.lang.Object
```
public abstract class Event<T>
```

Deze klasse is bedoeld om te worden geërfd bij het abonneren op gebeurtenissen.

## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [Event()](#Event--) | Initialiseert een nieuw exemplaar van de  Event  klasse. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [add(T delegate)](#add-T-) | Voegt een luisteraar toe voor het evenement. |
|
|  | [remove(T delegate)](#remove-T-) | Verwijdert een luisteraar voor het evenement. |
|
|  | [isEmpty()](#isEmpty--) | Controleert op aanwezigheid van ten minste één luisteraar. |
|
### Event() {#Event--}
```
public Event()
```


Initialiseert een nieuw exemplaar van de  Event  klasse.


### add(T delegate) {#add-T-}
```
public final synchronized void add(T delegate)
```


Voegt een luisteraar toe voor het evenement.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | delegate | T | Een luisteraar voor het evenement om toe te voegen. |
|

### remove(T delegate) {#remove-T-}
```
public final synchronized void remove(T delegate)
```


Verwijdert een luisteraar voor het evenement.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | delegate | T | Een luisteraar voor het evenement om te verwijderen. |
|

### isEmpty() {#isEmpty--}
```
public synchronized boolean isEmpty()
```


Controleert op aanwezigheid van ten minste één luisteraar.


**Returns:**
boolean - Een waarde die aangeeft dat er ten minste één luisteraar is toegevoegd voor het evenement.

