---
title: "DocumentIndexedEventArgs"
second_title: "GroupDocs.Search για Java API Reference"
description: "Αναπαριστά τα ορίσματα για το γεγονός που ολοκληρώνεται η ευρετηρίαση εγγράφου."
type: docs
weight: 12
url: /el/java/com.groupdocs.search.scaling.events/documentindexedeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class DocumentIndexedEventArgs extends EventArgs
```

Αναπαριστά τα ορίσματα για το γεγονός που ολοκληρώνεται η ευρετηρίαση εγγράφου.

## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getShardIndex()](#getShardIndex--) | Λαμβάνει τον δείκτη του τμήματος. |
|
|  | [getDocumentKey()](#getDocumentKey--) | Λαμβάνει το κλειδί του εγγράφου. |
|
### getShardIndex() {#getShardIndex--}
```
public final int getShardIndex()
```


Λαμβάνει τον δείκτη του τμήματος.


**Returns:**
int - Ο δείκτης του τμήματος.

### getDocumentKey() {#getDocumentKey--}
```
public final String getDocumentKey()
```


Λαμβάνει το κλειδί του εγγράφου.


**Returns:**
java.lang.String - Το κλειδί του εγγράφου.

