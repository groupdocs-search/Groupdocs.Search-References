---
title: "ErrorOccurredEventArgs"
second_title: "GroupDocs.Search για Java API Reference"
description: "Αναπαριστά τα ορίσματα για το γεγονός που εμφανίζεται σφάλμα σε έναν από τους κόμβους του δικτύου αναζήτησης."
type: docs
weight: 13
url: /el/java/com.groupdocs.search.scaling.events/erroroccurredeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class ErrorOccurredEventArgs extends EventArgs
```

Αναπαριστά τα ορίσματα για το γεγονός που εμφανίζεται σφάλμα σε έναν από τους κόμβους του δικτύου αναζήτησης.

## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getNodeIndex()](#getNodeIndex--) | Λαμβάνει τον δείκτη του κόμβου δικτύου αναζήτησης. |
|
|  | [getServiceIndex()](#getServiceIndex--) | Λαμβάνει τον δείκτη της υπηρεσίας κόμβου δικτύου αναζήτησης. |
|
|  | [getMessage()](#getMessage--) | Λαμβάνει το μήνυμα σφάλματος. |
|
### getNodeIndex() {#getNodeIndex--}
```
public final int getNodeIndex()
```


Λαμβάνει τον δείκτη του κόμβου δικτύου αναζήτησης.


**Returns:**
int - Ο δείκτης του κόμβου δικτύου αναζήτησης.

### getServiceIndex() {#getServiceIndex--}
```
public final int getServiceIndex()
```


Λαμβάνει τον δείκτη της υπηρεσίας κόμβου δικτύου αναζήτησης.


**Returns:**
int - Ο δείκτης της υπηρεσίας κόμβου δικτύου αναζήτησης.

### getMessage() {#getMessage--}
```
public final String getMessage()
```


Λαμβάνει το μήνυμα σφάλματος.


**Returns:**
java.lang.String - Το μήνυμα σφάλματος.

