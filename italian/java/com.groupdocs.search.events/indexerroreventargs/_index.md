---
title: "IndexErrorEventArgs"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Rappresenta gli argomenti per l'evento di errore di indicizzazione verificatosi."
type: docs
weight: 16
url: /it/java/com.groupdocs.search.events/indexerroreventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class IndexErrorEventArgs extends BaseIndexEventArgs
```

Rappresenta gli argomenti per l'evento di errore di indicizzazione verificatosi.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getMessage()](#getMessage--) | Restituisce il messaggio di errore. |
|
|  | [isCritical()](#isCritical--) | Ottiene un flag che indica che l'errore verificato è critico e l'indice dovrebbe essere riavviato. |
|
### getMessage() {#getMessage--}
```
public final String getMessage()
```


Restituisce il messaggio di errore.


**Returns:**
java.lang.String - Il messaggio di errore.

### isCritical() {#isCritical--}
```
public final boolean isCritical()
```


Ottiene un flag che indica che l'errore verificato è critico e l'indice dovrebbe essere riavviato.


**Returns:**
boolean - Il flag che indica che l'errore verificato è critico e l'indice dovrebbe essere riavviato.

