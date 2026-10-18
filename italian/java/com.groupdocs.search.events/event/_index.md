---
title: "Evento"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Questa classe è destinata ad essere ereditata quando ci si iscrive agli eventi."
type: docs
weight: 11
url: /it/java/com.groupdocs.search.events/event/
---
**Inheritance:**
java.lang.Object
```
public abstract class Event<T>
```

Questa classe è destinata ad essere ereditata quando ci si iscrive agli eventi.

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [Event()](#Event--) | Inizializza una nuova istanza della classe  Event . |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [add(T delegate)](#add-T-) | Aggiunge un listener per l'evento. |
|
|  | [remove(T delegate)](#remove-T-) | Rimuove un listener per l'evento. |
|
|  | [isEmpty()](#isEmpty--) | Verifica la presenza di almeno un listener. |
|
### Event() {#Event--}
```
public Event()
```


Inizializza una nuova istanza della classe  Event .


### add(T delegate) {#add-T-}
```
public final synchronized void add(T delegate)
```


Aggiunge un listener per l'evento.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | delegate | T | Un listener per l'evento da aggiungere. |
|

### remove(T delegate) {#remove-T-}
```
public final synchronized void remove(T delegate)
```


Rimuove un listener per l'evento.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | delegate | T | Un listener per l'evento da rimuovere. |
|

### isEmpty() {#isEmpty--}
```
public synchronized boolean isEmpty()
```


Verifica la presenza di almeno un listener.


**Returns:**
boolean - Un valore che indica che almeno un listener è stato aggiunto per l'evento.

