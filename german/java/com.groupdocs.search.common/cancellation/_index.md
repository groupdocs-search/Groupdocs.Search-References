---
title: "Abbruch"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Stellt ein Objekt zur Anforderung des Abbruchs einer Operation dar."
type: docs
weight: 11
url: /de/java/com.groupdocs.search.common/cancellation/
---
**Inheritance:**
java.lang.Object
```
public class Cancellation
```

Stellt ein Objekt zur Anforderung des Abbruchs einer Operation dar.


**Learn more**

* [Indexing options](../https://docs.groupdocs.com/display/searchjava/Indexing+options)
* [Search options](../https://docs.groupdocs.com/display/searchjava/Search+options)

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [Cancellation()](#Cancellation--) | Initialisiert eine neue Instanz von |
Abbruch
Klasse.
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [isCancelled()](#isCancelled--) | Gibt einen Wert zurück, der anzeigt, dass ein Abbruch angefordert wurde. |
|
|  | [cancel()](#cancel--) | Stellt eine Anfrage zum Abbruch. |
|
|  | [cancelAfter(int milliseconds)](#cancelAfter-int-) | Stellt eine Anfrage zum Abbruch nach Ablauf der angegebenen Millisekundenzahl. |
|
### Cancellation() {#Cancellation--}
```
public Cancellation()
```


Initialisiert eine neue Instanz von
Abbruch
Klasse.


### isCancelled() {#isCancelled--}
```
public final boolean isCancelled()
```


Gibt einen Wert zurück, der anzeigt, dass ein Abbruch angefordert wurde.


**Returns:**
boolean - Ein Wert, der anzeigt, dass ein Abbruch angefordert wurde.

### cancel() {#cancel--}
```
public final void cancel()
```


Stellt eine Anfrage zum Abbruch.


### cancelAfter(int milliseconds) {#cancelAfter-int-}
```
public final void cancelAfter(int milliseconds)
```


Stellt eine Anfrage zum Abbruch nach Ablauf der angegebenen Millisekundenzahl.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Millisekunden | int | Die Anzahl der Millisekunden, nach denen ein Vorgang abgebrochen wird. |
|

