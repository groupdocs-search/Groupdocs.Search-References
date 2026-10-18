---
title: "Cancellation"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Rappresenta un oggetto per richiedere la cancellazione di un'operazione."
type: docs
weight: 11
url: /it/java/com.groupdocs.search.common/cancellation/
---
**Inheritance:**
java.lang.Object
```
public class Cancellation
```

Rappresenta un oggetto per richiedere la cancellazione di un'operazione.


**Learn more**

* [Indexing options](../https://docs.groupdocs.com/display/searchjava/Indexing+options)
* [Search options](../https://docs.groupdocs.com/display/searchjava/Search+options)

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [Cancellation()](#Cancellation--) | Inizializza una nuova istanza di |
Cancellation
classe.
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [isCancelled()](#isCancelled--) | Restituisce un valore che indica che è stata richiesta la cancellazione. |
|
|  | [cancel()](#cancel--) | Effettua una richiesta di cancellazione. |
|
|  | [cancelAfter(int milliseconds)](#cancelAfter-int-) | Effettua una richiesta di cancellazione dopo la scadenza del numero specificato di millisecondi. |
|
### Cancellation() {#Cancellation--}
```
public Cancellation()
```


Inizializza una nuova istanza di
Cancellation
classe.


### isCancelled() {#isCancelled--}
```
public final boolean isCancelled()
```


Restituisce un valore che indica che è stata richiesta la cancellazione.


**Returns:**
boolean - Un valore che indica che è stata richiesta la cancellazione.

### cancel() {#cancel--}
```
public final void cancel()
```


Effettua una richiesta di cancellazione.


### cancelAfter(int milliseconds) {#cancelAfter-int-}
```
public final void cancelAfter(int milliseconds)
```


Effettua una richiesta di cancellazione dopo la scadenza del numero specificato di millisecondi.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | millisecondi | int | Il numero di millisecondi dopo i quali un'operazione verrà annullata. |
|

