---
title: "IndexErrorEventArgs"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Stelt de argumenten voor het evenement voor wanneer een indexfout optreedt."
type: docs
weight: 16
url: /nl/java/com.groupdocs.search.events/indexerroreventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class IndexErrorEventArgs extends BaseIndexEventArgs
```

Stelt de argumenten voor het evenement voor wanneer een indexfout optreedt.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getMessage()](#getMessage--) | Haalt het foutbericht op. |
|
|  | [isCritical()](#isCritical--) | Haalt een vlag op die aangeeft dat de fout kritiek is en dat de index opnieuw moet worden gestart. |
|
### getMessage() {#getMessage--}
```
public final String getMessage()
```


Haalt het foutbericht op.


**Returns:**
java.lang.String - Het foutbericht.

### isCritical() {#isCritical--}
```
public final boolean isCritical()
```


Haalt een vlag op die aangeeft dat de fout kritiek is en dat de index opnieuw moet worden gestart.


**Returns:**
boolean - De vlag die aangeeft dat de fout kritiek is en dat de index opnieuw moet worden gestart.

