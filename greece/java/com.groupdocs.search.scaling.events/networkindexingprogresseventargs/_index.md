---
title: "NetworkIndexingProgressEventArgs"
second_title: "GroupDocs.Search για Java API Reference"
description: "Αναπαριστά τα ορίσματα για το γεγονός αλλαγής προόδου της λειτουργίας ευρετηρίασης."
type: docs
weight: 14
url: /el/java/com.groupdocs.search.scaling.events/networkindexingprogresseventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class NetworkIndexingProgressEventArgs extends EventArgs
```

Αναπαριστά τα ορίσματα για το γεγονός αλλαγής προόδου της λειτουργίας ευρετηρίασης.

## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getNodeIndex()](#getNodeIndex--) | Λαμβάνει τον δείκτη του κόμβου δικτύου αναζήτησης. |
|
|  | [getServiceIndex()](#getServiceIndex--) | Λαμβάνει τον δείκτη της υπηρεσίας κόμβου δικτύου αναζήτησης. |
|
|  | [getProcessedDocuments()](#getProcessedDocuments--) | Λαμβάνει τον αριθμό των επεξεργασμένων εγγράφων. |
|
|  | [getTotalDocuments()](#getTotalDocuments--) | Λαμβάνει τον συνολικό αριθμό εγγράφων για επεξεργασία. |
|
|  | [getProgressPercentage()](#getProgressPercentage--) | Λαμβάνει το ποσοστό της προόδου. |
|
### getNodeIndex() {#getNodeIndex--}
```
public final int getNodeIndex()
```


Λαμβάνει τον δείκτη του κόμβου δικτύου αναζήτησης.


**Returns:**
int - Ο δείκτης του κόμβου δικτύου αναζήτησης.

### getServiceIndex() {#getServiceIndex--}
```
public final int getServiceIndex()
```


Λαμβάνει τον δείκτη της υπηρεσίας κόμβου δικτύου αναζήτησης.


**Returns:**
int - Ο δείκτης της υπηρεσίας κόμβου δικτύου αναζήτησης.

### getProcessedDocuments() {#getProcessedDocuments--}
```
public final int getProcessedDocuments()
```


Λαμβάνει τον αριθμό των επεξεργασμένων εγγράφων.


**Returns:**
int - Ο αριθμός των επεξεργασμένων εγγράφων.

### getTotalDocuments() {#getTotalDocuments--}
```
public final int getTotalDocuments()
```


Λαμβάνει τον συνολικό αριθμό εγγράφων για επεξεργασία.


**Returns:**
int - Ο συνολικός αριθμός εγγράφων για επεξεργασία.

### getProgressPercentage() {#getProgressPercentage--}
```
public final double getProgressPercentage()
```


Λαμβάνει το ποσοστό της προόδου.


**Returns:**
double - Το ποσοστό της προόδου.

