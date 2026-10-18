---
title: "OperationFinishedEventArgs"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Stelt de argumenten voor het evenement voor wanneer de indexeringsbewerking is voltooid."
type: docs
weight: 17
url: /nl/java/com.groupdocs.search.events/operationfinishedeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class OperationFinishedEventArgs extends BaseIndexEventArgs
```

Stelt de argumenten voor het evenement voor wanneer de indexeringsbewerking is voltooid.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getMessage()](#getMessage--) | Haalt het bericht op. |
|
|  | [getOperationType()](#getOperationType--) | Haalt het operatietype op. |
|
### getMessage() {#getMessage--}
```
public final String getMessage()
```


Haalt het bericht op.


**Returns:**
java.lang.String - Het bericht.

### getOperationType() {#getOperationType--}
```
public final OperationType getOperationType()
```


Haalt het operatietype op.


**Returns:**
[OperationType](../../com.groupdocs.search.events/operationtype) - The operation type.

