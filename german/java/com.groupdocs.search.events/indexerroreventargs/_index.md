---
title: "IndexErrorEventArgs"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Stellt Argumente für das Ereignis dar, wenn ein Indexfehler aufgetreten ist."
type: docs
weight: 16
url: /de/java/com.groupdocs.search.events/indexerroreventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class IndexErrorEventArgs extends BaseIndexEventArgs
```

Stellt Argumente für das Ereignis dar, wenn ein Indexfehler aufgetreten ist.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getMessage()](#getMessage--) | Ermittelt die Fehlermeldung. |
|
|  | [isCritical()](#isCritical--) | Gibt ein Flag zurück, das anzeigt, dass der aufgetretene Fehler kritisch ist und der Index neu gestartet werden sollte. |
|
### getMessage() {#getMessage--}
```
public final String getMessage()
```


Ermittelt die Fehlermeldung.


**Returns:**
java.lang.String - Die Fehlermeldung.

### isCritical() {#isCritical--}
```
public final boolean isCritical()
```


Gibt ein Flag zurück, das anzeigt, dass der aufgetretene Fehler kritisch ist und der Index neu gestartet werden sollte.


**Returns:**
boolean - Das Flag, das anzeigt, dass der aufgetretene Fehler kritisch ist und der Index neu gestartet werden sollte.

