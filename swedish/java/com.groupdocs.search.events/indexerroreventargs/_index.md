---
title: "IndexErrorEventArgs"
second_title: "GroupDocs.Search för Java API-referens"
description: "Representerar argument för händelsen när ett indexfel inträffar."
type: docs
weight: 16
url: /sv/java/com.groupdocs.search.events/indexerroreventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class IndexErrorEventArgs extends BaseIndexEventArgs
```

Representerar argument för händelsen när ett indexfel inträffar.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getMessage()](#getMessage--) | Hämtar felmeddelandet. |
|
|  | [isCritical()](#isCritical--) | Hämtar en flagga som indikerar att felet är kritiskt och att indexet bör startas om. |
|
### getMessage() {#getMessage--}
```
public final String getMessage()
```


Hämtar felmeddelandet.


**Returns:**
java.lang.String - Felmeddelandet.

### isCritical() {#isCritical--}
```
public final boolean isCritical()
```


Hämtar en flagga som indikerar att felet är kritiskt och att indexet bör startas om.


**Returns:**
boolean - Flaggan som indikerar att felet är kritiskt och att indexet bör startas om.

