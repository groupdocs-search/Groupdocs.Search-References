---
title: "Cancellation"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Représente un objet permettant de demander l'annulation d'une opération."
type: docs
weight: 11
url: /fr/java/com.groupdocs.search.common/cancellation/
---
**Inheritance:**
java.lang.Object
```
public class Cancellation
```

Représente un objet permettant de demander l'annulation d'une opération.


**Learn more**

* [Indexing options](../https://docs.groupdocs.com/display/searchjava/Indexing+options)
* [Search options](../https://docs.groupdocs.com/display/searchjava/Search+options)

## Constructeurs

| Constructeur | Description |
| --- | --- |
|  | [Cancellation()](#Cancellation--) | Initialise une nouvelle instance de la |
Cancellation
classe.
|
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [isCancelled()](#isCancelled--) | Obtient une valeur indiquant que l'annulation a été demandée. |
|
|  | [cancel()](#cancel--) | Effectue une demande d'annulation. |
|
|  | [cancelAfter(int milliseconds)](#cancelAfter-int-) | Effectue une demande d'annulation après l'expiration du nombre spécifié de millisecondes. |
|
### Cancellation() {#Cancellation--}
```
public Cancellation()
```


Initialise une nouvelle instance de la
Cancellation
classe.


### isCancelled() {#isCancelled--}
```
public final boolean isCancelled()
```


Obtient une valeur indiquant que l'annulation a été demandée.


**Returns:**
booléen - Une valeur indiquant que l'annulation a été demandée.

### cancel() {#cancel--}
```
public final void cancel()
```


Effectue une demande d'annulation.


### cancelAfter(int milliseconds) {#cancelAfter-int-}
```
public final void cancelAfter(int milliseconds)
```


Effectue une demande d'annulation après l'expiration du nombre spécifié de millisecondes.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | millisecondes | int | Le nombre de millisecondes après lequel une opération sera annulée. |
|

