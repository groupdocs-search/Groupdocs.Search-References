---
title: "MergeOptions"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Fornisce opzioni per l'operazione di unione."
type: docs
weight: 28
url: /it/java/com.groupdocs.search.options/mergeoptions/
---
**Inheritance:**
java.lang.Object
```
public class MergeOptions
```

Fornisce opzioni per l'operazione di unione.


**Learn more**

* [Merge indexes](../https://docs.groupdocs.com/display/searchjava/Merge+indexes)
* [Optimize index](../https://docs.groupdocs.com/display/searchjava/Optimize+index)

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [MergeOptions()](#MergeOptions--) | Inizializza una nuova istanza della classe MergeOptions. |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [isAsync()](#isAsync--) | Restituisce il flag dell'esecuzione asincrona dell'operazione. |
|
|  | [setAsync(boolean value)](#setAsync-boolean-) | Imposta il flag dell'esecuzione asincrona dell'operazione. |
|
|  | [getCancellation()](#getCancellation--) | Restituisce l'oggetto di annullamento dell'operazione. |
|
|  | [setCancellation(Cancellation value)](#setCancellation-com.groupdocs.search.common.Cancellation-) | Imposta l'oggetto di annullamento dell'operazione. |
|
### MergeOptions() {#MergeOptions--}
```
public MergeOptions()
```


Inizializza una nuova istanza della classe MergeOptions.


### isAsync() {#isAsync--}
```
public final boolean isAsync()
```


Ottiene il flag dell'esecuzione asincrona dell'operazione. Il valore predefinito è  false .


**Returns:**
boolean - Il flag dell'esecuzione asincrona dell'operazione.

### setAsync(boolean value) {#setAsync-boolean-}
```
public final void setAsync(boolean value)
```


Imposta il flag dell'esecuzione asincrona dell'operazione. Il valore predefinito è  false .


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | boolean | Il flag dell'esecuzione asincrona dell'operazione. |
|

### getCancellation() {#getCancellation--}
```
public final Cancellation getCancellation()
```


Ottiene l'oggetto di annullamento dell'operazione. Il valore predefinito è  null .


**Returns:**
[Cancellation](../../com.groupdocs.search.common/cancellation) - The operation cancellation object.

### setCancellation(Cancellation value) {#setCancellation-com.groupdocs.search.common.Cancellation-}
```
public final void setCancellation(Cancellation value)
```


Imposta l'oggetto di annullamento dell'operazione. Il valore predefinito è  null .


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | value | [Cancellation](../../com.groupdocs.search.common/cancellation) | L'oggetto di annullamento dell'operazione. |
|

