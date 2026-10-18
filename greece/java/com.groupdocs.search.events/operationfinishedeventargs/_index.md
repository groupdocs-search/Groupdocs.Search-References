---
title: "OperationFinishedEventArgs"
second_title: "GroupDocs.Search για Java API Reference"
description: "Αναπαριστά τα ορίσματα για το γεγονός που ολοκληρώνεται η λειτουργία ευρετηρίασης."
type: docs
weight: 17
url: /el/java/com.groupdocs.search.events/operationfinishedeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class OperationFinishedEventArgs extends BaseIndexEventArgs
```

Αναπαριστά τα ορίσματα για το γεγονός που ολοκληρώνεται η λειτουργία ευρετηρίασης.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getMessage()](#getMessage--) | Λαμβάνει το μήνυμα. |
|
|  | [getOperationType()](#getOperationType--) | Λαμβάνει τον τύπο λειτουργίας. |
|
### getMessage() {#getMessage--}
```
public final String getMessage()
```


Λαμβάνει το μήνυμα.


**Returns:**
java.lang.String - Το μήνυμα.

### getOperationType() {#getOperationType--}
```
public final OperationType getOperationType()
```


Λαμβάνει τον τύπο λειτουργίας.


**Returns:**
[OperationType](../../com.groupdocs.search.events/operationtype) - The operation type.

