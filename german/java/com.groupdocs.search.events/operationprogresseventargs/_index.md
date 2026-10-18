---
title: "OperationProgressEventArgs"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Stellt Argumente für das Ereignis dar, wenn der Fortschritt des Indexierungsvorgangs aktualisiert wird."
type: docs
weight: 18
url: /de/java/com.groupdocs.search.events/operationprogresseventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class OperationProgressEventArgs extends BaseIndexEventArgs
```

Stellt Argumente für das Ereignis dar, wenn der Fortschritt des Indexierungsvorgangs aktualisiert wird.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getTotalDocuments()](#getTotalDocuments--) | Liefert die Gesamtzahl der zu verarbeitenden Dokumente. |
|
|  | [getProcessedDocuments()](#getProcessedDocuments--) | Gibt die Anzahl der erfolgreich verarbeiteten Dokumente zurück. |
|
|  | [getSkippedDocuments()](#getSkippedDocuments--) | Gibt die Anzahl der übersprungenen Dokumente zurück. |
|
|  | [getProgressPercentage()](#getProgressPercentage--) | Liefert den Prozentsatz des Fortschritts. |
|
|  | [getLastDocumentKey()](#getLastDocumentKey--) | Gibt den Schlüssel des zuletzt verarbeiteten Dokuments zurück. |
|
|  | [getLastDocumentPath()](#getLastDocumentPath--) | Gibt den Pfad des zuletzt verarbeiteten Dokuments zurück. |
|
|  | [getLastDocumentStatus()](#getLastDocumentStatus--) | Gibt den Status des zuletzt verarbeiteten Dokuments zurück. |
|
### getTotalDocuments() {#getTotalDocuments--}
```
public final int getTotalDocuments()
```


Liefert die Gesamtzahl der zu verarbeitenden Dokumente.


**Returns:**
int - Die Gesamtzahl der zu verarbeitenden Dokumente.

### getProcessedDocuments() {#getProcessedDocuments--}
```
public final int getProcessedDocuments()
```


Gibt die Anzahl der erfolgreich verarbeiteten Dokumente zurück.


**Returns:**
int - Die Anzahl der erfolgreich verarbeiteten Dokumente.

### getSkippedDocuments() {#getSkippedDocuments--}
```
public final int getSkippedDocuments()
```


Gibt die Anzahl der übersprungenen Dokumente zurück.


**Returns:**
int - Die Anzahl der übersprungenen Dokumente.

### getProgressPercentage() {#getProgressPercentage--}
```
public final double getProgressPercentage()
```


Liefert den Prozentsatz des Fortschritts.


**Returns:**
double - Der Prozentsatz des Fortschritts.

### getLastDocumentKey() {#getLastDocumentKey--}
```
public final String getLastDocumentKey()
```


Gibt den Schlüssel des zuletzt verarbeiteten Dokuments zurück.


**Returns:**
java.lang.String - Der Schlüssel des zuletzt verarbeiteten Dokuments.

### getLastDocumentPath() {#getLastDocumentPath--}
```
public final String getLastDocumentPath()
```


Gibt den Pfad des zuletzt verarbeiteten Dokuments zurück.


**Returns:**
java.lang.String - Der Pfad des zuletzt verarbeiteten Dokuments.

### getLastDocumentStatus() {#getLastDocumentStatus--}
```
public final DocumentStatus getLastDocumentStatus()
```


Gibt den Status des zuletzt verarbeiteten Dokuments zurück.


**Returns:**
[DocumentStatus](../../com.groupdocs.search.common/documentstatus) - The last processed document status.

