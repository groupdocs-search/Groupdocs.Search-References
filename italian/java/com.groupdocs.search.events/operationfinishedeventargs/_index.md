---
title: "OperationFinishedEventArgs"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Rappresenta gli argomenti per l'evento di completamento dell'operazione di indicizzazione."
type: docs
weight: 17
url: /it/java/com.groupdocs.search.events/operationfinishedeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class OperationFinishedEventArgs extends BaseIndexEventArgs
```

Rappresenta gli argomenti per l'evento di completamento dell'operazione di indicizzazione.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getMessage()](#getMessage--) | Ottiene il messaggio. |
|
|  | [getOperationType()](#getOperationType--) | Ottiene il tipo di operazione. |
|
### getMessage() {#getMessage--}
```
public final String getMessage()
```


Ottiene il messaggio.


**Returns:**
java.lang.String - Il messaggio.

### getOperationType() {#getOperationType--}
```
public final OperationType getOperationType()
```


Ottiene il tipo di operazione.


**Returns:**
[OperationType](../../com.groupdocs.search.events/operationtype) - The operation type.

