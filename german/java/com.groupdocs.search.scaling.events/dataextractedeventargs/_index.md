---
title: "DataExtractedEventArgs"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Stellt Argumente für das Ereignis dar, wenn die Datenextraktion eines Dokuments abgeschlossen ist."
type: docs
weight: 10
url: /de/java/com.groupdocs.search.scaling.events/dataextractedeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class DataExtractedEventArgs extends EventArgs
```

Stellt Argumente für das Ereignis dar, wenn die Datenextraktion eines Dokuments abgeschlossen ist.

## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getExtractorIndex()](#getExtractorIndex--) | Ermittelt den Extraktor-Index. |
|
|  | [getDocumentKey()](#getDocumentKey--) | Ermittelt den Dokumentenschlüssel. |
|
### getExtractorIndex() {#getExtractorIndex--}
```
public final int getExtractorIndex()
```


Ermittelt den Extraktor-Index.


**Returns:**
int - Der Extraktor-Index.

### getDocumentKey() {#getDocumentKey--}
```
public final String getDocumentKey()
```


Ermittelt den Dokumentenschlüssel.


**Returns:**
java.lang.String - Der Dokumentenschlüssel.

