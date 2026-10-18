---
title: "Händelse"
second_title: "GroupDocs.Search för Java API-referens"
description: "Denna klass är avsedd att ärvas när man prenumererar på händelser."
type: docs
weight: 11
url: /sv/java/com.groupdocs.search.events/event/
---
**Inheritance:**
java.lang.Object
```
public abstract class Event<T>
```

Denna klass är avsedd att ärvas när man prenumererar på händelser.

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [Event()](#Event--) | Initierar en ny instans av klassen  Event  . |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [add(T delegate)](#add-T-) | Lägger till en lyssnare för händelsen. |
|
|  | [remove(T delegate)](#remove-T-) | Tar bort en lyssnare för händelsen. |
|
|  | [isEmpty()](#isEmpty--) | Kontrollerar om minst en lyssnare finns. |
|
### Event() {#Event--}
```
public Event()
```


Initierar en ny instans av klassen  Event  .


### add(T delegate) {#add-T-}
```
public final synchronized void add(T delegate)
```


Lägger till en lyssnare för händelsen.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | delegat | T | En lyssnare för händelsen att lägga till. |
|

### remove(T delegate) {#remove-T-}
```
public final synchronized void remove(T delegate)
```


Tar bort en lyssnare för händelsen.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | delegat | T | En lyssnare för händelsen att ta bort. |
|

### isEmpty() {#isEmpty--}
```
public synchronized boolean isEmpty()
```


Kontrollerar om minst en lyssnare finns.


**Returns:**
boolean - Ett värde som indikerar att minst en lyssnare har lagts till för händelsen.

