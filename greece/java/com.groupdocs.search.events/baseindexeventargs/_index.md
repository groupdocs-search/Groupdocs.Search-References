---
title: "BaseIndexEventArgs"
second_title: "GroupDocs.Search για Java API Reference"
description: "Αναπαριστά τη βασική κλάση των ορισμάτων γεγονότος."
type: docs
weight: 10
url: /el/java/com.groupdocs.search.events/baseindexeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class BaseIndexEventArgs extends EventArgs
```

Αναπαριστά τη βασική κλάση των ορισμάτων γεγονότος.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getTime()](#getTime--) | Λαμβάνει την ώρα ενός συμβάντος. |
|
|  | [getIndexId()](#getIndexId--) | Λαμβάνει το αναγνωριστικό του ευρετηρίου. |
|
|  | [getIndexFolder()](#getIndexFolder--) | Λαμβάνει το φάκελο του ευρετηρίου. |
|
|  | [getStatus()](#getStatus--) | Λαμβάνει την κατάσταση του ευρετηρίου. |
|
### getTime() {#getTime--}
```
public final Date getTime()
```


Λαμβάνει την ώρα ενός συμβάντος.


**Returns:**
java.util.Date - Η ώρα ενός συμβάντος.

### getIndexId() {#getIndexId--}
```
public final UUID getIndexId()
```


Λαμβάνει το αναγνωριστικό του ευρετηρίου.


**Returns:**
java.util.UUID - Το αναγνωριστικό του ευρετηρίου.

### getIndexFolder() {#getIndexFolder--}
```
public final String getIndexFolder()
```


Λαμβάνει το φάκελο του ευρετηρίου.


**Returns:**
java.lang.String - Ο φάκελος του ευρετηρίου.

### getStatus() {#getStatus--}
```
public final IndexStatus getStatus()
```


Λαμβάνει την κατάσταση του ευρετηρίου.


**Returns:**
[IndexStatus](../../com.groupdocs.search.common/indexstatus) - The index status.

