---
title: "IndexErrorEventArgs"
second_title: "GroupDocs.Search για Java API Reference"
description: "Αναπαριστά τα ορίσματα για το γεγονός που προέκυψε σφάλμα ευρετηρίου."
type: docs
weight: 16
url: /el/java/com.groupdocs.search.events/indexerroreventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class IndexErrorEventArgs extends BaseIndexEventArgs
```

Αναπαριστά τα ορίσματα για το γεγονός που προέκυψε σφάλμα ευρετηρίου.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getMessage()](#getMessage--) | Λαμβάνει το μήνυμα σφάλματος. |
|
|  | [isCritical()](#isCritical--) | Λαμβάνει μια σημαία που υποδεικνύει ότι το σφάλμα που συνέβη είναι κρίσιμο και ότι το ευρετήριο πρέπει να επανεκκινηθεί. |
|
### getMessage() {#getMessage--}
```
public final String getMessage()
```


Λαμβάνει το μήνυμα σφάλματος.


**Returns:**
java.lang.String - Το μήνυμα σφάλματος.

### isCritical() {#isCritical--}
```
public final boolean isCritical()
```


Λαμβάνει μια σημαία που υποδεικνύει ότι το σφάλμα που συνέβη είναι κρίσιμο και ότι το ευρετήριο πρέπει να επανεκκινηθεί.


**Returns:**
boolean - Η σημαία που υποδεικνύει ότι το σφάλμα που συνέβη είναι κρίσιμο και ότι το ευρετήριο πρέπει να επανεκκινηθεί.

