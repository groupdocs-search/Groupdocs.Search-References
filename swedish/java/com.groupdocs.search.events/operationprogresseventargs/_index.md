---
title: "OperationProgressEventArgs"
second_title: "GroupDocs.Search för Java API-referens"
description: "Representerar argument för händelsen när framstegen för indexeringsoperationen uppdateras."
type: docs
weight: 18
url: /sv/java/com.groupdocs.search.events/operationprogresseventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class OperationProgressEventArgs extends BaseIndexEventArgs
```

Representerar argument för händelsen när framstegen för indexeringsoperationen uppdateras.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getTotalDocuments()](#getTotalDocuments--) | Hämtar det totala antalet dokument för bearbetning. |
|
|  | [getProcessedDocuments()](#getProcessedDocuments--) | Hämtar antalet framgångsrikt bearbetade dokument. |
|
|  | [getSkippedDocuments()](#getSkippedDocuments--) | Hämtar antalet överhoppade dokument. |
|
|  | [getProgressPercentage()](#getProgressPercentage--) | Hämtar procentandelen av framstegen. |
|
|  | [getLastDocumentKey()](#getLastDocumentKey--) | Hämtar nyckeln för det senast bearbetade dokumentet. |
|
|  | [getLastDocumentPath()](#getLastDocumentPath--) | Hämtar sökvägen för det senast bearbetade dokumentet. |
|
|  | [getLastDocumentStatus()](#getLastDocumentStatus--) | Hämtar status för det senast bearbetade dokumentet. |
|
### getTotalDocuments() {#getTotalDocuments--}
```
public final int getTotalDocuments()
```


Hämtar det totala antalet dokument för bearbetning.


**Returns:**
int - Det totala antalet dokument för bearbetning.

### getProcessedDocuments() {#getProcessedDocuments--}
```
public final int getProcessedDocuments()
```


Hämtar antalet framgångsrikt bearbetade dokument.


**Returns:**
int - Antalet framgångsrikt bearbetade dokument.

### getSkippedDocuments() {#getSkippedDocuments--}
```
public final int getSkippedDocuments()
```


Hämtar antalet överhoppade dokument.


**Returns:**
int - Antalet överhoppade dokument.

### getProgressPercentage() {#getProgressPercentage--}
```
public final double getProgressPercentage()
```


Hämtar procentandelen av framstegen.


**Returns:**
double - Procentandelen av framstegen.

### getLastDocumentKey() {#getLastDocumentKey--}
```
public final String getLastDocumentKey()
```


Hämtar nyckeln för det senast bearbetade dokumentet.


**Returns:**
java.lang.String - Nyckeln för det senast bearbetade dokumentet.

### getLastDocumentPath() {#getLastDocumentPath--}
```
public final String getLastDocumentPath()
```


Hämtar sökvägen för det senast bearbetade dokumentet.


**Returns:**
java.lang.String - Sökvägen för det senast bearbetade dokumentet.

### getLastDocumentStatus() {#getLastDocumentStatus--}
```
public final DocumentStatus getLastDocumentStatus()
```


Hämtar status för det senast bearbetade dokumentet.


**Returns:**
[DocumentStatus](../../com.groupdocs.search.common/documentstatus) - The last processed document status.

