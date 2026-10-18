---
title: "Ereignis"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Diese Klasse ist zum Erben vorgesehen, wenn man Ereignisse abonniert."
type: docs
weight: 11
url: /de/java/com.groupdocs.search.events/event/
---
**Inheritance:**
java.lang.Object
```
public abstract class Event<T>
```

Diese Klasse ist zum Erben vorgesehen, wenn man Ereignisse abonniert.

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [Event()](#Event--) | Initialisiert eine neue Instanz der  Event  Klasse. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [add(T delegate)](#add-T-) | Fügt einen Listener für das Ereignis hinzu. |
|
|  | [remove(T delegate)](#remove-T-) | Entfernt einen Listener für das Ereignis. |
|
|  | [isEmpty()](#isEmpty--) | Prüft, ob mindestens ein Listener vorhanden ist. |
|
### Event() {#Event--}
```
public Event()
```


Initialisiert eine neue Instanz der  Event  Klasse.


### add(T delegate) {#add-T-}
```
public final synchronized void add(T delegate)
```


Fügt einen Listener für das Ereignis hinzu.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Delegat | T | Ein Listener für das Ereignis zum Hinzufügen. |
|

### remove(T delegate) {#remove-T-}
```
public final synchronized void remove(T delegate)
```


Entfernt einen Listener für das Ereignis.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Delegat | T | Ein Listener für das Ereignis zum Entfernen. |
|

### isEmpty() {#isEmpty--}
```
public synchronized boolean isEmpty()
```


Prüft, ob mindestens ein Listener vorhanden ist.


**Returns:**
boolean - Ein Wert, der angibt, dass mindestens ein Listener für das Ereignis hinzugefügt wurde.

