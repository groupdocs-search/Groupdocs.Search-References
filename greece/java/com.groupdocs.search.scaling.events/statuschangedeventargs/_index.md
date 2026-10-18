---
title: "StatusChangedEventArgs"
second_title: "GroupDocs.Search για Java API Reference"
description: "Αναπαριστά τα ορίσματα για το γεγονός αλλαγής κατάστασης του δικτύου αναζήτησης."
type: docs
weight: 17
url: /el/java/com.groupdocs.search.scaling.events/statuschangedeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class StatusChangedEventArgs extends EventArgs
```

Αναπαριστά τα ορίσματα για το γεγονός αλλαγής κατάστασης του δικτύου αναζήτησης.

## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getOldStatus()](#getOldStatus--) | Λαμβάνει την παλιά κατάσταση του δικτύου αναζήτησης. |
|
|  | [getNewStatus()](#getNewStatus--) | Λαμβάνει τη νέα κατάσταση του δικτύου αναζήτησης. |
|
### getOldStatus() {#getOldStatus--}
```
public final SearchNetworkStatus getOldStatus()
```


Λαμβάνει την παλιά κατάσταση του δικτύου αναζήτησης.


**Returns:**
[SearchNetworkStatus](../../com.groupdocs.search.scaling/searchnetworkstatus) - The old search network status.

### getNewStatus() {#getNewStatus--}
```
public final SearchNetworkStatus getNewStatus()
```


Λαμβάνει τη νέα κατάσταση του δικτύου αναζήτησης.


**Returns:**
[SearchNetworkStatus](../../com.groupdocs.search.scaling/searchnetworkstatus) - The new search network status.

