---
title: "OperationProgressEventArgs"
second_title: "GroupDocs.Search για Java API Reference"
description: "Αναπαριστά τα ορίσματα για το γεγονός που ενημερώνεται η πρόοδος της λειτουργίας ευρετηρίασης."
type: docs
weight: 18
url: /el/java/com.groupdocs.search.events/operationprogresseventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class OperationProgressEventArgs extends BaseIndexEventArgs
```

Αναπαριστά τα ορίσματα για το γεγονός που ενημερώνεται η πρόοδος της λειτουργίας ευρετηρίασης.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getTotalDocuments()](#getTotalDocuments--) | Λαμβάνει τον συνολικό αριθμό εγγράφων για επεξεργασία. |
|
|  | [getProcessedDocuments()](#getProcessedDocuments--) | Λαμβάνει τον αριθμό των εγγράφων που επεξεργάστηκαν επιτυχώς. |
|
|  | [getSkippedDocuments()](#getSkippedDocuments--) | Λαμβάνει τον αριθμό των παραλειπόμενων εγγράφων. |
|
|  | [getProgressPercentage()](#getProgressPercentage--) | Λαμβάνει το ποσοστό της προόδου. |
|
|  | [getLastDocumentKey()](#getLastDocumentKey--) | Λαμβάνει το κλειδί του τελευταίου επεξεργασμένου εγγράφου. |
|
|  | [getLastDocumentPath()](#getLastDocumentPath--) | Λαμβάνει τη διαδρομή του τελευταίου επεξεργασμένου εγγράφου. |
|
|  | [getLastDocumentStatus()](#getLastDocumentStatus--) | Λαμβάνει την κατάσταση του τελευταίου επεξεργασμένου εγγράφου. |
|
### getTotalDocuments() {#getTotalDocuments--}
```
public final int getTotalDocuments()
```


Λαμβάνει τον συνολικό αριθμό εγγράφων για επεξεργασία.


**Returns:**
int - Ο συνολικός αριθμός εγγράφων για επεξεργασία.

### getProcessedDocuments() {#getProcessedDocuments--}
```
public final int getProcessedDocuments()
```


Λαμβάνει τον αριθμό των εγγράφων που επεξεργάστηκαν επιτυχώς.


**Returns:**
int - Ο αριθμός των εγγράφων που επεξεργάστηκαν επιτυχώς.

### getSkippedDocuments() {#getSkippedDocuments--}
```
public final int getSkippedDocuments()
```


Λαμβάνει τον αριθμό των παραλειπόμενων εγγράφων.


**Returns:**
int - Ο αριθμός των παραλειπόμενων εγγράφων.

### getProgressPercentage() {#getProgressPercentage--}
```
public final double getProgressPercentage()
```


Λαμβάνει το ποσοστό της προόδου.


**Returns:**
double - Το ποσοστό της προόδου.

### getLastDocumentKey() {#getLastDocumentKey--}
```
public final String getLastDocumentKey()
```


Λαμβάνει το κλειδί του τελευταίου επεξεργασμένου εγγράφου.


**Returns:**
java.lang.String - Το κλειδί του τελευταίου επεξεργασμένου εγγράφου.

### getLastDocumentPath() {#getLastDocumentPath--}
```
public final String getLastDocumentPath()
```


Λαμβάνει τη διαδρομή του τελευταίου επεξεργασμένου εγγράφου.


**Returns:**
java.lang.String - Η διαδρομή του τελευταίου επεξεργασμένου εγγράφου.

### getLastDocumentStatus() {#getLastDocumentStatus--}
```
public final DocumentStatus getLastDocumentStatus()
```


Λαμβάνει την κατάσταση του τελευταίου επεξεργασμένου εγγράφου.


**Returns:**
[DocumentStatus](../../com.groupdocs.search.common/documentstatus) - The last processed document status.

