---
title: "OperationProgressEventArgs"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Stelt de argumenten voor het evenement voor wanneer de voortgang van de indexeringsbewerking wordt bijgewerkt."
type: docs
weight: 18
url: /nl/java/com.groupdocs.search.events/operationprogresseventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class OperationProgressEventArgs extends BaseIndexEventArgs
```

Stelt de argumenten voor het evenement voor wanneer de voortgang van de indexeringsbewerking wordt bijgewerkt.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getTotalDocuments()](#getTotalDocuments--) | Haalt het totale aantal documenten voor verwerking op. |
|
|  | [getProcessedDocuments()](#getProcessedDocuments--) | Haalt het aantal succesvol verwerkte documenten op. |
|
|  | [getSkippedDocuments()](#getSkippedDocuments--) | Haalt het aantal overgeslagen documenten op. |
|
|  | [getProgressPercentage()](#getProgressPercentage--) | Haalt het percentage van de voortgang op. |
|
|  | [getLastDocumentKey()](#getLastDocumentKey--) | Haalt de sleutel van het laatst verwerkte document op. |
|
|  | [getLastDocumentPath()](#getLastDocumentPath--) | Haalt het pad van het laatst verwerkte document op. |
|
|  | [getLastDocumentStatus()](#getLastDocumentStatus--) | Haalt de status van het laatst verwerkte document op. |
|
### getTotalDocuments() {#getTotalDocuments--}
```
public final int getTotalDocuments()
```


Haalt het totale aantal documenten voor verwerking op.


**Returns:**
int - Het totale aantal documenten voor verwerking.

### getProcessedDocuments() {#getProcessedDocuments--}
```
public final int getProcessedDocuments()
```


Haalt het aantal succesvol verwerkte documenten op.


**Returns:**
int - Het aantal succesvol verwerkte documenten.

### getSkippedDocuments() {#getSkippedDocuments--}
```
public final int getSkippedDocuments()
```


Haalt het aantal overgeslagen documenten op.


**Returns:**
int - Het aantal overgeslagen documenten.

### getProgressPercentage() {#getProgressPercentage--}
```
public final double getProgressPercentage()
```


Haalt het percentage van de voortgang op.


**Returns:**
double - Het percentage van de voortgang.

### getLastDocumentKey() {#getLastDocumentKey--}
```
public final String getLastDocumentKey()
```


Haalt de sleutel van het laatst verwerkte document op.


**Returns:**
java.lang.String - De sleutel van het laatst verwerkte document.

### getLastDocumentPath() {#getLastDocumentPath--}
```
public final String getLastDocumentPath()
```


Haalt het pad van het laatst verwerkte document op.


**Returns:**
java.lang.String - Het pad van het laatst verwerkte document.

### getLastDocumentStatus() {#getLastDocumentStatus--}
```
public final DocumentStatus getLastDocumentStatus()
```


Haalt de status van het laatst verwerkte document op.


**Returns:**
[DocumentStatus](../../com.groupdocs.search.common/documentstatus) - The last processed document status.

